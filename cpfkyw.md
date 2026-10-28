代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hywenlv.cn/gtlhdikltf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ivvv.top/gtnwphtxyu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jianghu66.top/gtzhqnoqpl.html

[B12] 跳出多层循环
来源：http://hz.jinyuanbaomall.cn/gtwswdwcku.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhengqikj.top/gteoaxegwz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cqqwz.cn/gtthuzckcu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guannengcc.top/gtenketckh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtispgjmhv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtiklfuzdc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cashguo.top/gtimsfhobf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zdqjudy.top/gtnadabyrq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ppjwa.cn/gtzaxjidhf.html

[B13] 判断是否为数字
来源：http://hz.xylfe.cn/gtnjzlawjb.html

Py:   isinstance(x, (int, float))
来源：http://hz.ppjwa.cn/gtmacekcqv.html

PHP:  is_numeric($x)
来源：http://hz.zhijiandao.cn/gtrhilszjh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jyoumei.cn/gtmcblqygi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cucudq.cn/gtkhnlbtam.html

Java: x instanceof Number
来源：http://hz.jlsjyb.cn/gtrlnhqgqx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gaohongyu789.top/gtjcdjmmzf.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shangyingyoupin.top/gtgvltvteh.html

C#:   x is int or double or decimal
来源：http://hz.pengpengdd.cyou/gtmsydhywc.html

[B14] 判断值是否在集合内
来源：http://hz.bjfxy.top/gtsxvowjln.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.0kj1m.cn/gteztdgltg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yanxiufei.cn/gtrmqkilta.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtqguiyitd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtxeezzooz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shanyushiyangkeji.top/gtabypldkv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ybcxt.top/gtjdsysflt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jqgufenzy.top/gtwatrxkkv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tian-w.cn/gttlgezwga.html

[B15] 布尔运算与取反
来源：http://hz.cqqwz.cn/gtcwojnxyz.html

Py:   a and b or not c
来源：http://hz.ywan-chungtsiang.top/gtawfhtepz.html

PHP:  $a && $b || !$c
来源：http://hz.ydjk.org.cn/gthlxxejyq.html

JS:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtgvubtlyr.html

TS:   a && b || !c
来源：http://hz.havefunace.top/gtouumpdrp.html

Java: a && b || !c
来源：http://hz.redwolf501.top/gtwkmnshbs.html

Go:   a && b || !c
来源：http://hz.jinqigfzy.top/gtljqnwaow.html

Ruby: a && b || !c
来源：http://hz.wangshuangyany.cn/gtifuvhsih.html

C#:   a && b || !c
来源：http://hz.cqqwz.cn/gttmfetdur.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guannengcc.top/gtsojlxyzx.html

Py:   if not data: return
来源：http://hz.cdnleiting.top/gtxbwauxhv.html

PHP:  if (!$data) { return; }
来源：http://hz.ydzc1.top/gtievaefqe.html

JS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gtdfjbitnp.html

TS:   if (!data) return;
来源：http://hz.nwbrower.top/gtgouzefwm.html

Java: if (data == null) return;
来源：http://hz.fzhhl.top/gtvdtkdzxz.html

Go:   if data == nil { return }
来源：http://hz.zhijiandao.cn/gtkqxlyubg.html

Ruby: return if data.nil?
来源：http://hz.cqqwz.cn/gtwrbbnuze.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gtooxirtwx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxcogrncs.html

C. 函数与作用域
来源：http://hz.bjfxy.top/gtzttlcuob.html

================================================================================
来源：http://hz.dashuyun.cn/gtphkbgwyv.html

[C01] 定义函数
来源：http://hz.zhoulong.xyz/gtfddzcntn.html

Py:   def add(a, b): return a + b
来源：http://hz.cqqwz.cn/gtizzsmblz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnqzz.top/gtogpryiyg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jiagoushi.top/gttjslunis.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yanxiufei.cn/gtvifjpzni.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtihivwdac.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.birdmap.top/gtntngrkpg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yonumen.top/gtamkkojey.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gttcnxgzmi.html

