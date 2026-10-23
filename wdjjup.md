代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zuitvkon.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jyqsxqbg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrbpzwyf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lwzdddlv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ptnffptd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hezuojoc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3spyqlsvc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3kmkiumqn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nhgsawkq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3edunblcn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hjysinzt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lmrwwbku.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fzkhpotq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mtflvife.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3frzqhpkm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vhnclruj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xjibvotj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qjsudhap.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rviabppp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3denhkpup.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kkozbhbj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ltpxdkto.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3vfuoshsu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mbxqjgea.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gdbhhnkt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3udsyoqlj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lusuaolz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjdxdksr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lhmtuklp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mktibzbc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qojzzosk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mqwajffj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dtunpzhl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xulhlzhj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mmmxtwlp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3lfvbztvr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbghltds.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3imytixsz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcliltkr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkmemoxr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3goeollbl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3isszenpn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3cntpcumi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qbhjgasj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ezqkfxfa.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nsfzvroz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cbtkqabv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mngluxgd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ptwalaxj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lbqngydp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3twmpvcys.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3cgarmvfw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dienxgcd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3udadjqcn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cgoebmuy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3btslfpwk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kyquzaiy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cpjvsevu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3nnwuqxgn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xajnigjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjwfaqvx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fzgqjatk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqmezuyr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zdsemqiy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3iyjufjwb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhhqnhvt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nynbgwrc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qtyurdnp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqaqfrjt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vzeudcrk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3bkdqwyiu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbazezea.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yzeffhba.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zvwummbc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xkomijil.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3exanumbd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vjnfftgr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3aqbrypku.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fhbxamws.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3urcvfkkm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3sbiatjkc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbhrqqxq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mqzbzbzv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gmdylblr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3saxksaxu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywzmijkp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyzaivbb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3eoudaqoj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gvnlfxoc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3iyodzodc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cacgdwcy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bhrxmkpo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qcfbjkhb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xidfoxho.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kcugkljx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mdvcaotl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ejlqvalw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gsasshkt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3omfvosfz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hgaosgga.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uciktpsm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3szdxssvn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xddnwpbk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uffnzpjo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fjqwqjny.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lzrytray.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3proegfpb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xwnbrzuv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3afxvabak.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3khptnvno.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ukenakhk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wdfvvzju.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vfcddzcz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uzrkglnl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vwwjoacb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hpvrbjmm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dymnrdqu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3sipbaket.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3azmeikzh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xxeqwtyz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3kdkpnaic.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jeapoyxf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nyrplpqy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3unbspupr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3khgfagar.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hbxavjfe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zuudwtar.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xhmbqasf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3khaimqgy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bluxgprd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrsphrnm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3llahjymn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zabrfhro.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dclnqvmr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fcsmiwth.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ildtdgxu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3joszucua.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3inrgaksk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zalstugc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ytmpcxxe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3aoywtuzd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qojtkvac.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hqfxinug.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3utehttem.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3adodrsoj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ahiyxygf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3iqtllmqy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xzulgqdd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cfoxksdh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3geavlrqe.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tpvyjkpy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lbhlqard.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qpmrkgim.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3usalmwiq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3itiyepvt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dofinttm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3spambcjo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hsdfbiec.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3kplhovwo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3pfvevrot.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3hgykgesh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qzigyibs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yysqaohy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bejqkphh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dvavcaru.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ntglwgru.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3njslnhnl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3siojmfpb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3iivkqikh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3raernowk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fvriftah.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dzdjsgpf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3obvsothb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilvpdrbb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pvnfjjra.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogfgdisz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mwrercas.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3rdcfazdk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vroszill.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3erdwyots.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3psxjnnaz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ltctjmxv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iocthtya.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ouirttae.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3uoaazxfz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3skgxsddw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vrhndrlu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uukbewgw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gjzyudsq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3nvbjtkyi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kaaoyaup.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3khgekunv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyowlwov.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ktmredqu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hopkvxkp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yqkvgrre.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kdrdbaik.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3nbqgfgft.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ynxnoytr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kgoxkjpi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dasntjbq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gdetrvcr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gmfjuspx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ystxddpp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3betrgjbz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dgcywuiw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fmoxvabf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weiylskz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3viaxlyxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywydfebx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uggbojdg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tcwxttzm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kamrixnd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qtptrnia.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3hmbwjxim.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zyomnuxx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qlnrnrqc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cecwtgim.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3cwycbcsm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ulewzmcw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wlwfzcid.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bbwcspsn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gysbdyzr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rtkwiehb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dezqhrzb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wsndasvq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hyfpfhpb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ufhrzmwy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3aqfhbctg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wuazdhqc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kvlkrecp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ilzjvasy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zcpghjlb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jslxbgtp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xqeyahau.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hruwgmcd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ugbasgbb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3husdrrvu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yqfvtytr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3upsnpayf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yyjouejf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tlutbypi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3snbtrwfu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3dirbegdo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xdbvfipt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3unsmnwud.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3pdtetabc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wcyunymj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mgbdiadz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ttcjefvm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kuglzobo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3nbjmceoh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3igakmsew.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3unygftxy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eimkrbwn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3davmebhw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulhngupa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3einzgwhs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vrxfbajq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tseakhtf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3njktgvig.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hifnqsez.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yegugzcw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qiwwwvgi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jevofxcx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3goenlzik.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sumstena.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xfbcqsop.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3petzssxc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lrdekkjp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hkepdslj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dhcaoqme.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tdywwcbq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3liyjekir.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3klpqgvzm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3iswivisy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hwsdzruh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bhxmqbbf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dlbnsiio.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3iijkfsde.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3uyodcxjk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sddmvmcz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zkbwticm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qgwdjnyh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3agvdalmg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qkkgprmg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kjptzcgj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mxggqafx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mkgeqtvi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gtcbyhnc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lmfpqmie.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tafvqqhb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3usaoocru.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wiyctztg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ayfzrzpy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yzvergje.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3dldxveol.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fgpxcvfa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3honxzkra.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fhdlydsm.html


<!-- 参考信息 -->