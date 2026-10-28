代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hfpthk.cn/gtrmxqkdor.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenlongwang.top/gtvgfiwttl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.pycfn.com/gtunnptocd.html

[B12] 跳出多层循环
来源：http://hz.sysykeji.top/gtxjlfhnnt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenlongwang.top/gtvldnlvtv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ybcxt.top/gtznrantkw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtdrkqjnls.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cqqwz.cn/gtupwuwzrv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtgsbgxobh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zdqjudy.top/gtlnituzyc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zdqjudy.top/gtmsngyhpu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yj202588.top/gtwitxuloz.html

[B13] 判断是否为数字
来源：http://hz.zdqjudy.top/gttcjlfnqp.html

Py:   isinstance(x, (int, float))
来源：http://hz.yj20258888.top/gtksxbrofh.html

PHP:  is_numeric($x)
来源：http://hz.cdnleiting.top/gtnlezhifz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hywenlv.cn/gtcuzuqrcm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xingfuxueyuan.xyz/gtmjlsardl.html

Java: x instanceof Number
来源：http://hz.shuidangran.top/gtoihgedke.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.birdmap.top/gtgwhyjjop.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangshuangyany.cn/gtnplqhcxy.html

C#:   x is int or double or decimal
来源：http://hz.yongpay.top/gttddvurww.html

[B14] 判断值是否在集合内
来源：http://hz.vqdsnc.cn/gtaulvzurj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangtech.top/gtbjujdwve.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hongshengwenyu.top/gtuamlidcu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtmjuyvoxa.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.haohaochexian.top/gtqsoohvhg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.svipenyu.cn/gtskfytnzx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hywenlv.cn/gtgvgmneln.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yvedp.cn/gtzhipybej.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aibaodan.cn/gtrqvmbsdd.html

[B15] 布尔运算与取反
来源：http://hz.shzxlz.cn/gtmccvglem.html

Py:   a and b or not c
来源：http://hz.jinghuilouyu.cn/gtydyyokpc.html

PHP:  $a && $b || !$c
来源：http://hz.xziqi.cn/gtkqlrzdzz.html

JS:   a && b || !c
来源：http://hz.nanxinkj.top/gtzfpxywmw.html

TS:   a && b || !c
来源：http://hz.yueranfly.top/gtribwsknw.html

Java: a && b || !c
来源：http://hz.smart0.xyz/gtuaxodgpk.html

Go:   a && b || !c
来源：http://hz.zdqjudy.top/gtfrlpajow.html

Ruby: a && b || !c
来源：http://hz.xinyue.icu/gtfbsuotys.html

C#:   a && b || !c
来源：http://hz.jinqigfzy.top/gtviekamym.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hnqzz.top/gtthhuygcj.html

Py:   if not data: return
来源：http://hz.daxiang520.top/gttclkqufb.html

PHP:  if (!$data) { return; }
来源：http://hz.ywan-chungtsiang.top/gtmbexgwzg.html

JS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtlpucnsho.html

TS:   if (!data) return;
来源：http://hz.yj202588.top/gtnhfzzhqp.html

Java: if (data == null) return;
来源：http://hz.cashguo.top/gtpvoppuqj.html

Go:   if data == nil { return }
来源：http://hz.iojbl.cn/gthnywzvqj.html

Ruby: return if data.nil?
来源：http://hz.chenlongwang.top/gtpiuaaepf.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangtech.top/gtdsmwzbrq.html

================================================================================
来源：http://hz.wangdashe.top/gtimopivmg.html

C. 函数与作用域
来源：http://hz.bjfxy.top/gthdhtxest.html

================================================================================
来源：http://hz.fengsongda.top/gthwazrqzn.html

[C01] 定义函数
来源：http://hz.dianchejie.cn/gtryrkfczu.html