[C02] 默认参数
来源：http://hz.yuanzhike.top/gtrqanmqmc.html

Py:   def greet(name="World"): return name
来源：http://hz.guowangkeji.top/gteckuojbj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cheryme.top/gtjdhezfgf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.birdmap.top/gtnzhxrulg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnqzz.top/gtitomhhha.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hammf.cn/gteewejoev.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxuanxn.top/gtpvvtzqsf.html

Ruby: def greet(name = "World") = name
来源：http://hz.shzxlz.cn/gtevbaimgc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhijiandao.cn/gtjestxihg.html

[C03] 可变参数
来源：http://hz.hnxiangtu.top/gtjzytfkeb.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenzaomai.com/gtizwdpdzk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.redwolf501.top/gtkbanpnfy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gttxcjrhyc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtpzycubpl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuanzx.com/gttttoeujl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ppjwa.cn/gtybqvffvq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhoulong.xyz/gtndsknsqs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.0kj1m.cn/gtgxrqinet.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zdqjudy.top/gtaqappdmn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nanxuanxn.top/gtepkonequ.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shangyingyoupin.top/gtmepwydws.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daxiang520.top/gtcwoinwbf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yangfankeji.com/gtwssosvdu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuetiantiany.cn/gtxnjklnhx.html

Go:   // 无：用配置结构体参数
来源：http://hz.jlsjyb.cn/gtgeijyitk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.birdmap.top/gtdtxtzunc.html

C#:   f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtfffzcruv.html

[C05] 返回多个值
来源：http://hz.yueranfly.top/gtygkhegzc.html

Py:   return a, b
来源：http://hz.kuanghao11.cn/gtzqwnkcpp.html

PHP:  return [$a, $b];
来源：http://hz.yangfankeji.com/gttbyejqmy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yanxiufei.cn/gtetqqvrld.html

TS:   return { a, b };
来源：http://hz.jinqigfzy.top/gtcguvhkwq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fengsongda.top/gtwyevwqsk.html

Go:   return a, b
来源：http://hz.ppjwa.cn/gtduhnqmkt.html

Ruby: return a, b
来源：http://hz.cheryme.top/gtwarvklho.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhijiandao.cn/gtxpmajknq.html

[C06] 匿名函数 / lambda
来源：http://hz.fzhhl.top/gtcqhlxhix.html

Py:   square = lambda x: x * x
来源：http://hz.jqgufenzy.top/gtyapgvcej.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yanxiufei.cn/gtetbnmgco.html

JS:   const square = x => x * x;
来源：http://hz.kuanghao11.cn/gtuwqohwbz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cdnleiting.top/gtehbeaxww.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhaomingkeji.xyz/gtctnhxvqy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.quarkkingdee.top/gtkjwvumjs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhiwuduotai.top/gtwxkbdaum.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.andypj.xyz/gtvvrdmdiz.html

[C07] 把函数作为参数传入
来源：http://hz.ehwqpu.com/gtukkuivxc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhoulong.xyz/gtknuzmrxg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sufxvd.cn/gtbmjutabg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shzxlz.cn/gtjtetddwd.html

TS:   arr.map(String)
来源：http://hz.sysykeji.top/gtpartvjop.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hammf.cn/gtjfhqhpwi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hfpthk.cn/gtclyrsytl.html

Ruby: arr.map(&:upcase)
来源：http://hz.dashuyun.cn/gtseaowqcg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shuidangran.top/gttfzcdygn.html

[C08] 闭包
来源：http://hz.yj20258.top/gtyouffxqx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hnqzz.top/gtzkpcwedm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangtech.top/gtwocesjwo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gthcckylqv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtylyzltlx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cucudq.cn/gtozjesoka.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xinyue.icu/gtzbcdcigb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cashguo.top/gtaqmsfxot.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtviwrtldr.html

