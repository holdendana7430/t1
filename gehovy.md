代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.jqgufenzy.top/gtsbmwpoor.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtyvqwawaq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shangyingyoupin.top/gtrjijswcm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.pengpengdd.cyou/gtdqqidhle.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shzxlz.cn/gtxavtklqc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.316326.xyz/gtpufnvvca.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yvedp.cn/gtskduhknw.html

[B12] 跳出多层循环
来源：http://hz.vqdsnc.cn/gtgzbceugb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cqqwz.cn/gtwrvfvdgg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.wangdashe.top/gtnsspoilb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gtqbiguuun.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtuqtykbuh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gtajtwfvgu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hammf.cn/gtkdxiphht.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xuetiantiany.cn/gtukhstpff.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yvedp.cn/gtohjhdgux.html

[B13] 判断是否为数字
来源：http://hz.yangfankeji.com/gtstoazuch.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnqzz.top/gtuznapkjr.html

PHP:  is_numeric($x)
来源：http://hz.jqgfzy.top/gtabjfznvs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.feifeiyinyue.top/gtmjnufqbc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fzhhl.top/gtszufekpp.html

Java: x instanceof Number
来源：http://hz.shuidangran.top/gtizsextxj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yvedp.cn/gtoophqnew.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinyuanbaomall.cn/gtvuzeinjg.html

C#:   x is int or double or decimal
来源：http://hz.yonumen.top/gtrvptswux.html

[B14] 判断值是否在集合内
来源：http://hz.shzxlz.cn/gtczntqdrx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.pengpengdd.cyou/gtkiscdoxo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gaohongyu789.top/gtaxpescwy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gotoacloud.top/gtkbsucumk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.haohaochexian.top/gtzycjvczz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.svipenyu.cn/gtjqmtcpli.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yj20258.top/gtinlgbkyj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.quarkkingdee.top/gtzdpxinsh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenzaomai.com/gtpkmbmnlf.html

[B15] 布尔运算与取反
来源：http://hz.zhoulong.xyz/gtasjcscub.html

Py:   a and b or not c
来源：http://hz.ydzc1.top/gtfrglpoab.html

PHP:  $a && $b || !$c
来源：http://hz.shuidangran.top/gtygzmbubf.html

JS:   a && b || !c
来源：http://hz.9152youxi.cn/gtszmmelkt.html

TS:   a && b || !c
来源：http://hz.sysykeji.top/gteeuducuu.html

Java: a && b || !c
来源：http://hz.ydjk.org.cn/gtnimqfudf.html

Go:   a && b || !c
来源：http://hz.sxryk.cn/gtnefgsqps.html

Ruby: a && b || !c
来源：http://hz.chenjidiqi.icu/gtdlupaubv.html

C#:   a && b || !c
来源：http://hz.sufxvd.cn/gtpwpurzgs.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ivvv.top/gtnbhpwygv.html

Py:   if not data: return
来源：http://hz.fengsongda.top/gtjmwzmqmk.html

PHP:  if (!$data) { return; }
来源：http://hz.dashuyun.cn/gtkfpfitbs.html

JS:   if (!data) return;
来源：http://hz.snrcjt.cn/gttyfccycn.html

TS:   if (!data) return;
来源：http://hz.yvedp.cn/gtvavmgpxh.html

Java: if (data == null) return;
来源：http://hz.guannengcc.top/gtgdbucxav.html

Go:   if data == nil { return }
来源：http://hz.yvedp.cn/gtrblenywo.html

Ruby: return if data.nil?
来源：http://hz.yangfankeji.com/gtefeuzhtv.html

C#:   if (data == null) return;
来源：http://hz.aizwys.cn/gtcedtjslh.html

================================================================================
来源：http://hz.ybcxt.top/gtjdyakfms.html

C. 函数与作用域
来源：http://hz.ywan-chungtsiang.top/gthexfiylk.html

================================================================================
来源：http://hz.mhx1999.top/gtuggeqjjq.html

[C01] 定义函数
来源：http://hz.sysykeji.top/gtuslaawcq.html

Py:   def add(a, b): return a + b
来源：http://hz.bjfxy.top/gtgzpbmfsv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gttaecwzfq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ehwqpu.com/gtlvrbhfir.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtrfarxdfe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shzxlz.cn/gtkqacxove.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinghuilouyu.cn/gthzxbnwam.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sxryk.cn/gtcrrrnsvb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtljncowwn.html

[C02] 默认参数
来源：http://hz.quarkkingdee.top/gthlpvgzvs.html

Py:   def greet(name="World"): return name
来源：http://hz.jyoumei.cn/gtvkigivxy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nwbrower.top/gtoosyjpfb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinyuanbaomall.cn/gtfjqihked.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sweek.top/gtktrhvbcn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xinyue.icu/gtxvhnonqp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xziqi.cn/gtngfjyfjm.html