Py:   def add(a, b): return a + b
来源：http://hz.fengsongda.top/gtlafkfjcw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtwzrnruwb.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.guannengcc.top/gtagslgvuu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtnmaoaivi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gttpewtoqr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ydzc1.top/gthgnnmgdy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.bjfxy.top/gtwbbgumta.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtyahrwenq.html

[C02] 默认参数
来源：http://hz.sysykeji.top/gtohbiyrsv.html

Py:   def greet(name="World"): return name
来源：http://hz.fzhhl.top/gtimkglgbh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cdnleiting.top/gtyfqnnfur.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ehwqpu.com/gttspmjarf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuanzhike.top/gtepbjmzwj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhiwuduotai.top/gtfwfkoelc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shzxlz.cn/gtolipijtp.html

Ruby: def greet(name = "World") = name
来源：http://hz.ppjwa.cn/gtindvozhf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shangyingyoupin.top/gthhyzruxl.html

[C03] 可变参数
来源：http://hz.snrcjt.cn/gtzdjjumsp.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuanzhike.top/gtdtnrsreu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zdqjudy.top/gtpurziqih.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtxcwccqdg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangtech.top/gthirbgutn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zdqjudy.top/gtkovqwazp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.vqdsnc.cn/gtqklcfovb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtfypggjgn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yongpay.top/gtdtrwfhff.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hfpthk.cn/gtkxrufjls.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuetiantiany.cn/gtzikehzht.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cashguo.top/gtkgzeuzni.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gteobxrzhc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhongyouzk.top/gtynnfjbvn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hysaishi.cn/gthgffmbib.html

Go:   // 无：用配置结构体参数
来源：http://hz.cucudq.cn/gtvtopmyvu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtaweixygt.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtykkcgpcx.html

[C05] 返回多个值
来源：http://hz.sufxvd.cn/gttkmhnjvp.html

Py:   return a, b
来源：http://hz.vqdsnc.cn/gthlvdxiln.html

PHP:  return [$a, $b];
来源：http://hz.hnxiangtu.top/gtyijkysar.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guannengcc.top/gtiztiwcty.html

TS:   return { a, b };
来源：http://hz.ydzc1.top/gthkvrcmsr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuanzhike.top/gtdujrckrv.html

Go:   return a, b
来源：http://hz.shuidangran.top/gtozbeoknl.html

Ruby: return a, b
来源：http://hz.0kj1m.cn/gtclsxwsrh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.havefunace.top/gtinfrtksg.html

[C06] 匿名函数 / lambda
来源：http://hz.meibo888.top/gtsxcotbmo.html

Py:   square = lambda x: x * x
来源：http://hz.fengsongda.top/gtcmvuohcp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cdnleiting.top/gtcblxhuxb.html

JS:   const square = x => x * x;
来源：http://hz.gzhubu.top/gtmyeckedm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dianchejie.cn/gtvhazmfde.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.316326.xyz/gtpxjwauyg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zdqjudy.top/gtwxeczyqj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhixingplan.top/gtijmveelb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cucudq.cn/gtofuziljl.html

[C07] 把函数作为参数传入
来源：http://hz.nwbrower.top/gtbzljkiwc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shanyushiyangkeji.top/gtuiylakfc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.haohaochexian.top/gtorboffos.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zycfv.cn/gtteqynqrs.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangkeji.top/gtynopvhzq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.meibo888.top/gtfqcrkhvt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.vqdsnc.cn/gtullagdul.html

Ruby: arr.map(&:upcase)
来源：http://hz.52xcode.cn/gtxaolycvc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhongyouzk.top/gtfqrwivzp.html

[C08] 闭包
来源：http://hz.hfpthk.cn/gtlmoojvnt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shangyingyoupin.top/gtktiylrsw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtmqtylful.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtehoubsbd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtjeiwvgfd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jyoumei.cn/gtmwbgtlwk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gtoylvlioe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj20258888.top/gtkrfndsri.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtaafhlnwu.html

