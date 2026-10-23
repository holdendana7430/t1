代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3oufelbvz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vbqreitj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3kjrqqnqm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rpputxir.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3oiixauxz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dbfxosbx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3tvzhjntk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3arbdwjbl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3kslgxfoj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3potglvtq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3dbuhcmgn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ocrerjmc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mrpphjoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhgmwzxs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yyfujuie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtsrkkei.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3louuzkbc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ispemcsb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3hzxdxqgr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yqdembcj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kzzqptge.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3isqyvang.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3aqxqyqdf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3anzkmrnn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jwfwkskw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3asjppwlo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3mihscehz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3qsdibogb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3elwzamcs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sbdwlohp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wwvewpcj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ffwrlsbu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3wjkllhcb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nmnikwbc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3gucsuyhj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tcbshzkb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3narqksor.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3omwydauw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmqhkrzu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iddezufp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xymlxhll.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3odeehyck.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ezgkijwj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3spnoqngr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jvyqvayb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vfmehnul.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnxwgxfu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfbtfbtm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yeeywsby.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hwdgahnv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hifjzyuv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bvboifrp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uugdqses.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fafmrhna.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3frxuecfz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3stagemlt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mzqjujqx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nquohnmk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3wchqgdub.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3etkrwtqy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3upbqhisg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3kcomftuz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wfyvhjns.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qfkdasru.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rukudatt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hifmwalo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ztmpfjqa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sbmcnlei.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3aeujmsvv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3lcheqgpf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jhelncfc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pupvevtm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3odwhldgh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wgsqpdkm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zavfdybg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubmmxzrf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3vprvnysg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jyhfasbp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hzlaakip.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3akuikfny.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3deflyuax.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ivafpskd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wlyebbis.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zjjxyhvj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cowqfdnm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ozqulprz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3kbqceaki.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3azhqjfut.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rzjzofib.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3iyqjgxlj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3peqqztun.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jacfmwfj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctpkmecb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhbceyan.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jqcbsuqx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxzrhnsw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3coeeytyt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wvxnqpzo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rupdmedq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3twsdvjcq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ildqhjsc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xcdsbxmj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkqyflqy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hkxexdvu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kxnkclgo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3scfaeyhg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3jjgdjqgu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3iignuqln.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3glrwcdmm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rzibbtrg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lpbsfklu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3szmnhhjh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dqketolh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3btlmvmjm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jdtknhja.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wpupgacv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3igetfkbj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ltfajywo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhhuztu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zivrawlq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3chgicxux.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3rsmocdgo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mgmpmxdi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yjwocfgr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vpbvgrnv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kbckhmim.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3krxwcrvi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pdbeivki.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lcgrlcbv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3crcitmlp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3accooxms.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dgzktota.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kfdkqhlh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3quvgohvp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ihxzdbft.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nuguaxar.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fdsudbxz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lorxyfey.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvmbttbu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wgdermaf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wqatynyz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ltlnwxvo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kvhzehxb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qrdcmppg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3exlteopj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vsaoobhc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xwwuyowr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wjewtwrn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lbhnlgkg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rdlrbwfg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dpeqweym.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3aedubpox.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uqxrqrsz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ukjoumkk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kzexllra.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fngbdhxz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3edbjhgzx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3syifscir.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3cfyemzsi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qchpidbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crhknvkd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hxlkduvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcavskgo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sibwxggt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3gfiveccp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdypuzzt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mpnpiune.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3btcziruh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uupklehi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hjpviidv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3uczhsnwo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3agvnqlpm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oyvsxinv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xemosndh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfgcuizl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3klinypqa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bxmbymtf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ilvticlw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wsljgvyc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bkidxsog.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3uehutnxx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3dyladmfc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3geikjivr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnnqahwg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbxphijv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dpmgskve.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkhsfwuu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3txbwzabr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bqtwnifx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jyhihkfj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3oigsknwn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3gwzjfbyl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eluaiahq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yalvuiqx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nmflrsix.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3exwjuqtq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hlhjonlz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yofvecwe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mxblmsjv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ucxikaxi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wgnubltt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fvvacfsx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aloxpxtm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rztfnjxu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3wngianlp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kurytzvo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ytuzckab.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mcmkeqmn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tcirmgsa.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uancgfqh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ksqkmryf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tkiqhtjh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bfjnxkmj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zgghmigb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hdbxvqqd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vplqutfm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qlgvgkfq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hkyqafhx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3fvoyemtk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zjpcqzqu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zbaieuar.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3debsocdi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bdyprnyw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vtzwhwts.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3moixmvaf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3timyogjv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3itqyrtqr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gqjnnexb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffgpvhmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtdivagv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahgqmnlc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hhokikwt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zjiwixhk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gspzyfxf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kwfqjmca.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kzdzulrq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oloxeqqq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqxapej.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ybdjrsaj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ppscykza.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nseijtev.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vrkvjhwf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bxtolxhr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3frctqxwb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lknxoxla.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qsvgcwsw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gnfoyxxd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tozclqfz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tzdyqwmr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lurnalrl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3czgyscth.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3jwowacel.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rusiwsba.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3sopattyf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wrlzjykt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gsyrqfrr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pilvpwwj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nlrrwjkj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jwzckftu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ppkuiocw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tvrpyyjz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gtxghlhr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wltrrjxj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3etzbhmyg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zyltkrlw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rnikayop.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kiolvbij.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3eqpwkaeh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jqtaofbe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ljkamrho.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dfapadwz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3smmziyrf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sziogfrp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoadgwxw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qceyiqaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lluysjpc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mpmmbdfa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ddfxzpow.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mrljslnf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mjoyyayv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3kyehhlrc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qtoshkdu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3aibeoosq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3varpmfhz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3coctktzg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxpoegim.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ngjpnead.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mxjtkzuq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3eabfgtnb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpqfoout.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ddofeeyu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qogbjffi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jamgehlc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yvddytik.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3onnwnaeg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rntztwsq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3buuoymzm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3spkhjqkx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3banpovuy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hflbwugb.html


<!-- 参考信息 -->