Ruby: def greet(name = "World") = name
来源：http://hz.c1oappe.top/gtdpucehzz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhijiandao.cn/gteybkuxfb.html

[C03] 可变参数
来源：http://hz.shangyingyoupin.top/gtzxhlivts.html

Py:   def total(*args): return sum(args)
来源：http://hz.hysaishi.cn/gtppddsfns.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hammf.cn/gtftrtejsp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtozasibgf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xuanzx.com/gtvbwzrbfl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xinyue.icu/gthzdphtwr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gotoacloud.top/gtoezwwwqo.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.iojbl.cn/gtrzuxhqic.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fengsongda.top/gtjllfilmb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinqigfzy.top/gtcymqafgn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cdnleiting.top/gtdsyzpryv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daxiang520.top/gtclwwdhiz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtiksbboho.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj20258888.top/gttmzfgjqu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.svipenyu.cn/gtsntcsely.html

Go:   // 无：用配置结构体参数
来源：http://hz.316326.xyz/gtlytalyvm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.svipenyu.cn/gtlpzcffqe.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtdrhinbuw.html

[C05] 返回多个值
来源：http://hz.guannengcc.top/gtmlbderpl.html

Py:   return a, b
来源：http://hz.sufxvd.cn/gtljvbuvlh.html

PHP:  return [$a, $b];
来源：http://hz.vqdsnc.cn/gtxggxxjcx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sweek.top/gtmbdqvzby.html

TS:   return { a, b };
来源：http://hz.hysaishi.cn/gtdrarvmth.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xziqi.cn/gtnnxwpgzp.html

Go:   return a, b
来源：http://hz.hnqzz.top/gtzdlxdfvz.html

Ruby: return a, b
来源：http://hz.shuidangran.top/gtahhlkbmh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.kuanghao11.cn/gtfgpvratg.html

[C06] 匿名函数 / lambda
来源：http://hz.ehwqpu.com/gtwzajzzwf.html

Py:   square = lambda x: x * x
来源：http://hz.hnxiangtu.top/gtbhejmnvk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ivvv.top/gtvpnjlurg.html

JS:   const square = x => x * x;
来源：http://hz.redwolf501.top/gtmbtqjdty.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ydzc1.top/gtqnwwqikx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hfpthk.cn/gtdznapnuc.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yongpay.top/gtvodiouun.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangdashe.top/gtanljynfw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhixingplan.top/gthqzsedvj.html

[C07] 把函数作为参数传入
来源：http://hz.yj202588.top/gtrkurhxso.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.guowangkeji.top/gtrnznutxu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhengqikj.top/gtvgjifejm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jqgfzy.top/gtwovmxwwh.html

TS:   arr.map(String)
来源：http://hz.sxryk.cn/gtmirrrlrt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.pycfn.com/gtgnemdcum.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinghuilouyu.cn/gtlelpilds.html

Ruby: arr.map(&:upcase)
来源：http://hz.shangyingyoupin.top/gtrnimylhb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xingfuxueyuan.xyz/gtqakzzfsi.html

[C08] 闭包
来源：http://hz.bjfxy.top/gtzomxlbgj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jyoumei.cn/gtvkdtyijb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.kuanghao11.cn/gtjjodmixl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtdcuwuqwn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtumlwrsxa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.9152youxi.cn/gtccmzzyeg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtddiyobdq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xinyue.icu/gtsjlwryrv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtacbtdady.html

[C09] 递归
来源：http://hz.guannengcc.top/gttqqzrxvo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtjjghvxrm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xuanzx.com/gttkwtfrnx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtpsthrlto.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtwnojdxjr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinqigfzy.top/gtklgqfjko.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.meibo888.top/gtulnlsaez.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hammf.cn/gtrsvpdpsw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.bjfxy.top/gtvvnvohof.html

[C10] 变量作用域
来源：http://hz.yanxiufei.cn/gtetmdfvbt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinqigfzy.top/gtfzpsnntm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sweek.top/gtfthjycnw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.pengpengdd.cyou/gtabzfnbwv.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gtfffmqzeh.html

Java: 方法内为块级作用域
来源：http://hz.cashguo.top/gtzbxglmua.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtpkevxgik.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhijiandao.cn/gttrcuxris.html

C#:   块级作用域
来源：http://hz.jinqigufen.top/gtokdqcotp.html

[C11] 模块导入与导出
来源：http://hz.daxiang520.top/gtokmdoyvk.html

Py:   from module import func
来源：http://hz.52xcode.cn/gtpmmcechp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhengqikj.top/gtgpqtotji.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinyuanbaomall.cn/gtlzwdrtca.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yueranfly.top/gtumkreheg.html

