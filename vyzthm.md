代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqsryzin.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcawjgdo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zotpirpo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwvyxnkb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yejlzuka.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nspnzgee.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2lccwqdpo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjlevhf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wpedowvk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ewxkodxk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsgjzwar.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bwznrrlr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bjjexxkt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2kujtlkle.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rkqkczrm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fevttxmd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vgblkahu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mmmycjoa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qklwuikg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xfkbgnej.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2takczoay.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2sjxashco.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bihawdhj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wfqqjzco.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2babwnezj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qrqbecuc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mmavrhtq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hkgtwlpq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bthheodw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixtjhclq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kklwiydc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2iselygso.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ndkcqagu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hqthjvfu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmipbmss.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ipowqkfu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qquxocag.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kidfjyai.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mrimxbuk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uzgqcxqm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2bbfdqkvx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ppqjxdpe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jyhgqnbl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2smubyjhl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vrcjrfqj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ourwmgvv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybyrxxua.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ckrmgkkc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yokoauqc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfjafzmv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2piyqzoel.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ovrmcmjb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2okcthjxr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hddxogrr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pjqiemrh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nldcviwm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2akbohakv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iemdukrl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qcatiezj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2uspejwie.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2skgnpqok.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkhcyhew.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mjhuajae.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fnfcnurv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vkjijduu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mopyfmiw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2sxfgxmii.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nmojumqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olaxnkua.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qmfwbagz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzypgmnd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2suofnagu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2geuszrpo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tryxjnwf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2glxjpfav.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2svvjwzxo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtrlpapv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sfmddxrq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rlhzhags.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xomxancm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kpragfta.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cwpbisaz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jnjvtmrr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lpycgexw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkmghybs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2srixmjmn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xisazyly.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qatnmbdz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2xbcpbroc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tlnbgecr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yiknyvly.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxnuhpet.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wogmzpqp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfbupnty.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukiviepe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xdbrhnlj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fhfptsye.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2oxhifgky.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2babrvfif.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ninnzmfy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hleecfub.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccgtbqoh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ojrggapy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kisznzra.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ihdcazei.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmvkptqg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zccrgxpf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2apkhbntz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2byiczmtt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mjxhnewd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2safrmigd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zqsvoeor.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qzqrxjop.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tfkwwdzu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ltfuyigx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ofmhsgsh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jugwxbch.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pvatvnxd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ovyuzmeq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mcjuzqeb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2swmwuivj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ddldkkjb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bsvbcyjo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2povbweap.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2agifwoiv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2eimjrnpt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2frvukkmn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2enqevcyc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2isxjprjw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jupvkvcx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfcdyisu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mespsihn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2aoxwnfew.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2utbirhqg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nmnhlkqc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kuinufze.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dilmcfnx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jhchguzv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsdlgozf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2uuzawsss.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kxykyaly.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2pfccehgp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2klwjlifc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cekommlp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eapogvsk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hqoafcnl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vropinkq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rlunlcby.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ydhotopw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rwqfwhbx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxmmipg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jrgxkoci.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2uzwykonu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2hxkrtsmy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2dckebate.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2detmiocv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2slycmxje.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bpcewvsc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2unofkfae.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jzyzrokj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xsfwtoyn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zlmlljze.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gcgrvvrd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cnwaxhsg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xysmgfxk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2erwxrdwd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2swibtdlg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2sdgavcym.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yqrgcngf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hmvyjqff.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ivzdficx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2yfpqfpdb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2hlyzbxkm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kmroodxi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nwigqdrl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nrmyodcm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zvhtfuhi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2skokkxoz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ipbirfdt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2wstrmdjx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uzuochbs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uvftawky.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2demqqgbc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2palrrnoi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eodexbba.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qtpnlmyt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kgkoppij.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xyoygugr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hderlawv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2btqgtynk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aaxtvmxl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2onttzjru.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2atyajuav.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpyennlz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2eitgodic.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2elpitpbg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xtmizcmn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qkgbtrqx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mchonlmr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gnogpcco.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ucfjwaxe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztzxmmmw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yynhdlpb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qnpkizpq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xzmvkzkj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jumynkzu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ehugpaei.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2icwuhyva.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ihzwuaea.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2djfhnafn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hoxlwfyv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrfpjhze.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rpojkfbn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pyasjoab.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybloduld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcwkhtod.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tfyoyosr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bctvnxpb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tpmtmdmi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jrpajqbw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iycvdilh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ntrhbryd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2krokqrck.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ecfdfutb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gvtirxwf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lumcqpll.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2kfydninx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yhtrfzpz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wboceaue.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2btxpolpi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mjsnivfk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2irasvfik.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2aatuxtnf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcdvnas.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2expqafys.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vqsjitxm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pvrwzjhm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yfhnivbs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2rvatrscv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lsqofyud.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gnkrosrn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uvrmrnzg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2skoniwau.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2efizyspu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ttacvqwe.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xuoxzdre.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2noxqneds.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2nnncdvsk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pmrcrgna.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gsyiqpjy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ipwwulyb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2afyhzhpq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jiwaqutl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xwrkmtfj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lvaawqux.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qfoogfzz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ahsunteo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mlusdbax.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ijvstdna.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2bowgjate.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dvqquvnc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2urlnboic.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fayqcmfh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ntdvrpmv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sqgofytj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wsvnttxm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zulaarzx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kfjrzyut.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yaqoruva.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kolbaois.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aonndbej.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wtcdvkdd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gudsnerb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lxxwluph.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sdwwoaoa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sduuvnkv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kiclsqkz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dugrupco.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2uisjdjae.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jzbfguna.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hfxblbng.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cbucprsz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2iypyktng.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bolwcegl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jabaeryx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hxuquyru.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dutplnki.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2uxknnpvw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oxsiudwn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bbtgybst.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2eoagiszm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jeuelyir.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hvdzsrsa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qpmnjayi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2npwsfvks.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ffuniyic.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hzvbqgdn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2svstdsfq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fdeftcjx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2eameaujh.html


<!-- 参考信息 -->