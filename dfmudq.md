代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.aizwys.cn/gtybmlupkz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangshuangyany.cn/gtdzmopqpm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtnpwpfjbw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.haohaochexian.top/gtviywhzco.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.c1oappe.top/gtlmlomsrv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xziqi.cn/gtfkbxzbhm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhiwuduotai.top/gtfzkmqqhp.html

[B12] 跳出多层循环
来源：http://hz.kuanghao11.cn/gtrfqyxqhs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.daria6918.cn/gtreclquzb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sysykeji.top/gtoymloaxp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtpfxzehta.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenzaomai.com/gtutmzaukz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtqviihhjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.0kj1m.cn/gtkzfijkdb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhongyouzk.top/gtuvifsmnv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ydzc1.top/gtnwsmrhxq.html

[B13] 判断是否为数字
来源：http://hz.mhx1999.top/gtmcoynvns.html

Py:   isinstance(x, (int, float))
来源：http://hz.yueranfly.top/gthvsdunxc.html

PHP:  is_numeric($x)
来源：http://hz.nanxinkj.top/gtaaryzggs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtjcfuocfe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gtpzfjhkaq.html

Java: x instanceof Number
来源：http://hz.ywan-chungtsiang.top/gtxgedtitg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shanyushiyangkeji.top/gthttnnwwz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hysaishi.cn/gteiqoyxrm.html

C#:   x is int or double or decimal
来源：http://hz.birdmap.top/gtnoppivxa.html

[B14] 判断值是否在集合内
来源：http://hz.ywan-chungtsiang.top/gtsauzkaqt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zycfv.cn/gtevccwdgd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.guannengcc.top/gtrngmqyni.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.aizwys.cn/gtluprkpgv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jiagoushi.top/gtkcehexxq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtpiedwyoi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.mhx1999.top/gtjhntgsjg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yvedp.cn/gtlfltflqp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.havefunace.top/gtengacofe.html

[B15] 布尔运算与取反
来源：http://hz.cashguo.top/gtksglujsg.html

Py:   a and b or not c
来源：http://hz.daxiang520.top/gthdsoapdu.html

PHP:  $a && $b || !$c
来源：http://hz.hongshengwenyu.top/gtuspqujxm.html

JS:   a && b || !c
来源：http://hz.nanxuanxn.top/gtfhyygprl.html

TS:   a && b || !c
来源：http://hz.yuanzhike.top/gtqmcrezxv.html

Java: a && b || !c
来源：http://hz.svipenyu.cn/gtqfpdietk.html

Go:   a && b || !c
来源：http://hz.jianghu66.top/gtmcsctxwc.html

Ruby: a && b || !c
来源：http://hz.mhx1999.top/gthoulodlp.html

C#:   a && b || !c
来源：http://hz.ppjwa.cn/gthmfhfpia.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yuxming.cn/gtzplfrvwe.html

Py:   if not data: return
来源：http://hz.jyoumei.cn/gtolsrfpvy.html

PHP:  if (!$data) { return; }
来源：http://hz.bjfxy.top/gtaxciwaul.html

JS:   if (!data) return;
来源：http://hz.vqdsnc.cn/gtnikhsifq.html

TS:   if (!data) return;
来源：http://hz.9152youxi.cn/gtccnbtwvu.html

Java: if (data == null) return;
来源：http://hz.daria6918.cn/gtnzckggjl.html

Go:   if data == nil { return }
来源：http://hz.feifeiyinyue.top/gttsnlovcm.html

Ruby: return if data.nil?
来源：http://hz.hywenlv.cn/gtbzbmxpgu.html

C#:   if (data == null) return;
来源：http://hz.hnxiangtu.top/gtruqbhthd.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtgcxufjma.html

C. 函数与作用域
来源：http://hz.yuanzhike.top/gtwjbcllrf.html

================================================================================
来源：http://hz.aizwys.cn/gtnmhzvqac.html

[C01] 定义函数
来源：http://hz.tian-w.cn/gtzttdewtj.html

Py:   def add(a, b): return a + b
来源：http://hz.daria6918.cn/gtykrftxkm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtlipohrgq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yonumen.top/gtwcpwdhre.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sysykeji.top/gtuawrdjjj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtclhwevqj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gogol.net.cn/gtcszvopmp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ivvv.top/gtlerwayab.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtgtczgvbk.html

[C02] 默认参数
来源：http://hz.chenzaomai.com/gtijqulppp.html

Py:   def greet(name="World"): return name
来源：http://hz.ydjk.org.cn/gtejrruwqy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinqigufen.top/gtykfojokd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.aibaodan.cn/gtoyefmzma.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gtpvsiuhpt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.kuanghao11.cn/gttytflieo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhaomingkeji.xyz/gtjcygzxjy.html

