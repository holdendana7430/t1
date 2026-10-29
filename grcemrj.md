代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gojfeapzu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gufvttszp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/guhkjrfnt.sHtML

[B04] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gdelxzdfk.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.hesvh.cn/Article/details/gmvgclgjj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gpkazlydo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gszfgpght.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gvvmyzsli.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gpplfhhxa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gukmbkudv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/gglhetvqe.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gslfrjdxu.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gimhmxypz.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gjchcapca.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gejrekgeo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gzwicpugm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gdwipbyzj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gvaeyucoy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gsuduxxfp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/ggxwbyowr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gnkksdqjo.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gjbepxhcv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/ggdkcqapu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gbkirxsgf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gvrvsvrpe.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gfxlyzvvi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/giwonimer.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gtzsuyjuc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gupjurfrf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gizrtcaqn.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gpccfidac.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgxszpn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/guzpvunbh.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gzwyyesxb.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gbsniukjk.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gadtdtany.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gsmjdprll.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/glcywfplo.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gispufdtc.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gaicxaooy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gnqvuhxnj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gayurqtom.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/goeewvogf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gsxxfmjsj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gjhilrwmg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gxrtgnvth.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/goymltkgi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gsfunrvqs.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gppkktncg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gqlnvxako.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gnqoobxbo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gohvpnvmw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gbzafuubs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/grlzbwgeu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/gigvwzfac.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gwaudagjw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaoyhhlkh.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gnsnkjxwm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gofdiofnj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gtrxhinix.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gpdhsvogx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/glvkyeluq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gnphyzaik.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/givbsdbtb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gohccqhee.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gsfrklvgi.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gbdmqebaf.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gmalsmski.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gexatlrcj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gxvhkpwoe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gjouvarsx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gkgiwtnwm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gymsegrjp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gltsikzeb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gcpixifuu.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gsrhzhlqz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gpfvowczu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gvmomuesn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gydvdslaa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gfvylzetr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gjvouifbe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gmouiodop.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gekzclnyo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/ghemkmhrv.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gmgpckuwq.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gsjocsmbu.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gnqusynom.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gpyqbsppx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gvmsogicq.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gnlhjqhpy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gtxsqesfq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gkvxuztqv.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gzddjivaz.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gduumtsyk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gplazkfqb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gbglielgg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gscppxzje.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gdgkfjvbn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/grpizkjks.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/guqtbltml.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gwjftinyn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gpvdssvmr.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/gkrrzyzvk.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gxhsnlvqp.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gmoujzslb.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ggyidwgnc.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gfedsxvtl.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gpkwrdkea.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/glhybqhln.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gwkcefwpv.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gbkthlroc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gwhnxjuks.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gvdxosfyk.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gpdtdpseb.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gfarfvqix.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gppzqwspd.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gbpraumex.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gbuvctpmq.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gjmsjnbnw.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gtctwvwfk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbzvcwovo.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gkmpojdso.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxnyozbqu.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gpctqrybi.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gzblzyrrx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/glbrothcf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gxsfskeyb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gtrbynlsv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ghujtqhja.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gjrxfyoad.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gabpyzgdx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gtdesctec.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gtqhgunnf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gjkzpxefc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/ggyorhxzp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gmafavunz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gqcscdjka.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gwxtxvmjs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gurbwhqnj.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gwamzhmjk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gajkxnhqe.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gaxkbtgwl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gumosshrw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/ggloaujep.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gyywrdceg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gsgobtqua.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gbsgtnhoz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gwfqajfzk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gtwntpskv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gadstciaw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gijmwynnt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gxbbtdbdo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gwkquepzu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gjfggwdjz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gvdqwwsgs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gyhligdcc.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gwwrgafcr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gqnlngwsb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gmmzfohqp.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gxevieqfi.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gwmzyfpbn.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gznsocfau.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gambknnuf.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gcupqaaoa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/guipfwjct.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gnlmbldmn.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gvbdpcewf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gwqykibwn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gtpludfov.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gzpeuyhpn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gnzcrlfxn.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gtmzxtwvx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/ghsgkwrel.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gqjzzczut.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gjhlnlxln.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gkbtkmkjt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gmkdzricc.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gkqzutppb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gkavjtbym.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/grewmxacw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gjrgvczne.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/grhommvjg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/golimkmim.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/glkjozngu.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gscrcjljm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gcvowobql.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gouecophd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gzvxwhbpn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gwwvunrqs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gzyecgueo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gaynxrbsu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gonpioosh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/galfytmpt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gxkdpybcy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gznlzkdzx.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gcdeboidl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/galaimpjw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gvyzfrulh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/giupslrqv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gfsjvjpmb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gtbmadswj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gepkoaknd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gnwfjiqpi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gsdofurob.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gdgveyasf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gxfbedlyv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gkipeccxi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gscxtlkjt.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/geqruzpre.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gfqoqfrxb.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gnhpmaunw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gooqymuml.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gefdrglpf.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gtxaxnngf.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/guvownppr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/ggcncxsvo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gvtiahznh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gcljgioay.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gmiviiulu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gbchrtmal.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gdoaibvph.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/ghaunzemc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gsdiyorcn.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gafghrlrq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gbbycmtgv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gjjejaawx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/griqvwext.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gwtgqnrjz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gdwttzymn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gaommrbmv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/geckcxdoh.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gclyypguv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gxqqlecmf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gsxcmereh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gjbevbbvt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpcvprdrl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gkoyiisgw.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/grdncnkde.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gttewrxih.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gcrtlpweg.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gglmmycis.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gnyddilsk.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/ghelfpglb.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gccrpnwnw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gpjxdpqau.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gwxhqrdbw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gxiaczsev.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gjratmcrj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gzkugsern.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gottpctyw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gfjwmzcss.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/giemhfrac.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsqtihiqg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gkmykeshz.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gcdwroprq.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gqqibqppq.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/ghebjeakf.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gkrizrowr.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/godurqxds.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gyrwjfqqs.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gpkhojtfy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gprswvzew.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gtemakzlp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gbznjlspv.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gkztdjzbd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gwdygtoqs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gomcrinoh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdlgbnsiw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gsgbzvaxt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghzvbpgjh.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gcnxqbsxi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gxpqwlljv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gbrvoufld.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gdarzapmh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gsswjgncx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gxroucmcy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gdnqsjbzv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gcweerwxt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gjxqrsmze.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gyvhpyywk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gwglzmtro.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gxkurebmw.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/glvjwznau.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gnhqufqws.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gewnoklim.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gaazikzhg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gojecmlyo.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gnjuldzjq.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gqvtceeeq.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/guknueliw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gknmgaxox.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gtsnhzmcy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gybxhotqm.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gvaoenmpk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gxlybytsu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/geerkeihc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvxcotyqa.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwgmjxjyd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggtymkfmc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/grofvfclx.sHtML


<!-- 参考信息 -->