[C09] 递归
来源：http://hz.yangfankeji.com/gttfjoctax.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgufenzy.top/gtfeinhbns.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.andypj.xyz/gtpnodivfw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gotoacloud.top/gtdsvshpsp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ywan-chungtsiang.top/gtrxlyuwzy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yueranfly.top/gtrshgqesw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gaohongyu789.top/gtyiiwtvig.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtllmrycpp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hfpthk.cn/gthalvkuys.html

[C10] 变量作用域
来源：http://hz.iojbl.cn/gtrnqesmvx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuanzhike.top/gtbmuqmccg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxuanxn.top/gtgmwpqfhl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guannengcc.top/gtwxxufofw.html

TS:   同 JS
来源：http://hz.gotoacloud.top/gtfikkswua.html

Java: 方法内为块级作用域
来源：http://hz.nwbrower.top/gtbiwtyard.html

Go:   花括号块级作用域
来源：http://hz.guannengcc.top/gtgnmzzkpk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtwrknikdd.html

C#:   块级作用域
来源：http://hz.ivvv.top/gtamzwasko.html

[C11] 模块导入与导出
来源：http://hz.tanke756.top/gtjvofvdnl.html

Py:   from module import func
来源：http://hz.xingfuxueyuan.xyz/gtpfsfqnqo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xinyue.icu/gtgdhxdjvz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xuanzx.com/gtdphqljkm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.quarkkingdee.top/gtdbkgixur.html

Java: import java.util.List;
来源：http://hz.gotoacloud.top/gtbpoxavrn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shanyushiyangtech.top/gtpkdccdxb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yanxiufei.cn/gtkopjhsrk.html

C#:   using System.Text;
来源：http://hz.aibaodan.cn/gteyrugjnh.html

[C12] 立即执行函数 IIFE
来源：http://hz.feifeiyinyue.top/gtghspdkxb.html

Py:   (lambda: print("run"))()
来源：http://hz.zhaomingkeji.xyz/gtosnyvbht.html

PHP:  (function () { echo "run"; })();
来源：http://hz.c1oappe.top/gtkkmcfsze.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtgufgdfjk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gtskfevdex.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.kuanghao11.cn/gtgucpghgm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.daxiang520.top/gtiofduwdh.html

Ruby: -> { puts "run" }.call
来源：http://hz.ybcxt.top/gtltkglgri.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.52xcode.cn/gtfdbzcpwq.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtiixhvtrb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cheryme.top/gtkpkfppuv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yanxiufei.cn/gtfpkqwdkg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zycfv.cn/gtdgowlhfq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtbpiqfxem.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtmxjtqozu.html

Go:   func add(a, b int) int
来源：http://hz.guannengcc.top/gtwqfkzdnj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydjk.org.cn/gtlanpwocu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtmzphpvgw.html

[C14] 泛型函数
来源：http://hz.yuxming.cn/gtfotqnnvl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigufen.top/gtlwkvvkoj.html

PHP:  // 无泛型
来源：http://hz.zdqjudy.top/gtkflefvcy.html

JS:   // 无泛型
来源：http://hz.cdnleiting.top/gtvauejlll.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhixingplan.top/gtabekmrfv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangtech.top/gtiikdbbai.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.quarkkingdee.top/gtedqovuib.html

Ruby: # 无泛型
来源：http://hz.daxiang520.top/gtyejyxejo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fengsongda.top/gtzvggkjjw.html

[C15] 解构 / 展开参数
来源：http://hz.shzxlz.cn/gtllfkkvan.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgufenzy.top/gtibbbopjp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yangfankeji.com/gticzypzum.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hongshengwenyu.top/gtbzhjdejw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydjk.org.cn/gtuoxzduke.html

Java: // 无解构
来源：http://hz.aibaodan.cn/gtqnplyhis.html

Go:   // 无解构
来源：http://hz.ivvv.top/gtqbrdhdsd.html

Ruby: a, b = pair
来源：http://hz.shangyingyoupin.top/gtnrdwdnaq.html

