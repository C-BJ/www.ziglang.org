---
title: Performance Tracking
type: "perf"
mobile_menu_title: "Performance Tracking"
---

This project exists to track various benchmarks related to the Zig project regarding execution speed, memory usage, throughput, and other resource utilization statistics. 

The goal is to prevent performance regressions, and provide understanding and exposure to how various code changes affect key measurements.
<div id="tooltip" class="tooltip">
	<div class="title">
	<span class="benchmark-title"></span> > <span class="measurement-title"></span>
</div>
	<div class="contents">
		<table class="benchmarks">
		<thead>
			<tr>
				<th>Measurement</th>
				<th><a href="/documentation/master/#Debug">This commit<br /><span class="current commit"></span></a></th>
				<th><a href="/documentation/master/#ReleaseFast">vs previous</a></th>
				<th><a href="/documentation/master/#ReleaseFast">vs first</a></th>
			</tr>
		</thead>
		<tbody id="tooltip-measurements-table-body">
			<tr>
				<td>CPU Cycles</td>
				<td class="cpu_cycles this"></td>
				<span class="cpu_cycles previous change"></span>
				<td class="cpu_cycles first change"></td>
			</tr>
			<tr>
				<td>CPU Instructions</td>
				<td class="cpu_cycles this"></td>
				<td class="cpu_cycles previous change"></td>
				<td class="cpu_cycles first change"></td>
			</tr>
			<tr>
				<td>Cache References</td>
				<td class="cache_references this"></td>
				<td class="cache_references previous change"></td>
				<td class="cache_references first change"></td>
			</tr>
			<tr>
				<td>Cache Misses</td>
				<td class="cache_misses this"></td>
				<td class="cache_misses previous change"></td>
				<td class="cache_misses first change"></td>
			</tr>
			<tr>
				<td>Wall Time</td>
				<td class="wall_time this"></td>
				<td class="wall_time previous change"></td>
				<td class="wall_time first change"></td>
			</tr>
			<tr>
				<td>User-Space Time</td>
				<td class="utime this"></td>
				<td class="utime previous change"></td>
				<td class="utime first change"></td>
			</tr>
			<tr>
				<td>Kernel Time</td>
				<td class="stime this"></td>
				<td class="stime previous change"></td>
				<td class="stime first change"></td>
			</tr>
			<tr>
				<td>Max RSS</td>
				<td class="maxrss this"></td>
				<td class="maxrss previous change"></td>
				<td class="maxrss first change"></td>
			</tr>
			<tr>
				<td>Branch Misses</td>
				<td class="branch_misses this"></td>
				<td class="branch_misses previous change"></td>
				<td class="branch_misses first change"></td>
			</tr>
			<tr>
				<td>Samples</td>
				<td class="samples_count this"></td>
				<td class="samples_count previous change"></td>
				<td class="samples_count first change"></td>
			</tr>
		</tbody>
		</table>
		<table>
		<thead>
			<tr>
				<th>Info</th>
				<th><a href="/documentation/master/#Debug">This<br /><span class="current commit"></span></a></th>
				<th><a href="/documentation/master/#ReleaseFast">Previous</a></th>
				<th><a href="/documentation/master/#ReleaseFast">First</a></th>
			</tr>
		</thead>
		<tbody id="tooltip-commit-table-body">
			<tr>
				<td>Commit Hash</td>
				<td class="cpu_cycles this"></td>
				<span class="cpu_cycles previous change"></span>
				<td class="cpu_cycles first change"></td>
			</tr>
			<tr>
				<td>Committed</td>
				<td class="cpu_cycles this"></td>
				<td class="cpu_cycles previous change"></td>
				<td class="cpu_cycles first change"></td>
			</tr>
			<tr>
				<td>Benchmark Ran</td>
				<td class="cache_references this"></td>
				<td class="cache_references previous change"></td>
				<td class="cache_references first change"></td>
			</tr>
			<tr>
				<td>Zig Version</td>
				<td class="cache_misses this"></td>
				<td class="cache_misses previous change"></td>
				<td class="cache_misses first change"></td>
			</tr>
		</tbody>
		</table>
	</div>
</div>
<script src="https://cdn.jsdelivr.net/npm/tweakpane@3.0.5/dist/tweakpane.min.js"></script>
<script type="text/javascript" src="d3-7.1.1.min.js"></script>
<script type="text/javascript" src="perf.js"></script>