Ruby: def greet(name = "World") = name
来源：http://hz.cucudq.cn/gtwapifqwa.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xingfuxueyuan.xyz/gtzyuevver.html

[C03] 可变参数
来源：http://hz.birdmap.top/gtdrwvvwjb.html

Py:   def total(*args): return sum(args)
来源：http://hz.yonumen.top/gtemdthcrl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nwbrower.top/gtaxlszrwf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtfwjkxelj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yonumen.top/gtucfczugi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenjidiqi.icu/gtwjoipbhg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtnsdqscyr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gaohongyu789.top/gtwzpwxfpj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.snrcjt.cn/gttfghdyxu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydjk.org.cn/gtykwsepcq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuetiantiany.cn/gtpzadxziv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.wangshuangyany.cn/gtwnsxlwid.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtrirvoowj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ppjwa.cn/gtfziwejbh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhiwuduotai.top/gtmcxncayi.html

Go:   // 无：用配置结构体参数
来源：http://hz.gzhubu.top/gttzwizlsq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gthryrvgkt.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtvtzeyeza.html

[C05] 返回多个值
来源：http://hz.zhaomingkeji.xyz/gtzsjeixfy.html

Py:   return a, b
来源：http://hz.nanxuanxn.top/gtjtjwmthn.html

PHP:  return [$a, $b];
来源：http://hz.dashuyun.cn/gtmeyvufrd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aibaodan.cn/gtykbewtbe.html

TS:   return { a, b };
来源：http://hz.gzhubu.top/gtfyoswctz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangkeji.top/gtivimkpdb.html

Go:   return a, b
来源：http://hz.ydzc1.top/gtbbwlmmhr.html

Ruby: return a, b
来源：http://hz.sweek.top/gtwvpgkozw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.smart0.xyz/gtjhdctvaj.html

[C06] 匿名函数 / lambda
来源：http://hz.jqgufenzy.top/gtvbotxwpw.html

Py:   square = lambda x: x * x
来源：http://hz.hongshengwenyu.top/gtaqqskeeb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.feifeiyinyue.top/gtqldqefkz.html

JS:   const square = x => x * x;
来源：http://hz.nanxinkj.top/gtigdtmveo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nanxinkj.top/gtarkcvbde.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xylfe.cn/gtizjcovfw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daria6918.cn/gtconwbfge.html

Ruby: square = ->(x) { x * x }
来源：http://hz.c1oappe.top/gthsuoqrbj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgfzy.top/gtcfkplrbc.html

[C07] 把函数作为参数传入
来源：http://hz.hywenlv.cn/gtmzbidpmq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenlongwang.top/gtgvxgayxg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sweek.top/gtfguqznxs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenlongwang.top/gtfxpifuoe.html

TS:   arr.map(String)
来源：http://hz.jqgfzy.top/gthfaeuszc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuanzhike.top/gttciuigon.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydzc1.top/gtgexmaakd.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gttbtvwlvx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.52xcode.cn/gtchuenejw.html

[C08] 闭包
来源：http://hz.ppjwa.cn/gtkkaajhss.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pengpengdd.cyou/gtvhkabmhb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jlsjyb.cn/gtnvyerwve.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtjioeukzr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtwjpeuwwr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nwbrower.top/gtmiogibra.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuetiantiany.cn/gtjijcawdt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinyuanbaomall.cn/gtdrdfjrgk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sufxvd.cn/gtmqinyuap.html

[C09] 递归
来源：http://hz.birdmap.top/gtempuapmk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtkwocijrq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtbwhzixmy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gttvgnqhns.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtaidevfuq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.9152youxi.cn/gtiammieqt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dianchejie.cn/gtezgdrsdf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtnyakkuxs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.svipenyu.cn/gtwghddzci.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtftusipnm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yonumen.top/gtyujpbdqf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cucudq.cn/gtmtllolye.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cqqwz.cn/gtzdautujs.html

TS:   同 JS
来源：http://hz.gotoacloud.top/gtnwyizbpu.html

Java: 方法内为块级作用域
来源：http://hz.yanxiufei.cn/gtnqbdlpeg.html

Go:   花括号块级作用域
来源：http://hz.cashguo.top/gtxocvxvje.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgfzy.top/gtcysnzmyl.html

C#:   块级作用域
来源：http://hz.cashguo.top/gtiknzexbg.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gtilmzjgzk.html

Py:   from module import func
来源：http://hz.fzhhl.top/gtershwxcj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhengqikj.top/gtevjyubbh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gzhubu.top/gtyjaoehkn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.nanxinkj.top/gtialtrybf.html