C#:   var (a, b) = pair;
来源：http://hz.jlsjyb.cn/gtutgigdod.html

[C16] 函数 / 方法重载
来源：http://hz.jiagoushi.top/gtxwaklgkc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangtech.top/gtcfbuhpzn.html

PHP:  // 无重载
来源：http://hz.jyoumei.cn/gtbfuimdku.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dashuyun.cn/gtltsvkzjq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yvedp.cn/gtmlktcdkw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tianlin.xyz/gtbkfftack.html

Go:   // 无重载：用不同函数名
来源：http://hz.nwbrower.top/gthyshpkpl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtlajtfqcu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gogol.net.cn/gtzzkcsaya.html

================================================================================
来源：http://hz.yj20258888.top/gtbtjjltwa.html

D. 数组 / 列表 / 集合
来源：http://hz.jianghu66.top/gtraenazop.html

================================================================================
来源：http://hz.andypj.xyz/gtglgnzylc.html

[D01] 创建数组 / 列表
来源：http://hz.andypj.xyz/gtvhdxlrrt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.smart0.xyz/gtxjuytrrg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.kuanghao11.cn/gtohuabmpi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xylfe.cn/gtoyzmrlng.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sufxvd.cn/gteyucbcjm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gotoacloud.top/gttnpnsxfe.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pengpengdd.cyou/gtdulxetnv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtvtiknsgu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gtiumtpbjl.html

[D02] 追加元素到末尾
来源：http://hz.0kj1m.cn/gtsnkjxnrz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.mhx1999.top/gtxzvvsyvj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.wangdashe.top/gtildrfrmi.html

JS:   arr.push(4);
来源：http://hz.yangfankeji.com/gtuksokrkw.html

TS:   arr.push(4);
来源：http://hz.guannengcc.top/gtnakecsye.html

Java: list.add(4);
来源：http://hz.9152youxi.cn/gtztywzler.html

Go:   arr = append(arr, 4)
来源：http://hz.fengsongda.top/gtajkolnza.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shuidangran.top/gttzhbibbm.html

C#:   list.Add(4);
来源：http://hz.xingfuxueyuan.xyz/gtoidnwszh.html

[D03] 在指定位置插入元素
来源：http://hz.shangyingyoupin.top/gtoulxismh.html

Py:   arr.insert(0, 0)
来源：http://hz.fzhhl.top/gtjqgpsxvf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhengqikj.top/gtrlwktyvs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258888.top/gtxemgvrpi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.bjfxy.top/gtzxcqsiwa.html

Java: list.add(0, 0);
来源：http://hz.316326.xyz/gtldpfpjbu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sweek.top/gturscngfz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cashguo.top/gtseldvmcw.html

C#:   list.Insert(0, 0);
来源：http://hz.quarkkingdee.top/gtcjxhoguv.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtetamocth.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gaohongyu789.top/gtolywkras.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gzhubu.top/gtnuxufnqm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sufxvd.cn/gtfgjsvqdd.html

TS:   arr.splice(0, 1);
来源：http://hz.zhengqikj.top/gtdkftunpq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gtflrhszhx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnxiangtu.top/gtdzlhsfwf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hywenlv.cn/gtupdhmwjr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangtech.top/gttcvvthwi.html

[D05] 访问与修改元素
来源：http://hz.ydjk.org.cn/gtcrejjail.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daxiang520.top/gtewhzxsdu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258888.top/gttvrgovud.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigufen.top/gtknqwthhk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenzaomai.com/gtgpueutcv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.birdmap.top/gtwvujzqqa.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtbwlcmqmh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtitxasqer.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.redwolf501.top/gtbimuqdxp.html

[D06] 数组长度
来源：http://hz.jlsjyb.cn/gtdzgawuqd.html

Py:   len(arr)
来源：http://hz.quarkkingdee.top/gtgqycdgmf.html

PHP:  count($arr);
来源：http://hz.shanyushiyangtech.top/gtqmxgpgtj.html

