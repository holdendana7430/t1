代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tukmwbos.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2muhclivz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytpnzqib.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tmiucnwu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2segiuugr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fqanjbhg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2epmhfpgb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2bzqfuoaf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnvtebfi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2aeqzojpf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dpuzfwjd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgedkkus.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vjbzheip.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nrpnelub.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dihmfybt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tluhxyvi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xwgemlkh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2efiousun.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vsfuijdd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xikdtmxg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qvdeiouf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2itxnhdom.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dssikugz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xsepdjgv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2fgeimamh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2asmazkvn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hznsbcqz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qdlbxynq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ngtaeifa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jgvmjbhw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2snuijicm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vfuqylfm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2npcdzxvh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qfsanouq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zpwndtnn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gssfsuyr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fddbwrbl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ikfigpnh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rfzkdtrw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ywlmpfxa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2twfnumlk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ibtykfgk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2taclxdjw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2pxrxpjud.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uuxyxlff.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ppdsywrr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bropywdd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rznacjck.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvrszbhr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tbvmoacq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qekqchbu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvjqbqc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tybhigto.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ygezelss.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kcozkgxm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2riidnjnh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2eycpxdxv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dxksqkzt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yryhbpjh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hqphwdzq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2laagmgxy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kabuxpvy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kwtsbsky.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rdrkrnye.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hbodflax.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2cyjnhqol.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vngljejm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ctmbzrdx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qhkzkooc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uejnbygo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jwtuumay.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gdeacwyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgfwvryh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zhiukvom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqwcuiuk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oejvaoid.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bujdahvh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sobbmnmh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdjwjnnk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwvnpzly.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tppvwhpf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ngyddzwr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2zsardbus.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pgqxrdag.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ypsnakfo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xnbdbmjj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2hhltpzrh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oadwcqyc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovgvsqyj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2eetpeusj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2uuovcoqm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cogtacsa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mblbrlvi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xdegftiy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gltbujex.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2irqjojxp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsdbhaip.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymrajwmt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2guxdftex.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hixojutc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2owazlcxi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2chuswxdi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rkwarsmk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgdtclh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mnqwimnw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xystqqxq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hqmgxigq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tkiqbfoz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2qvibacdd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyrcjvvm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2djhamzju.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2yvdyeruv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vdqzxfjk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kdnvthpe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hzdrhttu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2shfkhbxm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2xhgoqfmj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ysrqylwp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2euvtxerr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ljcrursb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rddrqcos.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hnqjzlan.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2mummbccy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jwomhbkh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wekxwhul.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2pvzhvcto.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zvqgyfti.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2smldbhtl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pyhxmfdh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jsenqegn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xclsiyyc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2njudfgto.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2akuqnkxy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pavmebjl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lkvuklpr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fhshhklq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rrptccuk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ldzthpis.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ijyznhme.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zlbgcqix.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mpohjuao.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mexiasfj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2misnjzuj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2aebuhpti.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sbevvinr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2majclqkc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecmicpfj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ekwuqvjc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uazsnpht.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ifbknerv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2okttjwle.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qcgzapwe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ppcjgepa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ejbxgzot.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2idbzudkj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2txwqwucr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rllfpcjc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2aezixrlt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xrohgoaz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2irmzznbe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2teaatrkf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bplluvev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kcwujovs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2axzypjdq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rfbdmpmn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xkkjfucc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2picgpedr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nytilnaz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bptxbfmk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2klbocyfw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vrrosgdx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wqvighis.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2spoyajrx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2svsixfld.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2upjyugal.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vamprkgv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mnnuoxnn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dwvuxpqj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2thikvwua.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mkxguvej.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ciwbqbax.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2chclzxya.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kyairfpw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ohgeiyhi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iukukxxo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrgejcum.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nflbdwrl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgjfeivo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojsgjyht.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qplgcmsn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ofxqqdih.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kyohtndv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2snxbghid.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2iydypfhs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2muzwbuaa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ppornfxg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uiifadal.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpewhocm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zhyoqgmw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qxlxtugy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bhaihyou.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2goucuzra.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rzfmobsz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2otasznvc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2evsvrwyo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mxxeedjj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nkptrxhv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hbxrbpwb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lcwykkqx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cmlnamoq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kamrdnte.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kxlgowug.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ddlqjnbx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2xqelwhym.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zqshjrst.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bizeojwc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ssudkbwr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vzjwugqp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdzarbfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epiyjpma.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ealuvdkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnzyfzau.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nvzbiexi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2twfmxgbe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fvsbnnvo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gwpfqiwe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2wyjplmgn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ekriuqce.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mupngkod.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2oznnxjgz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zyvctkvw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nuvxxfdg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2iopkgfix.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ridjyuxb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lhmhonsz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2euprjzzq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2evhimuqu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qszqavao.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ckmndmyi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bsbpzhxg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xqvlgfzn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wrehfhdi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dbmxycfd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2izodcybp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nrmgwimt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tgwjmdsu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfzazvr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2huqwxjjl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bokdidqp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2gzrygqek.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2yuqzyoni.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2nclooejw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2uojwfysg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rauwjtqj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2wxexeurb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ereojpxp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2eudtifel.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2yocjvixt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2adbukrxq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gqoqfptd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2atksuilx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ifmjheqt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lfvvclvr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2nigrpboj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fiyppczq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qevdwjlj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xaxosdaq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oqsjzsbz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hndhtyvt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tzejunhl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cssizyph.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mgtftmtt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2noawsfas.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pmsajqkp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tiedrwcg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2efiwdbnt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kshlzaad.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zdulmjei.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jynorpqc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oxqowdyp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kvnbiute.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dkiriavb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2eduuvxbt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yehzjyyt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mhnentxx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pahigazy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zkhjcyep.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vtxxbxqz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zadjotkk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wqmlrons.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqmaedsu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tvglawqi.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fjvnzeco.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vinjpdvt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2oqghigmw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lspeuvfo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlrfxydk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2zvipytch.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lyscuxia.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ojftbezz.html


<!-- 参考信息 -->