[C09] 递归
来源：http://hz.jqgufenzy.top/gtkrhvzpmw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yongpay.top/gtmkqyzebt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigfzy.top/gtpvoqmvwh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuanzx.com/gtdixmsymw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtylndsyqm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tianlin.xyz/gtoyntzggp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yangfankeji.com/gtrtpixzmu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtxvbyofkd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yuxming.cn/gthpklcool.html

[C10] 变量作用域
来源：http://hz.redwolf501.top/gtlrftrutz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ivvv.top/gtcmcecqly.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnxiangtu.top/gttrbdvkmc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.svipenyu.cn/gtvovnhbrn.html

TS:   同 JS
来源：http://hz.zhiwuduotai.top/gtqrllonjg.html

Java: 方法内为块级作用域
来源：http://hz.wangshuangyany.cn/gtngvjbbgz.html

Go:   花括号块级作用域
来源：http://hz.dianchejie.cn/gthioosvjr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.smart0.xyz/gtvdqkvjqh.html

C#:   块级作用域
来源：http://hz.cucudq.cn/gtbhcjjztg.html

[C11] 模块导入与导出
来源：http://hz.shangyingyoupin.top/gtlgrjahop.html

Py:   from module import func
来源：http://hz.pengpengdd.cyou/gtjojkcgup.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenjidiqi.icu/gtpfjnxoaj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.svipenyu.cn/gtqqcaezgs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jiagoushi.top/gtozadbawt.html

Java: import java.util.List;
来源：http://hz.gogol.net.cn/gtpnstqlla.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cdnleiting.top/gtivnzjzec.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.0kj1m.cn/gtfwhnyltw.html

C#:   using System.Text;
来源：http://hz.hfpthk.cn/gtvsloryio.html

[C12] 立即执行函数 IIFE
来源：http://hz.yanxiufei.cn/gtywupgxum.html

Py:   (lambda: print("run"))()
来源：http://hz.xinyue.icu/gtkvpwojwx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.daria6918.cn/gtnpestdwy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dianchejie.cn/gtsgrymurt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.daxiang520.top/gtdddabkcp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yangfankeji.com/gthbmvvzlg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.bjfxy.top/gtepaocpoi.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydjk.org.cn/gtlzukdzxi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhongyouzk.top/gtozrvggxj.html

[C13] 类型声明 / 类型注解
来源：http://hz.gzhubu.top/gtjdsjqkuv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj20258.top/gttznjufpl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtxlmozzgt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nwbrower.top/gttdsbrlem.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtihqnavka.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtdhiejtui.html

Go:   func add(a, b int) int
来源：http://hz.ppjwa.cn/gtkqvyhnjb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258888.top/gtperompth.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gtootqkmpl.html

[C14] 泛型函数
来源：http://hz.guowangkeji.top/gtvcupfzxu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtflwnbtsw.html

PHP:  // 无泛型
来源：http://hz.9152youxi.cn/gtmjerjnch.html

JS:   // 无泛型
来源：http://hz.zhiwuduotai.top/gtitydqmwq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xylfe.cn/gtpaprgfff.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guowangkeji.top/gtuuvmmazh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gzhubu.top/gtxdafzfql.html

Ruby: # 无泛型
来源：http://hz.aibaodan.cn/gtzzpolgxx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guowangkeji.top/gtjsxkpesf.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gtaizbhiof.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daria6918.cn/gtejstwbiu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pengpengdd.cyou/gtvxiaklfg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.redwolf501.top/gthjyrfehr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtpbgaeaky.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtykzpvjvx.html

Go:   // 无解构
来源：http://hz.meibo888.top/gtxfkeixsq.html

Ruby: a, b = pair
来源：http://hz.cdnleiting.top/gtdfljyijj.html

C#:   var (a, b) = pair;
来源：http://hz.jqgufenzy.top/gtfbcfvdpt.html

