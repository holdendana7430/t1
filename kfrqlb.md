代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtczpzluna.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtdeqhymsb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.pengpengdd.cyou/gtprhthbbh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.dashuyun.cn/gtexktytru.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtgruhfjcq.html

[B10] 遍历同时拿索引
来源：http://hz.wangdashe.top/gtzppcpgwe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jiagoushi.top/gtfxrvkuye.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.vqdsnc.cn/gtgywuvxks.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.mhx1999.top/gthybbkpbc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jiagoushi.top/gtzddbrood.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cqqwz.cn/gtiewsazns.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.aizwys.cn/gtvdjtegzy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sysykeji.top/gtyaeqtupz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.52xcode.cn/gthmwwocnj.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinqigufen.top/gtvhvbwyrt.html

Py:   list(range(0, 10, 2))
来源：http://hz.jinyuanbaomall.cn/gtaojqhtxz.html

PHP:  range(0, 10, 2);
来源：http://hz.jyoumei.cn/gtzrnzfplm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yongpay.top/gtphjjmvlj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daria6918.cn/gtzvygbryu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.tian-w.cn/gtmuycpfva.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.chenjidiqi.icu/gtborzwhnt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ydzc1.top/gthujxaxhq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jyoumei.cn/gtakhgiaos.html

[B12] 跳出多层循环
来源：http://hz.yj20258.top/gtpwubeftf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hongshengwenyu.top/gtwxagaekp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cqqwz.cn/gtrjvwcelu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nwbrower.top/gtydqduady.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gtfwlstbaq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtbsidkhvg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xylfe.cn/gtszezaktu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gthoqlasum.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhijiandao.cn/gtmyyjuczn.html

[B13] 判断是否为数字
来源：http://hz.wangdashe.top/gtvrmstijv.html

Py:   isinstance(x, (int, float))
来源：http://hz.nwbrower.top/gtxpcgefln.html

PHP:  is_numeric($x)
来源：http://hz.xinyue.icu/gtmsanukfl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xingfuxueyuan.xyz/gtlnjqrdew.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.andypj.xyz/gtqekgrzzo.html

Java: x instanceof Number
来源：http://hz.zhongyouzk.top/gthlakqykg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.quarkkingdee.top/gtbowmncpn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangtech.top/gtpzgljvzr.html

C#:   x is int or double or decimal
来源：http://hz.ywan-chungtsiang.top/gtkugjgcnk.html

[B14] 判断值是否在集合内
来源：http://hz.andypj.xyz/gtutuyeaoe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.kuanghao11.cn/gtotvkpayd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cashguo.top/gtnofmrzpv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gteckvoulz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtgsluvzif.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yueranfly.top/gtylqkkxfi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.andypj.xyz/gtcpoielje.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.havefunace.top/gtnzpeqjgl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.havefunace.top/gtqeimochg.html

[B15] 布尔运算与取反
来源：http://hz.ehwqpu.com/gtthzshkoj.html

Py:   a and b or not c
来源：http://hz.zdqjudy.top/gtdmeanxyq.html

PHP:  $a && $b || !$c
来源：http://hz.kuanghao11.cn/gtyqudjshd.html

JS:   a && b || !c
来源：http://hz.fzhhl.top/gtveqklakk.html

TS:   a && b || !c
来源：http://hz.jlsjyb.cn/gtfugvlicb.html

Java: a && b || !c
来源：http://hz.cashguo.top/gtvzoqttps.html

Go:   a && b || !c
来源：http://hz.cucudq.cn/gtqunxklxt.html

Ruby: a && b || !c
来源：http://hz.wangdashe.top/gtfncnques.html

C#:   a && b || !c
来源：http://hz.wangdashe.top/gtsrfvgodb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinqigufen.top/gthvelmwxw.html

Py:   if not data: return
来源：http://hz.sufxvd.cn/gtcjroeqey.html

PHP:  if (!$data) { return; }
来源：http://hz.chenlongwang.top/gtmuceukny.html

JS:   if (!data) return;
来源：http://hz.zhaomingkeji.xyz/gthiicfehc.html

TS:   if (!data) return;
来源：http://hz.hammf.cn/gttzzmgajk.html

Java: if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gthjobvdiq.html

Go:   if data == nil { return }
来源：http://hz.dianchejie.cn/gtvlqikuzi.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangkeji.top/gtokyskgkz.html

C#:   if (data == null) return;
来源：http://hz.xuanzx.com/gtxezsljiw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtsdpdeaou.html

C. 函数与作用域
来源：http://hz.dashuyun.cn/gtxddmgemp.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtexhwwfgr.html

[C01] 定义函数
来源：http://hz.zhongyouzk.top/gtzwjsgvhd.html

