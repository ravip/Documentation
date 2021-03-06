---
ID_PAGE: 25297
PG_TITLE: LensRenderingPipeline
PG_VERSION: 2.1
TAGS:
    - PostProcess
    - PostProcessRenderPipeline
---
## Description

class [LensRenderingPipeline](/classes/3.1/LensRenderingPipeline) extends [PostProcessRenderPipeline](/classes/3.1/PostProcessRenderPipeline)



## Constructor

## new [LensRenderingPipeline](/classes/3.1/LensRenderingPipeline)(name, parameters, scene, ratio, cameras)

@constructor

         * [Effect](/classes/3.1/Effect) parameters are as follow:

{

     chromatic_aberration: number;       // from 0 to x (1 for realism)

     edge_blur: number;                  // from 0 to x (1 for realism)

     distortion: number;                 // from 0 to x (1 for realism)

     grain_amount: number;               // from 0 to 1

     grain_texture: BABYLON.[Texture](/classes/3.1/Texture);     // texture to use for grain effect; if unset, use random B&W noise

     dof_focus_distance: number;         // depth-of-field: focus distance; unset to disable (disabled by default)

     dof_aperture: number;               // depth-of-field: focus blur bias (default: 1)

     dof_darken: number;                 // depth-of-field: darken that which is out of focus (from 0 to 1, disabled by default)

     dof_pentagon: boolean;              // depth-of-field: makes a pentagon-like "bokeh" effect

     dof_gain: number;                   // depth-of-field: highlights gain; unset to disable (disabled by default)

     dof_threshold: number;              // depth-of-field: highlights threshold (default: 1)

     blur_noise: boolean;                // add a little bit of noise to the blur (default: true)

}

Note: if an effect parameter is unset, effect is disabled

         * @param {string} name - The rendering pipeline name

#### Parameters
 | Name | Type | Description
---|---|---|---
 | name | string | 
 | parameters | any | 
 | scene | [Scene](/classes/3.1/Scene) | 
optional | ratio | number | 
## Members

### LensChromaticAberrationEffect : string

The chromatic aberration [PostProcess](/classes/3.1/PostProcess) id in the pipeline

@type {string}
### HighlightsEnhancingEffect : string

The highlights enhancing [PostProcess](/classes/3.1/PostProcess) id in the pipeline

@type {string}
### LensDepthOfFieldEffect : string

The depth-of-field [PostProcess](/classes/3.1/PostProcess) id in the pipeline

@type {string}
## Methods

### setEdgeBlur(amount) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | amount | number | 

### disableEdgeBlur() &rarr; void


### setGrainAmount(amount) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | amount | number | 

### disableGrain() &rarr; void


### setChromaticAberration(amount) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | amount | number | 

### disableChromaticAberration() &rarr; void


### setEdgeDistortion(amount) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | amount | number | 

### disableEdgeDistortion() &rarr; void


### setFocusDistance(amount) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | amount | number | 

### disableDepthOfField() &rarr; void


### setAperture(amount) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | amount | number | 

### setDarkenOutOfFocus(amount) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | amount | number | 

### enablePentagonBokeh() &rarr; void


### disablePentagonBokeh() &rarr; void


### enableNoiseBlur() &rarr; void


### disableNoiseBlur() &rarr; void


### setHighlightsGain(amount) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | amount | number | 

### setHighlightsThreshold(amount) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | amount | number | 

### disableHighlights() &rarr; void


### dispose(disableDepthRender) &rarr; void

Removes the internal pipeline assets and detaches the pipeline from the scene cameras

#### Parameters
 | Name | Type | Description
---|---|---|---
optional | disableDepthRender | boolean | 

