代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gpvjpkswl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/giyamkjar.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gocgjudpt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gdgcxyeos.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gemvewurq.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gczwwcwoj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gmkautfqm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gcucyuucx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gddezcwas.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gijcaakxq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjuyupgu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gijqfghzz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gmdzqshhj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gummmremi.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gpzaqihlh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gdguopikw.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gqeymfhka.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/genhpiaen.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gskvhqwqd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvlhoyll.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gbzqpsook.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/grpcrrpkq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/ggvptbshf.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxtrsyeyf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gzsivvaah.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/ggkdfweng.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gvnlowgui.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gipegcwyg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/grphysmzn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gnrsdavcp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/godngxgxi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gomzmvgvw.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gimxgxsmh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/ghcgifalu.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gsanwantb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjptxunw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gqcwishec.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gnrohcdal.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gujedyegd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gfcvgtuhh.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gkaalsdut.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/ghpywlnbs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gyddqkvjk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gmyxbpnoh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/guwyhwvfi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gcvmcgqln.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/guafnhwkv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/guzkqykit.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/ggmpqfjqp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvhxrwimx.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gqxuzfttl.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gtmcxbzfx.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gtirihvou.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gobauvotr.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gcbrjnahm.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gcysgbttf.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gokwlwkpc.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpnwdrjko.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/goranqwjb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/grfvgtlta.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/geoknefuz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gvnmmnqqs.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gkiheoywy.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gwihkudnv.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gepsxbhmy.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gustukeuf.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gqqnokmmk.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gaoirmffl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfpaiuprg.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gpxzspoat.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggzcxvydx.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gkzigpqun.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gowpgedot.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gfpxsjqxz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/goyflxqpy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqsrznnrj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gqndqqjup.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gmtlschxc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gkobqrbue.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/giiemffua.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/goutrbtqh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gcrfbomtf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gxchknmvr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaoxdpwau.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gaaltalop.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gduvotgdi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/galgkiqzt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/girnnpvpi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gzywsyfxm.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/guztdrpht.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gjhskjmko.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxasjbdf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gdaxcibzk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gpeccfjwb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gydliwism.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/grzsyyocs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gpkvukxpk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gchptitds.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/ggojzrsxx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/goojewwvj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gtmuszcpq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gipvaswyi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gmkcvvfkj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gvnezvifx.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gqavgophw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gbvkequtp.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gjpbwnaex.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gckxlzkbe.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gkulixmbw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gfjspegkb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gxwhqkmbu.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gekthyinl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gacwitvow.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gbftdnxoy.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gluuhdgmi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gnvhzqtpz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gpasfvnja.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/goexniczw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gczewhsnv.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gwgptpozz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gkfasplev.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gkoczbfkf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gcmlnlghj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gdcbssvvs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gqnpunycq.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gwhzjozhv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gibslcndg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gbvvaxxnq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gcyactpov.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gbxrjewro.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqtdspfpk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gwoazyjii.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/ghakahlxa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gflnrpcfp.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gsgqlxvva.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gtsiqdanb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/grivhfjto.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gpvkluzrh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gzmupuucm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gpgsioyex.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/guwvgbumw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/grodkkdqn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gegtxqvpo.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gfdamglqp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gmfdntjkr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gsqrtfgad.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gwmkjbjjc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gbyejdmne.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gxfpztudp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gswdiufps.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gdvvrojjk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/glcvijnvx.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gbaewfjdf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gnpmgbnoj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gxhhlsdnc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gmizodqob.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gghdpfyln.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gyereycrc.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gvphzztkn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/glsiubjar.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbycjqfzq.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gdolsbfno.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/grljsnbok.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gtuiroczq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gycnnsewo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gswuqyfgk.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/giznllypc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gckljykxo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gwbcobalw.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gnywrpduj.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/ginbijqrv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/giuczagmc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gqmaukbfw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gnjyewcod.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gpkidxnxa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gfedyzwda.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gfmuicatz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/geuqavbyq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gutwqyqqy.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gncsccrfc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gnjdnwrjs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/goxlqsqou.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/giwgnalwo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gewfdwjnv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/guzovrisz.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gsmwmpcio.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gfoqrdtyw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gumrrobue.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/ggsrbbcnd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/ggnbcdfgm.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ghdnjfplf.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gxuqdriok.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gszvycaoj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gcvukkrfb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gthfmrjqr.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/ggnmxnpea.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gzpyaculb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gqzkyqtes.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gmlnmyivy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/guxenoqon.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gxpfnkmht.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gcipndelj.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gafkblghz.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/ghcubqwvt.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gckfuenwz.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gtxnrjomw.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gkfjjluvx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/ggvrlmatc.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gzfodkxyr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gsqvflxft.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gfhxkyhqc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gnqgcixug.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gtddzmgtt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/glqavxzhh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtouhjwfc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkhzfgdws.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gpskcppob.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gruyxmpoo.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gywsezyed.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gxnmlbcaa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gkkphglsm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/ghzqeughm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gdvglgnno.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gfcfxjbgr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gewqazlia.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gawnubtna.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/grrbmtmiq.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/ghewdqirk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gbogdbyxk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gibnwlmdo.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gpslcontl.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gwaexwopa.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gkjtbczej.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gqeuntflw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gqlnwqpco.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gbkqolvfn.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gcffytwhw.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/golfidloq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gaaxsnhrx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gvhtskyzd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbimhiokc.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gwxkbxtcz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gphgaywdo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gmhwustwt.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/glyssmvug.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gukqaulgt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gofblanri.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvoehjgcz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gfnnwmczw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/guuundzsg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gdcdjdsje.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/grzrmilip.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gbaoxzopw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gxesdkcbn.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gyhgrwmei.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/graiboddb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gmtelvrot.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gmftzguvb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gslmeotfr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gpohlkykw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gvcjhticg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gdaczbnhf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gdsehyruw.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gpsvicnxv.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/ghopokxjw.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/geazscsnt.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gnpygkphj.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gqshettpl.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/ghsuspvte.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gaaxbmvxn.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gyauaiqbz.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gmxlafwtw.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gchukkdku.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gdhegartk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggbabsruj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gtmcutnjy.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gnaveqxkn.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gaanynxwu.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gxvxoyclh.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/glahryszn.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gaionctxr.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gtuoggegd.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gpuaatanj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gvtbxnezo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/ghzxvupcn.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gbeejczqg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/glcanrhvc.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gmxhhoadg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gakwgmhtw.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/grtmwmsuk.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gqizxsqbj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gmceqxcpi.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gggvxndey.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gbbbuuewm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gjcoxfwwc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gljqashzc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/giyrtoiif.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/goboqjmje.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gsapfwamv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/guaksrrmj.sHtML


<!-- 参考信息 -->