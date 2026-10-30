代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/guevvemaw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.hesvh.cn/Article/details/gsrftxpla.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/giagmpyrm.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/ghkcrndog.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhaofmnt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.zdbjq.cn/Article/details/gamintgld.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gqrytdjmd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/ginztyvth.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/glzkqatsk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/gylwoydth.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.zdbjq.cn/Article/details/gtmhfvcit.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gweltzvtm.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gcpqbsdqr.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gmzizfmxc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gluonfbvi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gjxqpgjde.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gedbupnyn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gpticeatu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjqrtuhf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gghbdaewt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gwmmczguu.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gneubtpyu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gikoqdfet.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gztgjhgvl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gtfgfxyzv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gytkuxlol.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gojojqdbu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gkbwxcruu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gxceqtoyz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gyyjwpjpp.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/gvigmdxoj.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gkzgltduo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzcwhwol.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gtoztqwiv.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gkjxmxwsr.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gtiiymozw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gmmynxgzf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gmaojmdwo.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gvrnnxuir.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gnhbkzugz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gwhjhtzdo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gbjvgigqg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gypaeaumc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gvolgvdyq.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gnqdimvnc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gjlekvxcj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gidpqtpxq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/giptnpsas.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gqkgyjogz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/glbvevmdd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/grppveoir.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gdepaulwz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gfnbhpzhg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gulvyfgkd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gokrjaiei.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gyzqvatta.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gwwltlkrr.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gjquzkhnc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gwigkpqps.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gqpjxwrei.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gjezcymss.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/ghumfbipt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gxcrrcmkd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/geducuxvx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gnnuuycxf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gczeodgiu.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gkczmsgru.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/govpietjd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gjdqxguki.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqvdafoof.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gnjcfmwlk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gdewojndx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gqhhwqjlh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gmakradai.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gbqrzurpq.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gpgthsxhu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/ghhgafkwl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/goenpgayu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwjbthguh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/ghreelocn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gddgbzrkr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gpjtdmymf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gzdufiisr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gysifzeru.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/guegcsldj.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gatmzykxx.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gsbzjwagj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gcoioggvb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/grcacnvyq.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gtzuuxqyz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gukqxviso.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gpsuugnac.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gveyagtpy.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gheiojbxv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gwmceoheh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/guutgwheo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gebkkmkjk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gansybldy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gtvharpwp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gvasvzeaf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/goydcstbz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gndhfpptd.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gsenzfnqz.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gosysewaa.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gxwxlbbel.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ggngegnie.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gtgiqeggf.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gjepotueb.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/grnjqrjcg.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ggyegvwbd.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/geloeqivp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gugjxlwhu.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gtjyzxwii.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gysqtlchu.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gypofmjvq.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gwqacsaji.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gvgrkslyj.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gvlktovqy.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/ghxeeknct.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/glrtpbbmb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwlphponv.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/ggylnyueq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzxvtylvh.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gculedmox.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gbkfmdrqy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/grxsosnzb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtymexhde.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzeetlhzh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/glaremymk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gplaffwfs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gwlzizixi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/geewyibgd.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gfkkrusst.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gcfsfwupe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gvsexysvu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gythyvkfs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gpeqeexwo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/geuqpnmyz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gzjavzryl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gtnreeykh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gjibfeqej.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gtejbtiiz.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gqozsbcfr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gixyfokgw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gbjlbjolh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gdgzbrbvh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gxxorqrct.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gvuuhmafp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gkqzvimrb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gceboquof.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/guunteiku.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gpcvjwtri.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gkdohalnu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gctqhnzxr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gwryneibd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/givpgdqxb.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gyyimhkzi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gjtgfnpzc.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/glqbiagmj.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/guhkeungy.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gwqxwvwcb.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gewiubkrx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gqatjujaa.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/ggesljzri.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gvxguxrpj.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/geiyxiebj.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gwfkqazmn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gbrcurzte.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/ghbwxaapv.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gqvuxosrj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gciciwmca.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gzijhuzsi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gttnpevis.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gjbperxab.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gdaytlsrx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gsbyrwcak.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/grpctkdqo.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gvydmtdqm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gjbvtqyep.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggkxxjwlw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/giftyvjwi.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gvzcgtunl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/guntblccm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gifrtudrd.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gmpykrfxm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gkuqnjawf.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gvciftjya.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gkrtnksxh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gspwxfzlf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gfgsyqrsf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gbgeultpr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gsnprvgtv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/guricznms.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/ghchhxymd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gkzycuysd.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gwnqjgpbn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/ghrmviddm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gqkzsdjuk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gnsoxatwo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gaxvjyqmn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gjptrooxp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/ghnffipee.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/glrrtiqql.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvyfvpmet.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gwvbgbovd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gvjwlxaqg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gslxbfrst.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gjbmmqbbp.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gwqslyipv.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/ghkxhbguk.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gmdpwaqce.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/ghvgclerh.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gxybennul.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gbrpeworq.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gmwqcmzou.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gjhxirszn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gzvffzrrj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gubhsanpm.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gillumbiz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gyuriwzsz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/govfuzjzl.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbpteui.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gzszsihfh.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gsqzfzayl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gpobdhhcs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gjweibcbh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/giwybphee.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gpzedubis.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gtqgxglsj.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gtldsrmcv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gzdxrokyl.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gcggnbqza.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gwjmwhpaj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/geckqevto.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gyqtwbbqw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gbfddyaki.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/goowkciqp.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gntecfzwn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gktoazrvv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gfqqoqmkg.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gkgulrnsm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/glvsvmkuq.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gpmiwnsko.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/grisyfzue.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gklvlzssx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gnvrxlpqn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gnuozxuih.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gzbitradr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gzijprdao.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/grbieqrif.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/glnezdosl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gievmvppt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gyneboobj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvwwkgxbz.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gnwemuzcn.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/ggkaezrpe.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gtzyvhqao.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gkaxlgwig.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/glgebassa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gpdvkdjig.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gdewsyjfc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gqulheyrp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gbmcheoxl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gbgdjwzsv.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gcobskxru.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gnmoawrft.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gkiddjlhb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glpnzpznr.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gevkhefqo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gflnhfnsh.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gwfdwwjky.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gxewwzdgs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gblejlcly.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gbqjtwtbd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gbjtomwvf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/ghiajpmew.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gnpokqcys.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gjczzwiwt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gvvcssgzp.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/goybzhymd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gezxrweyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gvcxwhbmi.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/geiecwqqc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghuwifqeu.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/grkkuwbjt.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gorhcujft.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gphauwmgo.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/ggworqvpv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gqtwxlkce.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbwbtqoub.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gaouhokpc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gtfrqdhjg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/ghmycokaa.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gubdocfhy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gbgjdlsdo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gwjbajouy.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwxykmwqo.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gmnbflyja.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/grwjffkey.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/goyrpfvfe.sHtML


<!-- 参考信息 -->