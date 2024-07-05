<form class="grid grid-cols-2 gap-3">
	<div>
		<label for="name">input-text:</label>
		<input class="input" type="text" id="name" name="name" required />
	</div>

	<div>
		<label for="name">input-text-success:</label>
		<input class="input input-success" type="text" id="name" name="name" required />
	</div>

	<div>
		<label for="name">input-text-warning:</label>
		<input class="input input-warning" type="text" id="name" name="name" required />
	</div>

	<div>
		<label for="name">input-text-error:</label>
		<input class="input input-error" type="text" id="name" name="name" required />
	</div>

	<div>
		<label for="date">input-date:</label>
		<input class="input" type="date" id="date" name="date" required />
	</div>

	<div>
		<label for="time">input-time:</label>
		<input class="input" type="time" id="time" name="time" required />
	</div>

	<div>
		<label for="datetime-local">input-datetime-local:</label>
		<input class="input" type="datetime-local" id="datetime-local" name="datetime-local" required />
	</div>

	<div>
		<label for="month">input-month:</label>
		<input class="input" type="month" id="month" name="month" required />
	</div>

	<div>
		<label for="week">input-week:</label>
		<input class="input" type="week" id="week" name="week" required />
	</div>

	<div>
		<label for="file">File</label>
		<input class="input" id="file" type="file" />
	</div>

	<div>
		<label for="color">Color</label>
		<input class="input" id="color" type="color" />
	</div>

	<div>
		<label for="textarea">Textarea:</label>
		<textarea class="textarea" id="textarea" name="textarea" required></textarea>
	</div>

	<div>
		<label for="select">Select:</label>
		<select class="select">
			<option value="1">Option 1</option>
			<option value="2">Option 2</option>
		</select>
	</div>

	<div>
		<label for="radio">Radio:</label>
		<div class="flex items-center space-x-2">
			<input class="radio" type="radio" id="radio1" name="radio" value="1" required />
			<label for="radio1">Option 1</label>
			<input class="radio" type="radio" id="radio2" name="radio" value="2" required />
			<label for="radio2">Option 2</label>
		</div>
	</div>

	<div>
		<label for="range">Range:</label>
		<input type="range" value="75" max="100" />
	</div>
</form>