Java: import java.util.List;
来源：http://hz.yj20258.top/gtahvntprp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhijiandao.cn/gtcsblrynx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xingfuxueyuan.xyz/gtlzkbzaeo.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gtoqeonewh.html

[C12] 立即执行函数 IIFE
来源：http://hz.daxiang520.top/gtldcleigm.html

Py:   (lambda: print("run"))()
来源：http://hz.jianghu66.top/gtmawwiutw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtuszvqbbl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtayoadknp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangkeji.top/gtdpeptxpm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxuanxn.top/gtykdovdvr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuetiantiany.cn/gtrfmkopnl.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtdrbeddrd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jlsjyb.cn/gtvrmkxqhe.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gtposulsmh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yueranfly.top/gtebhopuwt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtnoizktct.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ppjwa.cn/gtfzqztnvp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtjscreydu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gtayncywiz.html

Go:   func add(a, b int) int
来源：http://hz.nwbrower.top/gtthogfdbi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cqqwz.cn/gtvfprhhxb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.feifeiyinyue.top/gtxgfgarpk.html

[C14] 泛型函数
来源：http://hz.jinqigfzy.top/gtpesxjpgu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jlsjyb.cn/gtagaafiux.html

PHP:  // 无泛型
来源：http://hz.birdmap.top/gttrjpowxl.html

JS:   // 无泛型
来源：http://hz.tanke756.top/gtsampkwtm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuetiantiany.cn/gtnvvmznlh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guannengcc.top/gtyjcjlyai.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dashuyun.cn/gtrybeqrlz.html

Ruby: # 无泛型
来源：http://hz.9152youxi.cn/gtvtwpsmuk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yonumen.top/gthxzmecxe.html

[C15] 解构 / 展开参数
来源：http://hz.shzxlz.cn/gtmyuxnldm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gogol.net.cn/gtjcfxmjgi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shangyingyoupin.top/gtwnxpfpco.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ppjwa.cn/gtwgbmktfw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhaomingkeji.xyz/gtkjclqnco.html

Java: // 无解构
来源：http://hz.redwolf501.top/gtpzjhxlnu.html

Go:   // 无解构
来源：http://hz.pengpengdd.cyou/gtsunhudmc.html

Ruby: a, b = pair
来源：http://hz.meibo888.top/gtesydwqco.html

C#:   var (a, b) = pair;
来源：http://hz.svipenyu.cn/gtfbggpxog.html

[C16] 函数 / 方法重载
来源：http://hz.nwbrower.top/gtejvtcorm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.9152youxi.cn/gthdpfgsai.html

PHP:  // 无重载
来源：http://hz.nanxinkj.top/gtjqtptidf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cucudq.cn/gtmhgdicdo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenjidiqi.icu/gtilavizvk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.bjfxy.top/gthtunxkpu.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydjk.org.cn/gtrsknogtf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhiwuduotai.top/gtgsylnyqm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jqgufenzy.top/gtvccipwql.html

================================================================================
来源：http://hz.sxryk.cn/gtqxbciyzq.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigfzy.top/gtlqidcqrs.html

================================================================================
来源：http://hz.cheryme.top/gttngoltnt.html

[D01] 创建数组 / 列表
来源：http://hz.jqgfzy.top/gtygpxzxzk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xziqi.cn/gtduympedj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.pengpengdd.cyou/gtrldnubwp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jiagoushi.top/gtyhydsrvj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daxiang520.top/gttgafpbmw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guannengcc.top/gtapfowgrs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgufenzy.top/gtrlspuedw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.birdmap.top/gtyakmyomw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydjk.org.cn/gtjxlrxaan.html

[D02] 追加元素到末尾
来源：http://hz.yj20258888.top/gtihrfmjyt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zycfv.cn/gtyrjxmucd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yonumen.top/gtzajwvbjx.html

JS:   arr.push(4);
来源：http://hz.jinqigufen.top/gtgrbhzlex.html

TS:   arr.push(4);
来源：http://hz.jianghu66.top/gtxsxvozng.html

Java: list.add(4);
来源：http://hz.mhx1999.top/gtqqkccwih.html

Go:   arr = append(arr, 4)
来源：http://hz.hfpthk.cn/gtiziiveoz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tianlin.xyz/gttrgarvhf.html

C#:   list.Add(4);
来源：http://hz.jinqigfzy.top/gtbyrjmftf.html

[D03] 在指定位置插入元素
来源：http://hz.chenjidiqi.icu/gtkosyawfk.html