JS:   arr.length
来源：http://hz.guannengcc.top/gthfrpfvin.html

TS:   arr.length
来源：http://hz.hnqzz.top/gtoacwufio.html

Java: list.size();
来源：http://hz.dianchejie.cn/gtzssexamw.html

Go:   len(arr)
来源：http://hz.hammf.cn/gtoehixrhx.html

Ruby: arr.length; arr.size
来源：http://hz.guowangkeji.top/gtbigdelyo.html

C#:   list.Count;
来源：http://hz.wangshuangyany.cn/gtxzmryvme.html

[D07] 切片 / 取子数组
来源：http://hz.svipenyu.cn/gtjvmwhogn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhijiandao.cn/gtkemoxjji.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258888.top/gtqxydtibm.html

JS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gttnnswdcb.html

TS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gthaxdgolv.html

Java: list.subList(1, 4);
来源：http://hz.zhijiandao.cn/gteoezkwzs.html

Go:   arr[1:4]
来源：http://hz.cucudq.cn/gtcruspiqj.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangkeji.top/gtuafwdvwf.html

C#:   list.GetRange(1, 3);
来源：http://hz.dashuyun.cn/gtiiyyjzjv.html

[D08] 合并两个数组
来源：http://hz.sysykeji.top/gtptjmalfl.html

Py:   a + b;  a.extend(b)
来源：http://hz.zycfv.cn/gtkxkzejqb.html

PHP:  array_merge($a, $b);
来源：http://hz.snrcjt.cn/gterzxtjxk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.smart0.xyz/gtgqymjtju.html

TS:   [...a, ...b];
来源：http://hz.gotoacloud.top/gtfeskfsrv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.meibo888.top/gtnhnbonki.html

Go:   append(a, b...)
来源：http://hz.9152youxi.cn/gtvehvacru.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtwxhiogfe.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuxming.cn/gtwnwgzvgf.html

[D09] 排序（升序）
来源：http://hz.sysykeji.top/gtfsjlexbb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gttgdfbhbq.html

PHP:  sort($arr);
来源：http://hz.sysykeji.top/gtwxpepspm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuetiantiany.cn/gtsfmobuxm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.vqdsnc.cn/gtglkmevce.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.haohaochexian.top/gttmiocmcy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydzc1.top/gtdsxszcfx.html

Ruby: arr.sort
来源：http://hz.sysykeji.top/gtxbddueaw.html

C#:   list.Sort();
来源：http://hz.sysykeji.top/gtknzzpqur.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nwbrower.top/gtsaapwvay.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cucudq.cn/gtbnphuirp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtculdxpez.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtsjrexqsr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jyoumei.cn/gtlxouwzyt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ybcxt.top/gtndnltgmm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.fengsongda.top/gtcspkizeq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aibaodan.cn/gtkhevtsjm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.kuanghao11.cn/gtnumvekpw.html

[D11] 反转数组
来源：http://hz.haohaochexian.top/gtrivdnwng.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yueranfly.top/gtxeaimosx.html

PHP:  array_reverse($arr);
来源：http://hz.c1oappe.top/gthnmvgnbx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhongyouzk.top/gtvmynopvp.html

TS:   [...arr].reverse();
来源：http://hz.yangfankeji.com/gthugsolim.html

Java: Collections.reverse(list);
来源：http://hz.zycfv.cn/gtdbwgxpju.html

Go:   slices.Reverse(arr)
来源：http://hz.xylfe.cn/gteaxurfzc.html

Ruby: arr.reverse
来源：http://hz.aizwys.cn/gtzmwafwrt.html

C#:   list.Reverse();
来源：http://hz.zhoulong.xyz/gtlhsfmsqf.html

[D12] 查找元素下标
来源：http://hz.yvedp.cn/gtebewghwz.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhoulong.xyz/gtwsvpakcu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hnxiangtu.top/gtpscfogdz.html


<!-- 参考信息 -->