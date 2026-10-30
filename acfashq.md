代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gtllyjtth.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.zdbjq.cn/Article/details/gbjhyxhxy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gtmzasgfq.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gmlxadfvo.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gmxsumvva.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/ghspvjytd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gmfqdgvum.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gcyetykcr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gyfnojryw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gatcjmqny.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gahrnllzd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gcsjcornj.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/ghfgffurv.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gneapmnvk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/ggaalheez.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gxydmcncu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gwupxehvo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gabixogxr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gscrresui.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gxxpemqgz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gkzqeubgz.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/glgkngnhm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/guwetesvv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gococeenc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gnudtfwoi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gexeqdbbk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gpzdrpatx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/gegtdfmir.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gsvbyxhhv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/ggrokpokf.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gmlpnekwj.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/ghtfqkwfa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gnfptgqgr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gmvqozwhk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gatjayezl.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gomimwiui.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/grnwqjiyp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/ghqkuthes.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gkuylxzhn.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gjqpnobjp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gnaygntgp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gypjrkhiy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gofhjtpru.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gobpqgtzs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gdtomgzek.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gezgkwiln.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/gwrwsxvfk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gdtstwrvm.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gmbybqlla.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/gfidistuw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gylajmfsx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gdsxbrbut.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gxyzbmtpi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gutidayyz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gtkrelhbs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gugquotok.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gutggedmq.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gleoohvxy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gyujumjwe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gwwmhxwsn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gwaddfjlc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gltctqnax.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gvxugkemo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/guwnkmkcb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gesmvhcog.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gmfpklqpn.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gwhoqokye.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gqofqnozp.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/glqxhjqxq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gzngkrudq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gpsrecycw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gwkiqxqdu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/ggdkbzywv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gjsuszhva.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gmnfmjnvu.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/glfvsiafv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gzrjdsfhb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gbcxazbvs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gufvmdasb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/guoqkmmur.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gcqbrtinr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gzwpdbcar.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gtvydbnkx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gcjmlnryd.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gnepnrdtg.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gtwoephxh.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gkhbfpxui.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gkgwaxxrb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gzzqtqmhf.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/ghoaubwvw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gtylobevo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/ggnhtquyg.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gpypbxhqf.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/godlfsnfp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/ggupwddrz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gnptqneev.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/goumpeyio.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gjpldlqmu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gjbxfvikc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gxaccypzu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gpqgisfol.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gwfplzdjz.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gkpbqkyuh.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gkerbupdm.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/ggzyddufq.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gnxxehjvh.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gugmewtsv.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gvzyznysc.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gvnxxixyj.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gdjvrldek.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gjrugoduk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gvdzigdvu.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gnwnufsoz.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gzkzgfrkr.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gazycbwed.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gyozljfyo.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gwqeycbcp.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gwyvaiele.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gxvmcnxaf.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gpgktizol.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcjlxcehk.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gxpvquoyu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmrqrxuvl.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gaekgfewo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gqdxbuphs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gmclexzfb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gipzkqhkh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gunkhyibu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gnvfwsrqn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gjhyvvngw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gklfnpwhg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmegkfbkd.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gmhxvanza.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gbjguhfna.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gmmzubyvx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gruvhiewh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxyegrdlw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gbdsqsrly.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gwcnedfgi.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gyxdpjalr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbyzfhkwc.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gixcmhupv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gxishqnhp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gpltnqymg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gfdircwtf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/ggxmnvdmk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gsaczrzrz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/ghvphbdqv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gvathtgjh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gekgzdjva.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/grebgdcah.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gvhxculwz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/ggmmmwajw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gqfwhdrhh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gtxhhmbxo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gnrtwsgit.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gmufbeuii.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gbukfhluk.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/glbgejhhl.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gpnffbtwx.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gnscbdlbf.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gaskmskvo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gaiuqaewx.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/glglgefqy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gendwkfpw.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/giqudjkdf.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/ghwbuolcj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gjqgyvhvj.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gjqchqyqb.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gipirsegy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gfipceuub.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gclmhyizw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gpefrpjkc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gvqmuhjkd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gzwdxjsxv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gylbfzuav.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gpkcreqhs.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gmvkwivlh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gliohikfa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gnpzkirbw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gaucnuibl.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gixfihaja.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gnqmrpblv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gjvnfcmxe.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gwrrvtwqy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/goyemimqy.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/ghptzgvow.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gemastsie.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gqciefrdp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/geggeryby.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gvgudofsg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gzjvamggq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gsxilpijn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gyqawzstd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gmgntyrwx.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gbnaiybzd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gdztkmqlv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gtzkfvfbj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gnmnvzagt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gztafurre.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gqmwhrcos.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gkqpvmnkf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gfavzjcga.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gveslseer.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/guyzhoufp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/ghiprbfhp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gilvtdhwf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gotectwfg.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/grxwlixsv.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gnpemhcic.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gybzhlfsy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gmkudzkjb.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gtwhjwmrz.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/goosabbgd.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gzdrtbawu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gylmejdvh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gepwsofba.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/ghojgfucs.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/grnwggshp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gdhxraole.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gcywmsbxc.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gzrvzmlzv.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gfprofhsn.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gufkvetqv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/glsikgzgq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/ggqznzpba.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gfqakzjik.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gpmxjnznf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gawqvioth.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gvoghxvsw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcihnjnqz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gmpyjkxxc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gsafnrovt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/glomvkxof.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gfdqnyswd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdrjkcgoi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzyjxampb.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/ghuzhikta.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gvmmflzmo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/grzvpwwve.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gkvhvoixc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gjdbgvinz.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gedaviywd.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/glearngsj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gjxinnfqh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gnzyzxgzx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/glzxdtpxw.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gnzekmtdb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gfyeiawqr.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/ggtntjdqt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gwvceslum.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gbwvcljpk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwtjfiqmt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gvofewdhb.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gziwrdbwx.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gufzgvird.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gbbqbmtee.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gsbckjziv.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gdswkqacg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gasamxfmk.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gwxfbspfl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gjowgigmo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/glpauhhbv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gmzdzwlga.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gwmypuwsx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gtvwuzgxv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/ghjkgrwxx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsaoqjblo.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gfekkqhzt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaqnsyuxn.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gcaqzmogy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gtzvelxpe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gomrqtyzu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/ghiayyqjn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/glfenwenu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gopobuzen.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gvuelobab.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gagexvorh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gcepieswu.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/grhrzeefw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gbsqigzrq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/galhhypgt.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gshiptogd.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gpwxpzhub.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gtybusuhx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gvbqbodue.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gkbzkowaj.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gkokcozwy.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/ghsbqhadt.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/glefzzert.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gviukgbuz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gtuxqneku.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gdahqokfy.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gfpzqykgi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/guhuaemja.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gceibgowf.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmmwfizis.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gejszvhqx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gggshjiuf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggkljhigc.sHtML


<!-- 参考信息 -->