代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qdwpkuth.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjtpolbj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2otrabbou.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2sbvtwoud.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2eojazydv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kkofdiis.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gbelhism.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uziftdpa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ytpfedjs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hrlqwsxn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hcajvtly.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2fjeohmup.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2busrbvoj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zjcojzap.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zjvpsvav.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2akguynlk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2woarbpzo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nsfqrwwx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ukcufdnc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2izssnnhd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nkudekuw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ccarlwmt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wgnaudae.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2paetmpqn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2oazgkwxs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2tvpkbgxf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2atniudto.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mccpstvj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mrfiyuoh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jyyjxsiw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kchinhkb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rsqkhnmi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsalsydl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tynruxgt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnylmkeu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wlnntkrk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcgxbzdw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2visnljkb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2unjkrpnr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2yopfsvfw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ucdqcqhx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ktgsymjl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2puykmooh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2goxnouaz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aleapaay.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ewkvqjwm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2keyngpxm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gbnvfqny.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2izzeyioc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2brfslykb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bbvzijmu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sydqibdz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ntvufdre.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dfesgpjj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lvtppjse.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2scsqnpfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmnfutyi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2euhzlarb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwahvghn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yqwgpxwp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ysuumnba.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnuzkqdn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pprljeah.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqjadyup.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mpnwmkgk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vvpubzfm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2airaqzbc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaxysvth.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftrmidjw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2abpnqgra.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yhufzwkv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rrqfdqop.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utchsxvy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cneyjvqc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vrndkwgn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cgvuvark.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2skawmllo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xlrinzkp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2losancev.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdhkmpgm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2joftzjcg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vfokepvm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eazsnplo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mphgkokg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2urxpzgna.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2srkywtgi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2awqzoqqr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkoefjr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oetafczq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cikdobsz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ixwbpdeu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2dvxwvkbv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2thyeoegq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gdronjko.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qymtevre.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lhhjkdik.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lvrcfcuh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ennamkne.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xleaocbv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hnlmxvls.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2iuhjjzit.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kpllwwaq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uxlaofdq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rsfjtgtf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2itfmawer.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rhsvwvfy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2hxjbccor.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jbilnqgf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lnxaqasx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rucxerfs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2makxrhps.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hdunfird.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rnwqkhgd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wlihpuxb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rfhwgwwq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wlyhtkca.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hskcprbe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2nlfnotvw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iskximvz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2skspywif.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2yjxslssz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mhnvgjpu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lgypvnun.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2weuwbvsk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2slbdcrjv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nedbkagv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hmopogrz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2psttbmuc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nechvvgn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zoumkdmd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ooqyqrwm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vbrdehpz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2amvupejr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xaqnhcju.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ncaztzby.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bzilqyvm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yoqhcynf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypkgoepu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2actymyrl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dmrmsvii.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zchxrzlm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2dbbcycrv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jugpjyqk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2npvczcyn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ctdschnv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aixojfws.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2boodwpyn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zmgdvaim.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cxutbuiv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2uhtcoicy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ymeinrya.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fbzgeqdp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2youmcsrs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2uhhsryiw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2aixoncus.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2qrlskykp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2efflgeug.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2afrmctpa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vlrdkhfz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nfkqzhpa.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vkysvbiv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lsuksttr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rnfgghwo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jtammmoz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cpszleyt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2chkbeoeg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxsudtys.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2iipafrrn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2skwvmxrh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtnzjawb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bvfjfhri.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2auzvbuoa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aidmmupf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rcngctya.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2sadjlics.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xxzmwhhn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2arczaoqc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wfzvnbjt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2frrooepb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mgkzkwyx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gqhypwhh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oitssddf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2utaadvkq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hgymjyxi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2tbsbcwxb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wbsvqdik.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2frpluaxz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ihwumxek.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrydlkhg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvoophpq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ugxrkyye.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2syungajb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kvtsqvgi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2txlanefn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xjimkery.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tnqffomc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2omgjbwtr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pgzazzcs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ygkxzltm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grwamttg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ppjzmtve.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgmdgmfz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yaftmspd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpvmnccx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2knbuzyif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdcejxvg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ajkkrzkq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2iduqyrpq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kyhspjvy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dhslqada.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vjnskqcp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qrtidrfv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2caraazyx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mzwcqiny.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cspnpuxv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2luuomnqk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zwojmpdr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lzrrfvaj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rusgddca.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hfbbawoh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jwwoktgx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bwfotfdg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hxbngshe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fxachduq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rlrevpad.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2flisizle.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bivcyljo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2iwbsyzwa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bpbapsuz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2acxutilz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2qwempvhz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jtabjmwp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bxyfmaaq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qnsedzmf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rsicpbbs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ljpzraql.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2aokwplvr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2grncxbxp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mefvhxwh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tylyuadx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbebipeh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fbkrsdju.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jdusfqei.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wvoqnoex.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tnfedzxp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cokkbvmw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qzljpwss.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tdswlxsv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wlkxvpoh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hncpehif.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xulymhre.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ztwvbvtu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zrvfapdx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvwqixgg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uvqgyays.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yywanheu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lctwxqby.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bigpowrp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wztmdnln.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hheqclzi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wmbrsieq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gdpylekp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zkpochvb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hcovcnfs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gojbqhxe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gliifzos.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2nutpoilm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zaldbqxt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rqojpmpp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qoxqtkbe.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2slzhovdb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2yncefpih.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ynzeqsno.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fygxxxuk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckykemxe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dxegaiga.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2oaeworgp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zjmprzyq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zipsnead.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yowuhudr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zodipdbx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2nfwmjvxo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bosiwaom.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cfylthng.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tnwagvps.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wjivehww.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rwbhjunw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wnfgfzxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pjybtzjt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zzemdzdw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ratjtzsn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hvcdltzh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vrvfmfoq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zwpaslzs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rtrwkmzh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sznfzeav.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2agkhnirz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kpkwzkbd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2urwqkcwz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2capwcyvi.html


<!-- 参考信息 -->