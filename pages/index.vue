<template>
  <UiGrid>
    <UiGridItem :width="['12/12', '4/12@m']">
      <h2>The Sidebar</h2>
      <p>Some sidebar content ...</p>
    </UiGridItem>
    <UiGridItem :width="['12/12', '8/12@m']">
      <h2>Main Content</h2>
      <UiMedia>
        <UiMediaFigure>
          <img
            src="https://images.unsplash.com/photo-1510798831971-661eb04b3739?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=70&h=70&q=80"
            alt=""
          />
        </UiMediaFigure>
        <UiMediaBody>
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam
          nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
          sed diam voluptua.
        </UiMediaBody>
      </UiMedia>
      <br />
      <UiMedia>
        <UiMediaBody>
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam
          nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
          sed diam voluptua.
        </UiMediaBody>
        <UiMediaFigure>
          <img
            src="https://images.unsplash.com/photo-1510798831971-661eb04b3739?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=70&h=70&q=80"
            alt=""
          />
        </UiMediaFigure>
      </UiMedia>
      <br />
      <UiMedia>
        <UiMediaBody>
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam
          nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
          sed diam voluptua. Lorem ipsum dolor sit amet, consetetur sadipscing
          elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore
          magna aliquyam erat, sed diam voluptua.
        </UiMediaBody>
        <UiMediaFigure align="center">
          <img
            src="https://images.unsplash.com/photo-1510798831971-661eb04b3739?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=70&h=70&q=80"
            alt=""
          />
        </UiMediaFigure>
      </UiMedia>
    </UiGridItem>
  </UiGrid>
</template>

<script>
import { UiGrid, UiGridItem } from "../components/ui/UiGrid.vue";
import {
  UiMedia,
  UiMediaBody,
  UiMediaFigure
} from "../components/ui/UiMedia.vue";

export default {
  components: {
    UiGrid,
    UiGridItem,
    UiMedia,
    UiMediaBody,
    UiMediaFigure
  }
};
</script>
