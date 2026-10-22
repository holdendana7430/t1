代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2jpgkghxm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2yzyrqlsz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzycuwat.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dulqenvw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2obssjaas.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zfyaoaor.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vhvwzfsy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zzyvjslf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgifcjxf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2plzbqdzl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bmhjvscb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zenpplmw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vlvcgzjc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qmfooyfm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2idivdmwq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pqakpfoc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2oklkyyvp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvkthium.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rnlytqku.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nnkkgxur.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kypovugc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gwmmpkcy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cekxenhl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tijbimdh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uezjgwus.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bmcogahm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jvjsrkks.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ysbntenm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wqttxiqz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ksmmqxdz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wxlxrggh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hkzhskem.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jtvgfijh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2oikenhsv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2uuwufvks.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dmduqlds.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rqjdwnvo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2lswhtiws.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqeqoorw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2snevmcnn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fzjbmlxz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2evihfewk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2uiaabiij.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ornbaiuv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rgtomyvq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2yevecjxl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2chwecwwd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gjymyiwx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rixotgwm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2albqdhpd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dwbszssz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tsszsdbs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbseprzv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jomjlmsc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ositjkzj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ymntxgmd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bitrmfih.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eluwwrer.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2izvgihpw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vniokqfo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ohiaaxdr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ibdedrif.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hfbcywyk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fnrjbhuc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mxnprmgk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jdcgreaz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xmpledzy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2njxezmce.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pbdgwxar.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2btwbqjxo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pnqmiqyo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2piintfsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdpixwqx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vctgexbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqvjivhb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2velrolas.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fneegqgg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqrllagk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2atygttgb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kjmmapwu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cydgnrfw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2iohlxwmb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2oxagjuvk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rzfnvbde.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wustkxvl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2kewvxwef.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nmoocmoa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ejrlipmx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojaopalo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2csxrzexk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dmzhsuse.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ybwgtvgl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xsvvvyqp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2daihrrgl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gukndjqe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2koxomsue.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqbobvsu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sdevyznf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ovosrmwr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zilwastk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqvzitzv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jhwwzjen.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ramlvcwy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2exvvnlcp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2xksxcqul.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bjpdered.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ekqczyge.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jlvhhnqp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmirrhdj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvphuhd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrlzteku.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pklmizam.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nqybarjz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2cgphaqff.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cybhzoyp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nqvvzvsd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kqltbxfe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rhljgcdq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hgxbhbrq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tcwplddc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mqpcxgic.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kgddlvfh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rejpugah.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lataegbk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2willuack.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ambhxcxn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qvdloqqb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jflndors.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kzryozmu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2szultvxl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jaueimkj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fuoantun.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2tktellne.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yeigtyfy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2esnfirrc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2kocrojxc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2maufmoaf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qwbqgjbg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2anojfngg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qgspwwft.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2osgpdyog.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gatcywlb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcljhbxr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2agrrkcbv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2gryrrren.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wyfszbmk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ourlvtpg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrtixqah.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjjppva.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2elfylwpk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2majpfyjf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2adeacmoa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2eosjhgnz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2pmpqanzh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgryjrzw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2zywypjbs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cafbcfox.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fnoildbm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hnycisgt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2okwbxzli.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ftmvthkh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hxenpncr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jnehqcmq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2shdbwmve.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kubwzeqq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2rphixmat.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fdomifrs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2mtyxmfcj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2joyzvubf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xuxuvmua.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zacrwjhz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pyzxfvqd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xowbwzsy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lwfdrjwh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ajoueimn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xypqhzcs.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2skrsuuxe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hpgpdkiu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dzrjqdkv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2egsdmxti.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2drwneydm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ocvnuobm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dsqganom.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2adkrsfqd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2swdjxgan.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xnzmpctr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2cuhccgdf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yvcmoabp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qubmowzp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2kxxwhqrv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sszdyerx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2uxapdrti.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbvjjtcm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2cruzqmnd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2czzrglfr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yxzbdlfp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmcucunr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zvryyyfe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gocrvupl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xcdsaxhl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2spjfezxe.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qptxdkvl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ltxgijlk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hevjlbfi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ahgjdgxl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qechnual.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lxypxnmh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2puydatmo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2equzurbr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rtzaoklv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xvvkkgof.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ugabbczn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vyevjknn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2bgohorvi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rdwjyanm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ikvtqjyx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zgckbllb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2uxniobvv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2whnvfwku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtbcjtti.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qmtgwozv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grxxcbsl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2phayipmg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wuymkznq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2geknypvx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wxccmrmn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2jcxnqpzf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2liomrcew.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kkurlwbn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dmtaveqe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qvjixfjq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wbxhhsdv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fvjkzhty.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2pcwhjkvi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vqktmhmd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2inwdplwt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vnrqibjz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2aofieern.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2klugbgwp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fpezebbb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lgcnxush.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mlukjkij.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gsdauitn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zyadwpsm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hvlvrtjx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2roqwilyr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbyuvou.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2iqinmfze.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kdzucoos.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hnfnwkml.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cygiqioi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wavwoptv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zzapffax.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xzwzrppp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xyaoixna.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ycezorit.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hjmzfbsy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ejxvivrr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lilpadme.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ywoiwkll.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bzuvwayt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iuipgydy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fchsmdzd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ebcbvbbq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lwfxcmvb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rzhpsyoa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gysxlyqy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qmxwszti.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkbkinje.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yyjtwnkt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2quirxgxr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2erxumjcc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2okpfdbgg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tyknuovm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ictyzhjx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dbgvsuba.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xvusciqt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2cyotqafd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nmabgdxz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jzcxpvic.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2orghurhy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uqmzooan.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kwlebycb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cnwotihm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2snijgltg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wlwzgbxd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mexnfbpq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2pswudmir.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lggzlvaq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bcoejesj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lwrtndlq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mtcgduxi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sszmqlrb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jnkspaye.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jhvprcdm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mxryxgxe.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2djzbuthd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2zxzjotny.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2najouwln.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2spwrgxez.html


<!-- 参考信息 -->