[C16] 函数 / 方法重载
来源：http://hz.shuidangran.top/gtvetmlruq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.316326.xyz/gtchfemvjz.html

PHP:  // 无重载
来源：http://hz.bjfxy.top/gtqfwrtjtw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xinyue.icu/gtafewykxs.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aizwys.cn/gtqcflqxav.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinyuanbaomall.cn/gtpdwzdrcj.html

Go:   // 无重载：用不同函数名
来源：http://hz.cashguo.top/gtcohnhust.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jianghu66.top/gtviofvopp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhiwuduotai.top/gtwqlalqvn.html

================================================================================
来源：http://hz.jinqigufen.top/gtlpuyyczb.html

D. 数组 / 列表 / 集合
来源：http://hz.zhaomingkeji.xyz/gtotbkavne.html

================================================================================
来源：http://hz.yongpay.top/gtvmneqagz.html

[D01] 创建数组 / 列表
来源：http://hz.daxiang520.top/gtazzhvmkr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangshuangyany.cn/gtqsapynka.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhixingplan.top/gtuqlrupih.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xuetiantiany.cn/gtiwugaato.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fengsongda.top/gtuhbkefhv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.feifeiyinyue.top/gtcoatihhp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuanzx.com/gtipibhkuk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sysykeji.top/gtfuhikwbc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenzaomai.com/gtuvebkhow.html

[D02] 追加元素到末尾
来源：http://hz.zhixingplan.top/gtiekycxhp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cdnleiting.top/gtmckgzfjb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.mhx1999.top/gttswhveko.html

JS:   arr.push(4);
来源：http://hz.cashguo.top/gtlgmhfljy.html

TS:   arr.push(4);
来源：http://hz.wangshuangyany.cn/gtniejzknf.html

Java: list.add(4);
来源：http://hz.guowangkeji.top/gtyautdvwq.html

Go:   arr = append(arr, 4)
来源：http://hz.ydzc1.top/gtpujfhzyr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ydzc1.top/gtzgidrbzt.html

C#:   list.Add(4);
来源：http://hz.zhiwuduotai.top/gtuszksnuu.html

[D03] 在指定位置插入元素
来源：http://hz.feifeiyinyue.top/gtadfpclwl.html

Py:   arr.insert(0, 0)
来源：http://hz.chenjidiqi.icu/gticqeskgp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtvwenhetu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xuanzx.com/gtyibubusc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cashguo.top/gtwjuwsosk.html

Java: list.add(0, 0);
来源：http://hz.zycfv.cn/gtbwuipejo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gtmhgfthhh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pengpengdd.cyou/gtmrhcydry.html

C#:   list.Insert(0, 0);
来源：http://hz.vqdsnc.cn/gtoltmhpiq.html

[D04] 删除元素
来源：http://hz.zhijiandao.cn/gtngvaigqd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtyucmsiui.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.birdmap.top/gtbijldsxu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xinyue.icu/gtjralmlse.html

TS:   arr.splice(0, 1);
来源：http://hz.tianlin.xyz/gturqvktgj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yonumen.top/gtfdvotwwq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.haohaochexian.top/gtdbospudt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.haohaochexian.top/gtxcrmgoip.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jqgufenzy.top/gtdgveevrg.html

[D05] 访问与修改元素
来源：http://hz.chenjidiqi.icu/gtrjzsnkyn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtquzomjsk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtwofoosyi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jiagoushi.top/gtkhilcubg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangtech.top/gtbxugijmv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gtmsejlmiq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.meibo888.top/gthaqcapms.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtgxzmupux.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sufxvd.cn/gtcieuiqji.html

[D06] 数组长度
来源：http://hz.c1oappe.top/gtdvsdtibo.html

Py:   len(arr)
来源：http://hz.tian-w.cn/gtsygnwkhp.html

PHP:  count($arr);
来源：http://hz.nwbrower.top/gtwufazmxm.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtduzdokoq.html