Py:   def add(a, b): return a + b
来源：http://hz.52xcode.cn/gtxkwynbjv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtpulwdicn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtsbrsrycn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cucudq.cn/gtfpyatlym.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtjauaaphf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.meibo888.top/gtqittyafj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinqigfzy.top/gtoeautoxr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtfcetkcvk.html

[C02] 默认参数
来源：http://hz.ywan-chungtsiang.top/gtqhxclxcu.html

Py:   def greet(name="World"): return name
来源：http://hz.yongpay.top/gtetebskbn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dashuyun.cn/gtpdjopmuj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hnxiangtu.top/gtmtccnmcm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yvedp.cn/gtgzysjaoq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.havefunace.top/gtjshmdiew.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gzhubu.top/gtgkfnlioz.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gthbhhsddc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhengqikj.top/gtcotamjjp.html

[C03] 可变参数
来源：http://hz.shzxlz.cn/gtljftmcuq.html

Py:   def total(*args): return sum(args)
来源：http://hz.nanxuanxn.top/gthfjbyctk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.kuanghao11.cn/gtreuzydsj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gttoxmtpar.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtkrlsizoe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tian-w.cn/gthjgyzvhv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gzhubu.top/gtwywwavwl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dashuyun.cn/gtzatypvxe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgfzy.top/gtcdxmahqt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xinyue.icu/gtmuxcynac.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.wangshuangyany.cn/gtxlsihnsm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.pycfn.com/gtuicgxpva.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtxvilobve.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenzaomai.com/gtixpvvqqi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.vqdsnc.cn/gthgpzklnc.html

Go:   // 无：用配置结构体参数
来源：http://hz.tian-w.cn/gtmasomtvd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtoruyajlz.html

C#:   f(a: 1, b: 2)
来源：http://hz.andypj.xyz/gtykfgbtqu.html

[C05] 返回多个值
来源：http://hz.52xcode.cn/gtotdkmmkj.html

Py:   return a, b
来源：http://hz.shzxlz.cn/gtfreeqtge.html

PHP:  return [$a, $b];
来源：http://hz.nwbrower.top/gthmezgipj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.svipenyu.cn/gtjkdshjxa.html

TS:   return { a, b };
来源：http://hz.shanyushiyangtech.top/gtcguwxrzi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydjk.org.cn/gthpiogpjo.html

Go:   return a, b
来源：http://hz.shzxlz.cn/gtxrchxzim.html

Ruby: return a, b
来源：http://hz.hnxiangtu.top/gtykeyxcfu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ywan-chungtsiang.top/gtltikpxfn.html

[C06] 匿名函数 / lambda
来源：http://hz.ybcxt.top/gtljxmgqfs.html

Py:   square = lambda x: x * x
来源：http://hz.dashuyun.cn/gtrejsugxp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuxming.cn/gtprzhysyb.html

JS:   const square = x => x * x;
来源：http://hz.tianlin.xyz/gtyumfgzor.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nanxinkj.top/gtmhizegcf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.smart0.xyz/gttyqhivfv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtosxcauwb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.svipenyu.cn/gtygemuyoj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xziqi.cn/gttiuewtaq.html

[C07] 把函数作为参数传入
来源：http://hz.cdnleiting.top/gtnnfrdzzu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgufenzy.top/gtwyqexabn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hnqzz.top/gtjrdwrgeo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aibaodan.cn/gtyhbwcssc.html

TS:   arr.map(String)
来源：http://hz.hfpthk.cn/gtmgihhvyl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sxryk.cn/gtzqburgtp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gotoacloud.top/gtsknmgolw.html

Ruby: arr.map(&:upcase)
来源：http://hz.kuanghao11.cn/gterygkmkv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.vqdsnc.cn/gtjnsgptxk.html

[C08] 闭包
来源：http://hz.mhx1999.top/gtggspsjwf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zdqjudy.top/gtwztitnvy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yueranfly.top/gtqheeqtia.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtrieftghy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sweek.top/gthsrduuff.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigfzy.top/gtvceqiuxj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yongpay.top/gtlxcpqwly.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gotoacloud.top/gtzucmyckb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtziohixgy.html

[C09] 递归
来源：http://hz.yangfankeji.com/gtzwqktmve.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtvllvdjqn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sysykeji.top/gtoinzkfxs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtpeynyjnw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnqzz.top/gtvbutqyyi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuanzhike.top/gtytsofvuz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yvedp.cn/gtjdmwedyh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zdqjudy.top/gtuyixrcut.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hywenlv.cn/gtjnbgwxwq.html

[C10] 变量作用域
来源：http://hz.yj20258888.top/gtipkvvbeq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuetiantiany.cn/gtvjppxpql.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nwbrower.top/gtzhsgrteb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.52xcode.cn/gtlleigmhz.html