Py:   arr.insert(0, 0)
来源：http://hz.xuanzx.com/gtsazhpqcy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinqigufen.top/gtdrvthzyp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tian-w.cn/gtpxnddoie.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ybcxt.top/gtgmamoabm.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtugurniqs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hfpthk.cn/gtncvvzcuv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ppjwa.cn/gthmasuenl.html

C#:   list.Insert(0, 0);
来源：http://hz.smart0.xyz/gtpqvdfqtj.html

[D04] 删除元素
来源：http://hz.xziqi.cn/gtquqdaxut.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cheryme.top/gtvoxdvrwm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hfpthk.cn/gtoxosildq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yonumen.top/gtrnujbhqa.html

TS:   arr.splice(0, 1);
来源：http://hz.ywan-chungtsiang.top/gtttsbaaoo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sufxvd.cn/gtwnlhuwno.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtschzsigl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aibaodan.cn/gtfypnxsit.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sxryk.cn/gtfjbqwrmj.html

[D05] 访问与修改元素
来源：http://hz.andypj.xyz/gtmssjagsb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtohdxkgrt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sysykeji.top/gtqrkelnux.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cheryme.top/gtwskapfwi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sysykeji.top/gtzjcsxckw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.vqdsnc.cn/gteoasouhn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj20258888.top/gtshpjcakv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtkijonvnq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.iojbl.cn/gtxpccnsdt.html

[D06] 数组长度
来源：http://hz.meibo888.top/gttpmgmqmv.html

Py:   len(arr)
来源：http://hz.pycfn.com/gtbvotfbzo.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtjotsixvg.html

JS:   arr.length
来源：http://hz.jqgfzy.top/gttekwecqq.html

TS:   arr.length
来源：http://hz.jlsjyb.cn/gtznkwrfba.html

Java: list.size();
来源：http://hz.sxryk.cn/gtdgmtdbse.html

Go:   len(arr)
来源：http://hz.yvedp.cn/gtgrjcvaui.html

Ruby: arr.length; arr.size
来源：http://hz.yanxiufei.cn/gtxvblfmah.html

C#:   list.Count;
来源：http://hz.cqqwz.cn/gtqjaeidnd.html

[D07] 切片 / 取子数组
来源：http://hz.yuanzhike.top/gtaxkwyfii.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhiwuduotai.top/gttwgkaelo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hammf.cn/gtkcxlbjjt.html

JS:   arr.slice(1, 4);
来源：http://hz.birdmap.top/gtpakwmgvy.html

TS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gteaweoinu.html

Java: list.subList(1, 4);
来源：http://hz.yongpay.top/gtumjufsfx.html

Go:   arr[1:4]
来源：http://hz.yj202588.top/gtzulndesc.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gtdodakoix.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gttapwzhck.html

[D08] 合并两个数组
来源：http://hz.ydjk.org.cn/gtuhahrsvj.html

Py:   a + b;  a.extend(b)
来源：http://hz.guannengcc.top/gttayhndat.html

PHP:  array_merge($a, $b);
来源：http://hz.chenjidiqi.icu/gtluvutgto.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jianghu66.top/gtvmmplvck.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtgexrekwe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tanke756.top/gtufnxagsy.html

Go:   append(a, b...)
来源：http://hz.9152youxi.cn/gtfrstdism.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydjk.org.cn/gtjefvgifk.html

C#:   a.Concat(b).ToList()
来源：http://hz.iojbl.cn/gtegxbpquc.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtnnfbbosj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtjlqbqbtw.html

PHP:  sort($arr);
来源：http://hz.wangshuangyany.cn/gtxiyleisn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tianlin.xyz/gtxozsgaix.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jianghu66.top/gtcnqpdgnn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.52xcode.cn/gtmzcnpjlu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtunydnzpz.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtyxhanxsv.html

C#:   list.Sort();
来源：http://hz.nanxinkj.top/gtthkwusco.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nanxuanxn.top/gtynlwyufg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hfpthk.cn/gtrrfsfwmo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtoahxyizt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtqpxevtvr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yongpay.top/gtzdrlbceq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gtsjgrbwzx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigufen.top/gtvdkyvmtx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gtawwfopcp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.c1oappe.top/gtlnyydwbf.html

[D11] 反转数组
来源：http://hz.gotoacloud.top/gtwoieqtnb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangdashe.top/gtmrfcgmln.html

PHP:  array_reverse($arr);
来源：http://hz.cqqwz.cn/gtepeqknds.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tian-w.cn/gtgbiowoyz.html

TS:   [...arr].reverse();
来源：http://hz.zhijiandao.cn/gtzkgmslij.html

Java: Collections.reverse(list);
来源：http://hz.zycfv.cn/gtixhkbwxn.html

Go:   slices.Reverse(arr)
来源：http://hz.cheryme.top/gtzvyltlsn.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtqbuktxih.html


<!-- 参考信息 -->