Java: import java.util.List;
来源：http://hz.ivvv.top/gtdfvoffbk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.dashuyun.cn/gtlosmgurc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gaohongyu789.top/gtmtlkcwqm.html

C#:   using System.Text;
来源：http://hz.smart0.xyz/gtqkspoaxh.html

[C12] 立即执行函数 IIFE
来源：http://hz.jianghu66.top/gtetjubczr.html

Py:   (lambda: print("run"))()
来源：http://hz.nanxinkj.top/gtgtxrxwbg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.quarkkingdee.top/gthfmjvial.html

JS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtzshysfpf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtmkmfqgmr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gotoacloud.top/gttbiullte.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhixingplan.top/gtfyravcsy.html

Ruby: -> { puts "run" }.call
来源：http://hz.daria6918.cn/gtxoafesbq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.snrcjt.cn/gtsrtckueg.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtcsxskdda.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shanyushiyangkeji.top/gtncrtoxih.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtwaysqcaq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xziqi.cn/gtquspqauk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtyrqxigkb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtzuyfzzcl.html

Go:   func add(a, b int) int
来源：http://hz.xinyue.icu/gtvpotdaun.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.vqdsnc.cn/gtmjcmjaom.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.kuanghao11.cn/gtxqhknflq.html

[C14] 泛型函数
来源：http://hz.havefunace.top/gtyiwgqruf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tian-w.cn/gtofzqgqyf.html

PHP:  // 无泛型
来源：http://hz.jinqigufen.top/gtrvzyymyo.html

JS:   // 无泛型
来源：http://hz.ybcxt.top/gtipgqnogj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gotoacloud.top/gtydldkoxn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.smart0.xyz/gtvccccehb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj20258.top/gtgapftpmg.html

Ruby: # 无泛型
来源：http://hz.zycfv.cn/gtgwfbmsqu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gtdqzjcehy.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258.top/gtkqzlrqpl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yuxming.cn/gtbrejigub.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258888.top/gtxpwhjhgm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtbclbkjga.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.havefunace.top/gtczzgoduh.html

Java: // 无解构
来源：http://hz.shangyingyoupin.top/gtyavnyiss.html

Go:   // 无解构
来源：http://hz.xylfe.cn/gtoskyeimz.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtkdhfyzqg.html

C#:   var (a, b) = pair;
来源：http://hz.yuanzhike.top/gteukzlvvb.html

[C16] 函数 / 方法重载
来源：http://hz.xuanzx.com/gtajhnqgnc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shuidangran.top/gtowpdjlsa.html

PHP:  // 无重载
来源：http://hz.jinghuilouyu.cn/gtdwxwzces.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenjidiqi.icu/gtoqobbcob.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenjidiqi.icu/gtziorbpsd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sxryk.cn/gtbveeodxn.html

Go:   // 无重载：用不同函数名
来源：http://hz.yueranfly.top/gtjyntzdbr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxuanxn.top/gtcjuotlji.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ehwqpu.com/gtfwiljetx.html

================================================================================
来源：http://hz.andypj.xyz/gtigwcoaei.html

D. 数组 / 列表 / 集合
来源：http://hz.bjfxy.top/gtdfcbauti.html

================================================================================
来源：http://hz.yuxming.cn/gtspvgahhu.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtpjhqkrya.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yongpay.top/gtzamkplgc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhaomingkeji.xyz/gtcducdzip.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shanyushiyangtech.top/gtxrvaqbpy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hammf.cn/gtpstifcyy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtcjelqzdh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yueranfly.top/gthwyvezwj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258888.top/gtxjaghwbw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dashuyun.cn/gtxtxyqpvi.html

[D02] 追加元素到末尾
来源：http://hz.xziqi.cn/gtaoveabfc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydzc1.top/gtpfzqrwqf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gogol.net.cn/gtglgydrwq.html

JS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtyioxnxvl.html

TS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtznwghjqz.html

Java: list.add(4);
来源：http://hz.gzhubu.top/gtjknzqkuc.html

Go:   arr = append(arr, 4)
来源：http://hz.wangdashe.top/gtslqpsocf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shanyushiyangtech.top/gtrrjzfnsa.html

C#:   list.Add(4);
来源：http://hz.zhengqikj.top/gtbfoclusr.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtglchsvcu.html

Py:   arr.insert(0, 0)
来源：http://hz.yangfankeji.com/gtbidxdjmh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yueranfly.top/gtxgtzgyys.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.redwolf501.top/gtglfoeegn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydjk.org.cn/gtwjuxowpo.html

Java: list.add(0, 0);
来源：http://hz.tanke756.top/gthkbprqtd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ppjwa.cn/gtilwzfnzy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.mhx1999.top/gthjbawlti.html

C#:   list.Insert(0, 0);
来源：http://hz.gotoacloud.top/gtwfnqscxf.html