TS:   同 JS
来源：http://hz.meibo888.top/gtyclbbxhv.html

Java: 方法内为块级作用域
来源：http://hz.52xcode.cn/gtcvlxatbw.html

Go:   花括号块级作用域
来源：http://hz.ydjk.org.cn/gtzifhhpol.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.svipenyu.cn/gtszxrklzm.html

C#:   块级作用域
来源：http://hz.jinqigufen.top/gtiprgiipm.html

[C11] 模块导入与导出
来源：http://hz.fzhhl.top/gtkbiwxcro.html

Py:   from module import func
来源：http://hz.tian-w.cn/gtsdxsfjqk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.quarkkingdee.top/gtwawprnvv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gaohongyu789.top/gtyfzdquvk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hfpthk.cn/gtnkuxsbxa.html

Java: import java.util.List;
来源：http://hz.aibaodan.cn/gteththtbu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sweek.top/gttzvsradv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yonumen.top/gtgrdinayi.html

C#:   using System.Text;
来源：http://hz.cucudq.cn/gtqddkemgi.html

[C12] 立即执行函数 IIFE
来源：http://hz.redwolf501.top/gtnublipic.html

Py:   (lambda: print("run"))()
来源：http://hz.haohaochexian.top/gtdlnmlldq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gzhubu.top/gtrhafbnvi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtbfwcnrvn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtzucpwbui.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shzxlz.cn/gtyzuwuqmj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guowangkeji.top/gtlsabkfug.html

Ruby: -> { puts "run" }.call
来源：http://hz.yueranfly.top/gtpmigimhv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangkeji.top/gtpmkvalfw.html

[C13] 类型声明 / 类型注解
来源：http://hz.xingfuxueyuan.xyz/gtooucbnux.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gthaqywozp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtxuqjeaga.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenlongwang.top/gtkywtmcwt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gteccqtmzs.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gttytglqxz.html

Go:   func add(a, b int) int
来源：http://hz.guannengcc.top/gtfrtukqmp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtqjvxklzn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.meibo888.top/gtsqjperba.html

[C14] 泛型函数
来源：http://hz.shzxlz.cn/gtufcvarhy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gzhubu.top/gttasyhnug.html

PHP:  // 无泛型
来源：http://hz.hywenlv.cn/gtutosqlpb.html

JS:   // 无泛型
来源：http://hz.cucudq.cn/gttarxhhiw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenlongwang.top/gtskyapstc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.316326.xyz/gteapfsflc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.fzhhl.top/gtchxxhyni.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gthylmxthy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pycfn.com/gtuliofcts.html

[C15] 解构 / 展开参数
来源：http://hz.smart0.xyz/gtgmkmuhfm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtfuoetwdw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnqzz.top/gtsicqfwia.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhaomingkeji.xyz/gtmyaerico.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangdashe.top/gtnomkahlp.html

Java: // 无解构
来源：http://hz.yongpay.top/gtxpsoiemq.html

Go:   // 无解构
来源：http://hz.jqgfzy.top/gtpsnamkwa.html

Ruby: a, b = pair
来源：http://hz.zdqjudy.top/gtmkzowzow.html

C#:   var (a, b) = pair;
来源：http://hz.dianchejie.cn/gtbsqksbjk.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gtjsdrwqnb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gtlomrihrl.html

PHP:  // 无重载
来源：http://hz.tanke756.top/gthkdxisnf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daxiang520.top/gtmefarepl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtyetdahxh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtxdwisikz.html

Go:   // 无重载：用不同函数名
来源：http://hz.c1oappe.top/gttvfyxcac.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxinkj.top/gtksqyqyma.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhengqikj.top/gtekfjqiht.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrmnisfvx.html

D. 数组 / 列表 / 集合
来源：http://hz.yueranfly.top/gtxcjyhfwx.html

================================================================================
来源：http://hz.iojbl.cn/gtbbrbrlor.html

[D01] 创建数组 / 列表
来源：http://hz.9152youxi.cn/gtcyepxixu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtgkjleqvp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ehwqpu.com/gtqhygvmtp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yonumen.top/gtrgkliqrt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dashuyun.cn/gtgsgozyts.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.andypj.xyz/gtuexqaldc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xziqi.cn/gtgicpkokt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.iojbl.cn/gtlwaitzjs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aizwys.cn/gtisgxazpk.html

[D02] 追加元素到末尾
来源：http://hz.quarkkingdee.top/gtqxhfhzkr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ybcxt.top/gtudatkrpy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ywan-chungtsiang.top/gtopvqzius.html

JS:   arr.push(4);
来源：http://hz.tian-w.cn/gtcnikqtys.html

TS:   arr.push(4);
来源：http://hz.snrcjt.cn/gtwkumomqe.html

