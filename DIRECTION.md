# Research direction

## The question

Can heat from the atmosphere be captured as electrical charge, at a scale worth using?

The founding questions are recorded word for word in INQUISITION.md. This file holds the analysis that came out of them.

## How the question narrowed

1. A material question. Does heat change an electron state in a way that can be captured as charge? Answer: yes, in several material families.
2. A source condition. The heat source is the atmosphere.
3. A mechanism proposal. Use the movement of thermal particles to force electrons into a higher orbital state.
4. An interface change. Air particles and electrons work at mismatched scales, so capture the shared movement of a fluid instead: drafts, eddies, a funnel, and capture at the tunnel wall.
5. A survey request. What current work exists in that direction?

Each step removed one wrong assumption and left a harder, smaller question.

## What is established

### At the electron scale

- Heat widens the spread of electron energies. A few electrons cross a barrier they normally cannot cross.
- Uniform heating gives no usable output. Excited electrons fall back where they rose. Capture needs a structure that lets them fall back through a wire.
- At 300 K the average thermal energy per particle is 0.026 eV. The share of electrons above a jump falls fast as the jump grows.
- A 0.05 eV jump: about 14% of electrons above it at any instant. A 0.10 eV jump: about 2%. A 0.15 eV jump: about 0.3%. A 1 eV jump: effectively none.
- Thermal motion is a spread of energies, not a promise. More collisions do not build up toward a guaranteed jump for one electron.
- A free electron has no orbital. Orbital states belong to electrons bound in an atom, a molecule, or a solid.
- In a solid, lattice vibrations stay in permanent contact with the electrons. That contact is the working form of the mechanism in step 3.

### At the source scale

- Air at one uniform temperature holds heat but no extractable work. A heat source needs a colder side before any of its heat can become electricity.
- Two free cold sides exist. The night sky, reached by radiation to space. And the air temperature of a few hours ago, stored in a heavy material that warms and cools slowly.
- Air is a strong source when the wanted output is heat. Air source heat pumps deliver about 3 to 4 units of heat per unit of electricity used. That is the control case every electricity route must be compared against.

### At the flow scale

- A flow carries two kinds of energy. Random thermal motion, which cannot be captured directly. And shared drift in one direction, which can.
- Raw power in a flow, per square metre of capture area: air at 3 m/s carries 16 W. Air at 5 m/s carries 75 W. Water at 1 m/s carries 500 W.
- A funnel raises speed at its narrow point. It does not raise total power. Total power is set by the area of the mouth.
- At draft speeds, air barely compresses. Stopping a 3 m/s draft raises its pressure by about 0.005% of atmospheric pressure. A passive tunnel does not create a useful hot spot.
- A wall that does not move does no work, however many particles hit it. Collisions with a fixed wall end as load on the structure and as friction heat.
- A moving wall changes that. Blades, rotating discs, and flexing membranes all take work from the same collisions that a fixed wall wastes.

## Open routes

### Route 1: direct thermal excitation in a narrow gap material

Use a semiconductor with an energy gap of 0.05 to 0.15 eV, so room temperature heat excites a steady share of its electrons. Sweep each excited electron into a circuit before it falls back, which happens within nanoseconds.

Known materials: bismuth telluride at 0.15 eV, indium antimonide at 0.17 eV, mercury cadmium telluride tuned below 0.1 eV.

Cost of the route: each captured electron carries little energy, so output voltage per junction is low and many junctions must be stacked.

### Route 2: atmosphere against the night sky

A panel facing a clear sky radiates heat to space and cools below air temperature. A thermoelectric module sits between the warm air and the cold panel.

Published result: a Stanford rooftop prototype produced about 50 milliwatts per square metre at night. Source: [Stanford report](https://ee.stanford.edu/shanhui-fans-moonlight-solar-panels-enables-electricity-generation-night).

Open test: how far humidity and cloud cut that output in a Gulf Coast climate, where the sky window is often closed.

### Route 3: atmosphere against its own past temperature

One side of a device follows air temperature fast. The other side sits in a phase change material, a substance that melts and freezes near room temperature, and lags hours behind. The gap between the two sides drives a thermoelectric module.

Published result: an MIT device using the day and night swing produced 350 millivolts and 1.3 milliwatts from a small sample under a 10 °C swing. Source: [project report](https://newatlas.com/mit-thermal-resonator-temperature-changes-electricity/53456/).

Open test: tuning the lag to a local climate, and total energy per day per square metre, not peak power.

### Route 4: flow capture

Capture the shared drift of air or water: thermal drafts, eddies, wind, and currents. This route became its own project: [ductricity](https://github.com/Foundation-0/ductricity).

Published state of the field, from the survey in this project: funnel systems around a conventional rotor are at pilot stage. Vortex oscillation devices work at about 100 W after a decade of development. Flutter and wall charge devices sit at milliwatt scale in laboratories. No large solar chimney has been built since the 50 kW Manzanares prototype ran from 1982 to 1989.

### Route 5: water at a charged wall

Water moving through narrow channels with charged walls drags ions with it and creates a voltage. Evaporation can drive the flow, so no pump is needed.

Published result: an EPFL device using evaporation, heat, and light reached 1 volt and 0.25 watts per square metre. Source: [EPFL report](https://actu.epfl.ch/news/nanodevice-produces-continuous-electricity-from--2/).

Open test: output held over weeks, and output per total device area when channels are packed into a panel.

## Test programme

### Phase 0: predictions before building

- Pick two routes. Write the predicted output with the numbers behind it, before any test.
- State the capture area, the total device area, and the weather the prediction assumes.

### Phase 1: desk models

- Build a model for each picked route from the relations in this file.
- A route stops here if its modelled ceiling, under local climate data, falls below 0.1 watts per square metre of capture area with no path upward.

### Phase 2: bench tests

- Measure net power only. Subtract any power used to drive flow, compress air, or cool a surface.
- Report power per capture area and power per total device area as two separate numbers.
- Record temperature on both sides, flow speed, pressure drop across the device, and test duration with every result.
- Label every number as measured, modelled, or claimed by others. The three do not mix.

### Kill rules

- A route dies if measured net output stays under one tenth of its Phase 0 prediction across three tests in the conditions the prediction assumed.
- A route dies if its output needs a flow, a pressure, or a temperature gap that the test site does not provide for free.
- A dead route stays in this file with its numbers. It is not tested again without a new mechanism.

## Open questions

- Can one surface shape a flow and extract from it at the same time, without the extraction stalling the flow? This is the ductricity question.
- Which narrow gap material holds its gap and its contacts after months at outdoor humidity?
- Can a stack of junctions on Route 1 reach a useful voltage before heat leaking through the stack cancels the gain?
- What does Route 2 produce across a full humid summer, night by night, rather than on the best clear night?
