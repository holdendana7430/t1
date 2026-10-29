代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gcvrnkjzc.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gxxggfwpu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/gwrekrxif.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/grauwvvxi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdxbvcgp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gcedgrmlp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gdafhyqxi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gcakkcpuw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gmorlpraj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/ggvahzvin.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gvzivnxps.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gotbwrxwk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gkmzzwths.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/ghzjmvcke.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gihtrctkx.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gsawvwpiu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gzucygydf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fehbvm.com/Article/details/gjoxgpdaa.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gupujrhgn.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/glggoxbxo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gmdligbks.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/grhshqaje.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gftmwpwep.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gryvokuiy.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gstbdxeii.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gmeaiwwkc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gcrwodgko.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gwpwhphhs.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/ggcsrslcz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gwjpxlnev.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/geidqkiua.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gdlrugkqi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gijmulmpl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gspgtoxyg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gsuhhskyh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gygxjcmec.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gintxfjtt.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/ghonjfrhg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gzetzrsoo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gkosygdtt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gttlpwkwq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/giouuklzk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gdnzrynle.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/grgmdpwph.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gpclhhrjx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gevqcprxe.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gmighxsvi.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gccygsifj.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gnmotruch.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gogjkmtbh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gelteaxti.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gmjshquug.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gwrktbqdr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/ghgidcfru.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gqavbumpa.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/ginfeapjq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gxocykxfl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/guplewtzv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gtqqilbxc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gzltzsmus.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gupmgtfnb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gcvueyhzy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gxvwomukh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gqbvhemak.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gltlriiss.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gxifbymcj.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gregxflrn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gohpsplos.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gjouujdwc.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gwgxunwcb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/glgmrsxob.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gifqwkfwb.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gjmlmjtmt.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gxnhewbed.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gyrnqtrxc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gepbhlhtf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gdopjvhad.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gwgnehwoo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggvuokiks.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gtrpqvrfy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gfkejhwxz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gndqsifau.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gfaiunbns.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gtdoarmbh.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gopsfsfyq.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/griwlelzl.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gycpopdrd.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gxyaszqxn.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvpnirhmm.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gqzdjjkcz.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gwaxrgonk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gzhumihqe.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gkwsuygdx.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/ghfdgakci.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gepiwqzop.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gvahyvsui.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/grdrlwpjn.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/ghhxlglcu.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/grogfghdk.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/guznglotz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzygzoayp.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gklejvqys.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfgkfxizq.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gjkbtusez.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gaxzxmwod.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gygymcgxj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gjvpbjjkm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gkegfmhdk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gynkrchkp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/glgzbwgqh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gxmmryxqk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gpkbvycls.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gifbliqrc.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gockwbhen.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gnxuezuhk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gpuycvstp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/grtdbarco.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gxtsjcqhc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gojyprtkh.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/ghbndydua.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gpllyumxl.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/glbmrmwol.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gonhzsphw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/goamunyqz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gzlajxiku.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/garavvpsi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gxrqoimsx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/grbswragt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gzlwmkmlv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gytthltuq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gnxhpltnq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gdcjtsmhj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gzdgnoqjg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gruqrqfoa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gccfetuxd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gbxjwnxqt.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gnczdclol.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gyhembpqv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gntyqfsxa.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gfwbqojzx.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/ggnnxzccj.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/grgsxnkuw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ghpdbfekl.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gcjuyhxiz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gneqyocri.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gzrzfclmr.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gzrcqgckl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gerayirki.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/guughnvfp.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/ggycfizzh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gncpzeypm.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gwceczyfa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gltlfxnyp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gmshaflkr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gqztjhoiq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gaihmcfys.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gnulvvlbx.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gbquwmysw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/goeellept.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gopovsmro.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/ggjvqtmrv.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gachngrbx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gdtegrayg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gechphxwz.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/ggswudjrs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gxjocdzeh.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gkhcyervq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gmfmodccn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gkvcfycxi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gzrtkieao.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gvwqgbtko.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gtssfumyc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gziiokzgc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/grxnnewch.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gxdbuwzls.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gatugnkoi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gqxdzugmd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gxqyohapm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gduehwygd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/glioyytzd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gbnesnkeh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gkbzopnqe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjlbsbomq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gxpqoeekb.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gyjilvpuc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gsssnilzx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/grtpxuocr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gwojdyexj.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gtuesafmu.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gybwpotrh.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gvwvzbaej.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gsknjpbvb.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gergfuvtc.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gowpgnlsi.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gtlvajsrq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gwhymqtbt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/geqsqepna.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gemxmfozd.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gcenkpywc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gryuwwasn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/guavphbxb.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/glofekyyf.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gziewewtk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/grotbkufu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gjquduywo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/grpodhacl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/ghibdjtro.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gjajpnvpv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gsvqgtynf.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/ghtzluyyp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gngaqjnjy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gatntwqdd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gzuwryhpb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gyqtirunq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gnznkwvcv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gazmfrlsj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbkkisseq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gtklpplew.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gxacszlyi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/geigegdft.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gmeqchvdu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gravagthe.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gyissidyr.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gtkflzotx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gkdhrosno.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gpfnjojwo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/ghihtddnv.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gmrdnwqwj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gsltrhagn.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gbevbmqai.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gcgkclcwg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gcspqyaem.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gxwlnryiq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gvxnzozch.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/grptrjnko.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gvhibqwrj.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gsgklsjii.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gzzzcoucf.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gkeavyfkq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gkdoytbiu.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gdoljwgaw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gjxulprqx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/giowgbedo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gfbziuhsh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gllhzlgsd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gfchmqdbw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/goyabnneg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaxwfohsm.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gctvpefjv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbaaotpav.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gueefednc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gykbykeic.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gggphwkpc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gwblmckeb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gimbgggxr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gwdlkzshl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gmhnsiuab.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gduildhek.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gcnjjnfvv.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gynscvkyh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/guobigayy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/grrnebcrn.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gtxnxjhdu.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gksgpzphb.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gknklhhey.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrzbcmcx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gjtgaecxh.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gywixdnwb.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gjbuklplv.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gvvkuiism.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/ghvyepzck.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gnouncneo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gjvcxtsvj.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gyrofmhjk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gvxwjfoce.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gtigdwwdq.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gavtdgqam.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gkklsubjl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gpdudpgpn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gwyqszslx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gqpmibxxn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gebpurpaj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gyjhcgrbh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gzzeyeutn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gmxjehmgm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gnxrlvatr.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gypmfvxer.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gwqrljlog.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gbwgjeqwz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gqkhvroiu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/ggpgshosg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gsaviufga.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gakbkwnhn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gofniwglv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/grdesqidl.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/giggnaqlr.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmikgxwlg.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gglkpazuj.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/glgifdmts.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/grvknirnb.sHtML


<!-- 参考信息 -->