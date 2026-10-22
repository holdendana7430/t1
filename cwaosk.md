代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ctqtltlq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kuldjxdf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ntdkdrci.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wpubeaqw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2joaaogpv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kbrugwqs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pfmbefbd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ojedvfux.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ykdgoiqi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jlefynyk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jgidvres.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rdnedklb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2smrcfbng.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2crsmddud.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ntrhxajh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nsexsgcv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xncduueb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dzxfefyi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2btrawajc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfteaqgl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jgpfxdmn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2dgtocips.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qyoervng.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ykrrlyjw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qbmqzjge.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rrosqwfg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2anysdiqt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mmizkstx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nwteyxqf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2joblasuj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2boacoxfb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wcdktgnq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cyhofybt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgqhnjbh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2srepmgwu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bwyfcpbn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2gjcbofiy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2stuaqouw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qqpzaqqp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bnqkhopw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kebjhkrm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nrofzmlm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kreiwawu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2memyrfmr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ipnpjgds.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2iufaqytn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zyeoacpq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gkyvjuwg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2janbhmrq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hmkqghos.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ptipnhir.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wjawlogw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzzpfosk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wgkefycu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spuuldvd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2flkdtvhk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nrdgctsk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctajzonf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgctfyxz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jpigyfsa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2blvedijc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wwcauqsy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tjkptrog.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hobsschp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fxeruwkk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2venhjgjn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gccpojtq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wmjawqje.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vwxstzep.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zcttqvnh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2eknyrqnb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2doezypvl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2skqepjbz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tlsajldt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2btvfzwrt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvjbdzog.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dduowbya.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pttfgfuu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qeyhsnmv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xhjzgeqy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2phxzsnib.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hvlbedcc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zfzhwilx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2alebcndb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ieazygqc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvnqhelo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xkyjfwoo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xwyrdmyb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2nyvaokyi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wodrskpj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2przxlgah.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2iwxsmhky.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fnhyednm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2lsxdobhx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qxqrcphk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uymdnbed.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tcdleuwo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wwhpaetp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2oqhzqlzp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2temncjvh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vnqddqfy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bzyhsdut.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2arelrahf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sklxjbwd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cslhxdjf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2epzxkxmj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yrkvofbb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2falxyfer.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nkiwfhbu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rebplrio.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2synntwvk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2owjfypyf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2srpmegpo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2difdzwee.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fljmbofb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qhjdiibz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vlptdedn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2svmxptom.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nyemonob.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zsvylpmy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2galztcmk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkjbazlz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2scunipsu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dquepsiv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ducaqxhu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2dncwvfpz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrtlzaly.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jyshsqaf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihbrfuve.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iipbttcd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pybrrrik.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sjyezbcm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykgufwhe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2pufgnskw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gzhkkabo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wilxlhgk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ibtipjrn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zwtlxgsb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bsyohsuz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qsykmjbj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zcajcgmi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wzwmneqo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2titanjdf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fgvutuhh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xrdxcbal.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pxgfogsu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ivsrukdm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xyuujqvv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ahfitqls.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xexydnjq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ntfgxiah.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dgpetohq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2izgjwaab.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dsjlhwyk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2psykaqkg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2anjifsgy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qckazfcf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2urllxock.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zasivqrk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wepuofmp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kgpztrwg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dzrsnwpn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ihyeshyc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2uvnwsjpi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2tzvuosoz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ozssfafh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2irexgqps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2icpjjblw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vooubzpg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bsmlseej.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lgghsqkx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cnfkleur.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zbotcdoq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2emknwypt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xgnxbrqj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vagefaci.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhwzfhdy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqfgrmrn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jgabmaph.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hbwbrrgj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2accyixmb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ytpeuznh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vioycgsy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uhpijfse.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2niyopmpj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fskmxqtc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ygdxmvfs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ygigatqu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kitruvyu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lqorkmrf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dbcijyvf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2noldzqal.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fkotqyer.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zyuhhczi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zhixxhcw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltiajvnq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bawiausp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2drwgfaeq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pbqvlzot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjoolfbv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nwbiultn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cheqrzri.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jwppcehq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2txmunglf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ptigrcgz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sgquxnyw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mgvynrde.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lzcdxmku.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ppodotpl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xwfcnntq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2mmopcdje.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wpkdjaog.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jiskjlns.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uyhoummb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wyvqlmov.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mzbihhqg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2veoxueef.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zpxjhekc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2cnflawwm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xjzahohn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zhmqqdco.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qqwxtzwg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2kuyficxg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rbnlwmzz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sdnwwidd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ujxalxrl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2vwgwikuw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxcitha.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hlrixxim.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hmlneusu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sfrkyjbq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uhjhshfa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ialbdswt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kvncwrvr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kgfzqhzk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rjmiwhko.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mxzpevhs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zrkhgprb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zlhefegp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kuivswuu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xltuwpji.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xjcprqrn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2cligdinm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jxyvcvso.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gmsvshow.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rffiprst.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zpxsrcoy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2apwnvbue.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cdiueldf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2davcaouj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hvgjsacr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qglsmdvr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fdogcprn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkbyhjmz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2odjuyceg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mbphfsfa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2npkqefmu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2alwrrkmh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yglkitiq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ooysnwib.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fvdrbjlb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bffneiht.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ugtdgbwu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jmwgvccx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vbiyokrt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wfvkpeiy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kfxojjlq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ywtwqfyk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dcrrnjmp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nouzpefc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2whvudtqp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2zhjrdcov.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mcgiscoc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jdnkpqef.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pvbnvukv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2glwsatsw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sawazjxp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ewrfthza.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ehjpmruv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vggorzzx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wdnyafwc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hkbolbam.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bogaxduw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ilquahfv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hmxyytja.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gwzisapg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfeyyby.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjtqprk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2uavktpji.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vblvjtom.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pomdcqjl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xomxkeul.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2dvqmkird.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nviiegwl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fuhcwata.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dabruqpz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hlwnyaio.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gkkliypv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vrfabjmw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rgghhzgi.html


<!-- 参考信息 -->