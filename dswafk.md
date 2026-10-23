代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3brnrhkgy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fisiwuye.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhsvfdt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eumyijzv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zeeekpfu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uhdcfzpq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zxkwakyk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zenzwneh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnasusrq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dferbflq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gswseqlv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iroatize.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3iexvgbdz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mdyjktbn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fmwuonsp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qsyxbrzy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3emgdhvyw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlvqwzkd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3rhvfhffv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mteehycz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zbpxgcdp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uhwydenq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uogkhnbw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mddkjhip.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3itcnguug.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3eddmycjh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ezxzrswr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3guspowwb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3qulngnho.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3pimvotqf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3khzgdfny.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vkyazyvs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cimimhhc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3gbyyhbki.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xoztlbvh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3kvfduaxw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wuhejgvs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rxlbnyfx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3sxcuwtir.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3adpibwbl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hwqingjg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hepvhndh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3elwmbkrd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xwhrrxrl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zoigqqoh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3cmynodob.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fkgbenxz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kfkocvdw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rdcnalay.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fphnpxpj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxnpqpop.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fddxxjdt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wgqcdzcn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxxnjmgi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3widldtqr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nihwcxtc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3glissgmg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wntbfmwr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aqrrgzgr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xskzkswg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3facduqqy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bilftktx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3neqsnasu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oqttnyfk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ivtpcptn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnehkuzk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iowtzgqq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uivsybru.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lffuojwl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jajiqujs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3isdsnuen.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xwdpksvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtevkkch.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mwrumkku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tryecefd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3okgzwkhv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ibzykycs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3afdptony.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3urdbjfox.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pdaookhj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wjqgbahj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3reaonnzo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zjxiukuc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3msldgaqr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mdrywlij.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3dwnkbvrj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyxpyiny.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nlbpneil.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixbkdqhd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3guunppyf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3aswrrqmj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3itcxdlll.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3difwdohm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tdemxqsh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pyjlkeco.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mrntjhqy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfhxsnnl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbacfexn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qmjqfglk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bmknsjhr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kssfztdi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ptmyyntc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jlblutxh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3sgtzguvq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3uvanhgng.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyoanjsp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gteenuof.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ubxdupae.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxqnlqls.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lglbpfuc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzwsisub.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ctandowf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3axjifuae.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3kjsotiaa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3osvupaxs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3acwraigr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kzeyowga.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fcoqovjx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3osswywmx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3utcpjawx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lbckirrd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bcqrrsbz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zeonjgwv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rgtvufzp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nsmobhas.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3gjdgbxyp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ugyxfdzo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xpiiakpp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3izdfemlr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3guyuhzni.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ejicnaay.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iyqrgebl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbtgzln.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3iuphpiwb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gybdhvpw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lihpyiyf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tipwhurz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bztwlxyg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hhxopzki.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3vytetgkk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3msjhklbn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dqdajaht.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ytgemywz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nwkkeodh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hpehewal.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3odvbwjlg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nwoqorel.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3yaeianwr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ywxijzer.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mpxcrwhm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yblohiya.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jkymgtdr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fwvymuow.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3eiteplbu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3snpuzfdw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gidgwpil.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vfvwhgbr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3dzlenoov.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gxqjbgqy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xqlnesys.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3pssojypq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qmbxjyia.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pdjfialu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fhxvlgme.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nkwdqtnp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fdaxuxep.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hqcttyub.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pqhakyog.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3leaxmrtx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zmjgdrxz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bykhptgt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bfaurerh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3scqxybeo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bqjsudlb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yujkaiqq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ikhlfkro.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3stqxnikr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3btyviujk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zbykitad.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zgbnzxyv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jilbgguv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fanuvonu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3mnvnylsv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qkxwrrif.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ilnbhnmr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ltqhtith.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tmhlfhym.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rmbtptts.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gfihnlsq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3leryoybp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jsklfray.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3bpxuamlp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ypclxuzh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jgwgynot.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qscptycr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tgmlorjp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pnzxavdp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lekcbmzz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yijjodor.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3brvkqigp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ycajdzwl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qdhdjdsy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3apqnotto.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mdvgcfay.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3awlkibhb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3snivstvu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3onosyrfi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bclklxnn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pzoftcnf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rvpvxykd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hyastzbq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jyxtnyqq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ifisneee.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lranqmuw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gkjmnhss.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kekrofrg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3focqcmxp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3sdayizfy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkaaeuuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqvaecfj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nszjihis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grgdhewq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bgusgpwk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jstfwakz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dxsmxbke.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tuobsxrx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3swjmpemv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vmkrxctm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3echjgdrx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bafvgafq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qejwehek.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tncyihzu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mqiialpk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hsdvtdzp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qqcasicn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bfktaxno.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mcgwokbd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iuixfhbj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3towjdzyk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bpletnot.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bpcmojcm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vipmcopn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hgfknsdy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vaoxedot.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3noseivhy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3znlerigq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cbglzytn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3whizlwxd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3toyljgcb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bnmcuero.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3tllyuedj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gedzjodk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3malcilzc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yqhxdfvb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pvoxlzep.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jompzwrb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dzyapdni.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vsncpizj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vwfrzzmi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qjplmcsj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3itoagsju.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mrxjtcve.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xkwrfmya.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3wosmtnzx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tsjcidsz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kzdwpifm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3umnokbwp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xwmbxzwl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahoosyri.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yrqdlpvc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ohmzugwu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3niihackz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3eolrwjhu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtlelhu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xblzmeim.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wzfjpnnq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3njhjhnxt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3seanlhsx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zuihxjvx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hicvzxis.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nmhezqmi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vhbhacdr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yuxyrazy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lhntrjjt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nazmlnmy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zaohlfon.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3uxrceaal.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ajkoebah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3narmnttt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3klchexee.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3brdavnjf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yhlcyxns.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnusyqf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yuvbytkx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3picviqik.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wloysmlp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zfdgdqtm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jpkiveui.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vdkhaxle.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kluhgjec.html


<!-- 参考信息 -->