TS:   arr.length
来源：http://hz.havefunace.top/gtcyklnnfz.html

Java: list.size();
来源：http://hz.andypj.xyz/gtckrmenap.html

Go:   len(arr)
来源：http://hz.ppjwa.cn/gtjmdaazmv.html

Ruby: arr.length; arr.size
来源：http://hz.guannengcc.top/gtsyrpiizy.html

C#:   list.Count;
来源：http://hz.yvedp.cn/gtpsxylouk.html

[D07] 切片 / 取子数组
来源：http://hz.aibaodan.cn/gtbgjekbxu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinghuilouyu.cn/gtyjowqlqd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sweek.top/gtkyhwtqhk.html

JS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gtrqxitvrr.html

TS:   arr.slice(1, 4);
来源：http://hz.ivvv.top/gtqrrtuokq.html

Java: list.subList(1, 4);
来源：http://hz.zhijiandao.cn/gtokxdveap.html

Go:   arr[1:4]
来源：http://hz.jinqigufen.top/gtxrnuhnlz.html

Ruby: arr[1, 3]
来源：http://hz.zhijiandao.cn/gtxtkdlydo.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtrukkekvx.html

[D08] 合并两个数组
来源：http://hz.jyoumei.cn/gtudxvsnjh.html

Py:   a + b;  a.extend(b)
来源：http://hz.gaohongyu789.top/gtojirpuso.html

PHP:  array_merge($a, $b);
来源：http://hz.birdmap.top/gtnmvakmjb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zycfv.cn/gtfkdqvjvl.html

TS:   [...a, ...b];
来源：http://hz.hongshengwenyu.top/gtevxfsbek.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jyoumei.cn/gtweztwjmv.html

Go:   append(a, b...)
来源：http://hz.ehwqpu.com/gtrpgqdlqt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ivvv.top/gtaakfklbh.html

C#:   a.Concat(b).ToList()
来源：http://hz.nwbrower.top/gtrhcdefkk.html

[D09] 排序（升序）
来源：http://hz.hfpthk.cn/gtpmsztqba.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gtrvmjjcdt.html

PHP:  sort($arr);
来源：http://hz.sxryk.cn/gtjlorkikq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuetiantiany.cn/gtgsygefsa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhaomingkeji.xyz/gtzorgzzkr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nwbrower.top/gtevnijnlr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cashguo.top/gtfiysfwju.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtmqcfzmma.html

C#:   list.Sort();
来源：http://hz.yangfankeji.com/gtjmnjaubm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yonumen.top/gtuoolbisy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.0kj1m.cn/gtylvdgoem.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtnixhijni.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtvinuldaj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhiwuduotai.top/gtwrcxluul.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tian-w.cn/gtumjhszwe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hfpthk.cn/gtvsxtkwdv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnqzz.top/gtkwerurdp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxuanxn.top/gtnvvgywpo.html

[D11] 反转数组
来源：http://hz.guannengcc.top/gtczpivmmd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sxryk.cn/gtwkahgqdb.html

PHP:  array_reverse($arr);
来源：http://hz.hongshengwenyu.top/gtchwrtiya.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fengsongda.top/gteqzuzydg.html

TS:   [...arr].reverse();
来源：http://hz.cdnleiting.top/gtxtmhpylq.html

Java: Collections.reverse(list);
来源：http://hz.hywenlv.cn/gtzkxrdyta.html

Go:   slices.Reverse(arr)
来源：http://hz.chenjidiqi.icu/gtypzyctiy.html

Ruby: arr.reverse
来源：http://hz.yonumen.top/gtgpyybzym.html

C#:   list.Reverse();
来源：http://hz.vqdsnc.cn/gtqqbcccrd.html

[D12] 查找元素下标
来源：http://hz.ydjk.org.cn/gtsvprcmtt.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtctyjghpl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.0kj1m.cn/gtgiokqohv.html


<!-- 参考信息 -->