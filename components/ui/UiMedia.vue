<script>
import classnames from "classnames";

export const UiMedia = {
  props: {
    gap: {
      default: "m",
      type: String
    },
    tag: {
      default: "div",
      type: String
    }
  },
  render() {
    const Tag = this.tag;
    return (
      <Tag class={classnames("media", `media--gap-${this.gap}`)}>
        {this.$slots.default}
      </Tag>
    );
  }
};

export const UiMediaFigure = {
  props: {
    align: {
      default: "start",
      type: String
    },
    tag: {
      default: "div",
      type: String
    }
  },
  render() {
    const Tag = this.tag;
    return (
      <Tag
        class={classnames(
          "media__figure",
          `media__figure--align-${this.align}`
        )}
      >
        {this.$slots.default}
      </Tag>
    );
  }
};

export const UiMediaBody = {
  props: {
    align: {
      default: "start",
      type: String
    },
    tag: {
      default: "div",
      type: String
    }
  },
  render() {
    const Tag = this.tag;
    return (
      <Tag
        class={classnames("media__body", `media__body--align-${this.align}`)}
      >
        {this.$slots.default}
      </Tag>
    );
  }
};

export default UiMedia;
</script>

<style lang="scss">
$gap-m: 1em;
$gap-l: 2em;

.media {
  display: flex;
}

.media__figure {
  &--align-center {
    align-self: center;
  }

  &--align-end {
    align-self: flex-end;
  }

  &:first-child {
    .media--gap-m > & {
      margin-right: $gap-m;
    }

    .media--gap-l > & {
      margin-right: $gap-l;
    }
  }

  &:last-child {
    .media--gap-m > & {
      margin-left: $gap-m;
    }

    .media--gap-l > & {
      margin-left: $gap-l;
    }
  }
}

.media__body {
  &--align-center {
    align-self: center;
  }

  &--align-end {
    align-self: flex-end;
  }
}
</style>
