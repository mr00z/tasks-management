<script lang="ts">
  import { mergeClassNames } from '../../utilities';

  export let value: string | string[] = '';
  export let className: string = '';
  export let placeholder: string = '';
  export let readonly: boolean = false;
  export let disabled: boolean = false;
  export let isInvalid: boolean = false;
  export let alt: boolean = false;
  export let size: 'large' | 'regular' | 'small' = 'regular';
</script>

<textarea
  class={mergeClassNames(className, 'form-control')}
  {placeholder}
  {readonly}
  {disabled}
  {value}
  class:is-invalid={isInvalid}
  class:alt-dm={alt}
  class:form-control-lg={size === 'large'}
  class:form-control-sm={size === 'small'} />
