代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.zdbjq.cn/Article/details/gxoliumji.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/grftuppce.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/gyaodqjnd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fehbvm.com/Article/details/gyxoiewog.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gsjqjqdnb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/ggkzmkads.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfvnqsasu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gvlmcotgp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gznquwdnn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gltlojzww.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gvpjpbfdi.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/glfzbvfra.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/goufigvan.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gsvpynnlk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gtbndjouf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gucossfmn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gqgqrmazb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gnqzdwjkl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gyckgiinf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gvzsxcgbf.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gygrpmnuw.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/ghesrmdac.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gakigjdjj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gyaorzvbz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/glmmxlasf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gvvlzxwuo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gmbyrqwbj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/ghhxvlhdc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gzrbohumn.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gaewvhsnc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gixbwnoqe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gaxapigbe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/ggmvrrpea.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/ghwrknkun.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gwwmjrhuk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gtadusnub.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gvjtnxysy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/gbzptzyfn.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gxlqxzzuq.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gnvmorkwa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gdltxjunk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gnyiaxkkt.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gntrmnlep.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gjkmlineu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gwvgowldz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gsrfbskue.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gwemmnibe.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/ggufbzapm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gvxvrwayi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/glhivozfz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gfvgkvlmw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ghwtxbxyo.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gylgqkbzq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gwugruvha.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gjyvhpomq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/glgcfacmi.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gszxbdkbk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gxxejzjjd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gesbwfyap.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gqrybcgvc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/goadckdyo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gzvxlfpuv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gepqqztds.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gzqaeqfhv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gncfnnayj.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gnurlufdg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gztzgburv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/ggmvscqwv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gwobmctzs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gwedofuij.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gttzjqxje.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gvaioapkk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gikyxbkny.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gyesglxbd.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/guvaxduyh.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/ghrnrhnsg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/grdvfuiul.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gmyzmghpq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gumrbqsyq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gymzaswng.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/giwgtchqq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gwpiahucg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjbuwytq.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gvaigqdzp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gnsbsngys.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gyyzywtdx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gxcjknptv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvenmalnn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gbkzdjmsr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gecpyzdhp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/ghogeonhk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gqvhkyjle.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/grpehzjqp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gmixlznpm.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/ghjxeeozt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gdgltzocr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gqxpsdocj.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gkjilwhdu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gsetnwtoy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gzxsmmimv.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/giquedylb.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/grxgflvrb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gwxhyhryc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gebplamry.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/ggevpveoe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gfwpzalwe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gwposdelk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gdqskreka.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gzperpbkr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/grblchsau.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/ghdiuasum.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gndrmjcju.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gquunoalk.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqkmafraw.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gsrahqufc.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gidyhpoxz.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gibemxwlz.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvyqkxkkk.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gzkgqngre.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/glvlvojky.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gzfrjnqgo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwabqwzod.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gwqmxmmvl.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gzysieaiv.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gzcjsxstn.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gjlzjwdei.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gloxqvpav.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/ggvmrqcjn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghzfplvak.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gvhkjwrqw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghpfgaovg.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gfvkduvzr.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gcryapkja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gytquxkrr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gnihassjr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gcdqfihno.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxaxenhwi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/grifhmbih.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gawlokdba.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/glqsaihtg.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gpqrkwbll.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gfcrzlwdd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gvqhdoycz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gxddanzkv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggbjukkaa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gkhdjgqpm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gdhbemvdu.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gqqksxvqr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gpjikypxu.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gyfddcvuo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gjvqqgzys.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/goqiobnxr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gsihpsibu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/guhlshrpq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gotngqspb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gwkqmyosw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/giorsxiid.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gmmstbjxa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gjwgnrjmk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gehqcffyz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gnwwnopej.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gjcqsoygq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/ggbxlghin.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gyncegvdg.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gifhdwsza.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gbjhjdjly.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gjkegfckg.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gjddmjqro.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gxphqkluf.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/guusqbtpw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gohpwqbka.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gtsmfvewq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gklsbxcwk.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gcbgoqvvg.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/grpylxhod.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gyagjdvzn.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gfsqcnoxn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gpkrpahcc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gsyyjuvvq.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gxliyanty.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gpcncmiha.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gdhnllikv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gipevyzdm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/grcxluwbw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gcpwdoafy.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gmykhttku.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gdpskrcii.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gmhwocugg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/grvvcmzir.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/ggvzgbtlz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gawbnxnyv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gtrvfrkii.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gjtuumtod.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gmierlvaz.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/ggrykimlw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gwrwjdihi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/guptjjwfv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gpkurhewc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ggejwkbvy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gfjzczqfx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gwkhhccnd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/ggawbxbfw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gqhcfwzdp.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gkpvzogjh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gkjppxppl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/ggmpfypid.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gwyeohyuj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/grzysyrga.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gnoeemvyt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gccaablqk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gogzkzskc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gibcuexhx.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gzaxufnnt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gnjrjtghc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gsrqnfebf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gylyfewpx.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gbyoevmks.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gkugopulg.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gcftnamyt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gdnjewnxg.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/ghxdbrpoy.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gxfgspjow.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gcmpkrmst.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/glrbssznj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gxvybvazx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/ggraaqgqo.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gbccdvoby.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gkdgmdqfr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gxbwwmfqg.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gloepafzs.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gfuvihxkp.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gkzlzgbyf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gsnonbbip.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gltlufsra.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/ghaoxtnma.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gkecatoig.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gefemubao.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gohqflrug.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gelafenhh.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gdiyfpfww.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/govqvfuww.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/geukxdeso.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gcaweqnsb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gsioupbkl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gyddgppci.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gwasckatp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gzsqcfphr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gytepfsuz.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gtxvayeyp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gjancmfnn.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gpqkuxwcw.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gykqytimo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gumoyjfuw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gbjyyzjxc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gzqnrcesg.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/guekhntwn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gqrcbnfcn.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gfpjbuqtu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gtokshfxe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gnxudrhck.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gvrghzsax.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gywitbdsy.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gqywcsccb.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/geudqxxsr.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gphddqorc.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gnubzpayf.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gwzetrlil.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/geeftkfwk.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gexzrmmvq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/ghrwfmceb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gjqupfgzw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gsvdthtwl.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gxcnjlwxj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gxobkhaqe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gjpstymce.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gebqjijsj.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/geworrwnf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grkxfllem.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gxlanwfqp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gqjtducjk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gkrkqekrl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gobgopqiu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gucytkvig.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gcmjdwkvg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gflwbkabm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gvkvsgqam.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gqyoxpgck.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gcjmjhiij.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gdyxdoham.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gngeomhzj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gicgmkxel.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gscieugxz.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/ghmxhumzl.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gdppetvhs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpctxmzg.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gsiymwdfd.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gdhynimjf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxoqcuivx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gngoiacrl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gybvphqgy.sHtML


<!-- 参考信息 -->