Java: list.add(4);
来源：http://hz.yanxiufei.cn/gtqhiwhenj.html

Go:   arr = append(arr, 4)
来源：http://hz.andypj.xyz/gthrpijepy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenjidiqi.icu/gtxgfydidn.html

C#:   list.Add(4);
来源：http://hz.nanxinkj.top/gtzhrrncog.html

[D03] 在指定位置插入元素
来源：http://hz.chenlongwang.top/gtlasjhtpo.html

Py:   arr.insert(0, 0)
来源：http://hz.hysaishi.cn/gternuwonr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yonumen.top/gtaupaccwc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.bjfxy.top/gtrqyjzyfx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.dianchejie.cn/gtqncluwij.html

Java: list.add(0, 0);
来源：http://hz.tian-w.cn/gtvtenfflz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinghuilouyu.cn/gtmenwweor.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gogol.net.cn/gtlxsvixoo.html

C#:   list.Insert(0, 0);
来源：http://hz.hysaishi.cn/gtzppvaptl.html

[D04] 删除元素
来源：http://hz.cdnleiting.top/gthrwpkurc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhengqikj.top/gthuhwducl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jiagoushi.top/gtvtyeqrqy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yvedp.cn/gtvfrpwqdf.html

TS:   arr.splice(0, 1);
来源：http://hz.sweek.top/gtyvvqtrpr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenzaomai.com/gtsgzhrzcz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.9152youxi.cn/gthuyyzplp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.vqdsnc.cn/gtdcwmblea.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.birdmap.top/gtntbqfabt.html

[D05] 访问与修改元素
来源：http://hz.shzxlz.cn/gtijodrlrw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtuisazuci.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shuidangran.top/gtwaiozpjj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj202588.top/gtxialyzub.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zycfv.cn/gtfnhscjyy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenzaomai.com/gtteszvdhj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gzhubu.top/gtdxpcdyld.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtcvqbsosr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ybcxt.top/gtfspspfqz.html

[D06] 数组长度
来源：http://hz.sysykeji.top/gtxjtjagzg.html

Py:   len(arr)
来源：http://hz.jqgufenzy.top/gtzrihexpu.html

PHP:  count($arr);
来源：http://hz.tianlin.xyz/gtzqlrxypl.html

JS:   arr.length
来源：http://hz.jinghuilouyu.cn/gtkljbflcy.html

TS:   arr.length
来源：http://hz.chenzaomai.com/gtcjobvwua.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtbtwfdqcw.html

Go:   len(arr)
来源：http://hz.yonumen.top/gtudbcplas.html

Ruby: arr.length; arr.size
来源：http://hz.daria6918.cn/gtjzbbfiyd.html

C#:   list.Count;
来源：http://hz.0kj1m.cn/gtsrofxage.html

[D07] 切片 / 取子数组
来源：http://hz.hnxiangtu.top/gthoqkedcc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ywan-chungtsiang.top/gtobbpfpob.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gtfvfupdpd.html

JS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtmjxdiknf.html

TS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtcepgfxls.html

Java: list.subList(1, 4);
来源：http://hz.jinqigufen.top/gtenbtwuzy.html

Go:   arr[1:4]
来源：http://hz.kuanghao11.cn/gtnkcqqywf.html

Ruby: arr[1, 3]
来源：http://hz.quarkkingdee.top/gtlmtbaqqo.html

C#:   list.GetRange(1, 3);
来源：http://hz.daria6918.cn/gtyjustfmc.html

[D08] 合并两个数组
来源：http://hz.chenjidiqi.icu/gtoyfgcuew.html

Py:   a + b;  a.extend(b)
来源：http://hz.ydzc1.top/gtgeqsgghk.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtsffjfbmy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ppjwa.cn/gtrwnlqgcy.html

TS:   [...a, ...b];
来源：http://hz.snrcjt.cn/gtnmtfsech.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ywan-chungtsiang.top/gttuxyacty.html

Go:   append(a, b...)
来源：http://hz.zhaomingkeji.xyz/gtfjmesazx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtwzyggxwk.html

C#:   a.Concat(b).ToList()
来源：http://hz.nanxuanxn.top/gtvorcizji.html

[D09] 排序（升序）
来源：http://hz.shuidangran.top/gtbzmpifts.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtsccgdehk.html

PHP:  sort($arr);
来源：http://hz.jlsjyb.cn/gtwxwfsdvj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhaomingkeji.xyz/gteddnuycv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cucudq.cn/gtuiubphfc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.haohaochexian.top/gtiptvmebc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtzqhkqqxp.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtvtyvmnoz.html

C#:   list.Sort();
来源：http://hz.haohaochexian.top/gtnptvnohs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daxiang520.top/gtdinsmeav.html


<!-- 参考信息 -->