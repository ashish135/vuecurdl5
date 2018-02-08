<template>
	<div class="create-task">
		<form action="" method="POST" id="create-task">
			<input type="hidden" id="_token" name="_token" :value="csrfToken">
			<div class="form-group">
				<label for="title">Task Title</label>
				<input type="text" name="task-title" class="form-control" />
			</div>
			<div class="form-group">
				<label for="task-desc">Task Description</label>
				<textarea class="form-control" name="task-desc"></textarea>
			</div>
			<div class="form-group">
			    <button class="btn btn-default">Add Task</button>
			</div>									
		</form>
	</div>
</template>

<script type="text/javascript">
	export default{
		computed: {
			csrfToken: function(){
				console.log(window);
		    }
		}
	}
</script>