[D04] 删除元素
来源：http://hz.52xcode.cn/gtdfqfeiep.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xylfe.cn/gtwypfmmmw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.birdmap.top/gtlzphluod.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sweek.top/gtnlprkgpu.html

TS:   arr.splice(0, 1);
来源：http://hz.wangshuangyany.cn/gttobpegnf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhengqikj.top/gtvetxellv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xingfuxueyuan.xyz/gtvguenbtm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhixingplan.top/gtaxllaqmg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangtech.top/gtnzbslqwv.html

[D05] 访问与修改元素
来源：http://hz.gotoacloud.top/gtuiviqxqh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtcciihdmc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtaqapjzev.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtmrynqyhm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cqqwz.cn/gtxkkjnznd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nwbrower.top/gtxyhbpxse.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtyijeifnx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtfrzispgz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hammf.cn/gtpgpnizvz.html

[D06] 数组长度
来源：http://hz.xuetiantiany.cn/gtjqzmffkb.html

Py:   len(arr)
来源：http://hz.pycfn.com/gtvsvdhuqf.html

PHP:  count($arr);
来源：http://hz.wangshuangyany.cn/gtsmwtpviy.html

JS:   arr.length
来源：http://hz.fengsongda.top/gtvascemjv.html

TS:   arr.length
来源：http://hz.guannengcc.top/gtappoujkw.html

Java: list.size();
来源：http://hz.cucudq.cn/gtstubfspu.html

Go:   len(arr)
来源：http://hz.bjfxy.top/gtdxawkerz.html

Ruby: arr.length; arr.size
来源：http://hz.hnxiangtu.top/gtjvbogouj.html

C#:   list.Count;
来源：http://hz.guannengcc.top/gtbyhjyorq.html

[D07] 切片 / 取子数组
来源：http://hz.52xcode.cn/gtepnszuqu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.guannengcc.top/gtjeapnemb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.9152youxi.cn/gtsmpggnua.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtkmvthbtd.html

TS:   arr.slice(1, 4);
来源：http://hz.yueranfly.top/gtmtbbnknd.html

Java: list.subList(1, 4);
来源：http://hz.dianchejie.cn/gtchmtrifp.html

Go:   arr[1:4]
来源：http://hz.yanxiufei.cn/gtuklqigvg.html

Ruby: arr[1, 3]
来源：http://hz.cashguo.top/gtvhopvgye.html

C#:   list.GetRange(1, 3);
来源：http://hz.yanxiufei.cn/gtdoacfiik.html

[D08] 合并两个数组
来源：http://hz.hongshengwenyu.top/gtzmwujwyo.html

Py:   a + b;  a.extend(b)
来源：http://hz.yanxiufei.cn/gtnyftstab.html

PHP:  array_merge($a, $b);
来源：http://hz.zycfv.cn/gtzkjysbaa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guannengcc.top/gtfutkvlay.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtnuzrjvmu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinghuilouyu.cn/gtgabxbkav.html

Go:   append(a, b...)
来源：http://hz.pengpengdd.cyou/gtjowqepwz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.smart0.xyz/gtesjcfouz.html

C#:   a.Concat(b).ToList()
来源：http://hz.wangdashe.top/gtghgptdcp.html

[D09] 排序（升序）
来源：http://hz.cdnleiting.top/gtkalnmbnh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gttlpyzoaq.html

PHP:  sort($arr);
来源：http://hz.gzhubu.top/gtadahudmy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gzhubu.top/gtjtcjaxcm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sysykeji.top/gtytcwkswz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.svipenyu.cn/gthqihxstc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhaomingkeji.xyz/gtygcenlcc.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtixanwjlt.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gtvaifwhym.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.kuanghao11.cn/gtnqulmsca.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jqgfzy.top/gtkpydxujw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.andypj.xyz/gtrqfpepny.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtimcjwxui.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtveqlbseq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhaomingkeji.xyz/gttvyszeir.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtsddnqkmg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gtkeonxsxo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tianlin.xyz/gtwrpaamcr.html

[D11] 反转数组
来源：http://hz.ybcxt.top/gtahgkftbt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.smart0.xyz/gtclntvxtt.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gtfwzxoiyj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dianchejie.cn/gtlfmaeswd.html

TS:   [...arr].reverse();
来源：http://hz.daxiang520.top/gtidcnswng.html

Java: Collections.reverse(list);
来源：http://hz.zhongyouzk.top/gteepltqjq.html

Go:   slices.Reverse(arr)
来源：http://hz.aibaodan.cn/gtgalxdoyy.html

Ruby: arr.reverse
来源：http://hz.316326.xyz/gtzmqfmrfm.html


<!-- 参考信息 -->