代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhongyouzk.top/gtpzfactkj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pycfn.com/gtrijnlxvy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guowangkeji.top/gtkkuwrmab.html

[B12] 跳出多层循环
来源：http://hz.ybcxt.top/gtgauiucks.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jlsjyb.cn/gtmeuarsls.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtqijcwsxm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gtebjvopql.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.feifeiyinyue.top/gtaucputga.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtylpjpxma.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xuetiantiany.cn/gtotpquqrd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.c1oappe.top/gtsoupejny.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hongshengwenyu.top/gtviazlfoa.html

[B13] 判断是否为数字
来源：http://hz.shanyushiyangtech.top/gtxmkqxvuw.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenzaomai.com/gtdbesukso.html

PHP:  is_numeric($x)
来源：http://hz.cdnleiting.top/gtvimnbxyy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.quarkkingdee.top/gtmxxbcjbj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gtqsqaclmf.html

Java: x instanceof Number
来源：http://hz.aibaodan.cn/gtodxcqnhx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ehwqpu.com/gtlmktoqub.html

Ruby: x.is_a?(Numeric)
来源：http://hz.fzhhl.top/gthigzdzbe.html

C#:   x is int or double or decimal
来源：http://hz.wangdashe.top/gtvnmlgvck.html

[B14] 判断值是否在集合内
来源：http://hz.316326.xyz/gtczbfstkw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.svipenyu.cn/gtuapapszk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xylfe.cn/gtnlrrfijn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigfzy.top/gtizsqpnao.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.daria6918.cn/gthtdqmvhm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tianlin.xyz/gtvgapatun.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhoulong.xyz/gtumyxlgqe.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhoulong.xyz/gtcwzlyhzl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cdnleiting.top/gtyzwswete.html

[B15] 布尔运算与取反
来源：http://hz.xziqi.cn/gtdgiscdkr.html

Py:   a and b or not c
来源：http://hz.zhongyouzk.top/gtrbhjtedm.html

PHP:  $a && $b || !$c
来源：http://hz.dashuyun.cn/gtrsodyils.html

JS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtihsqlkig.html

TS:   a && b || !c
来源：http://hz.hfpthk.cn/gtebcnlklb.html

Java: a && b || !c
来源：http://hz.jianghu66.top/gtibfncxij.html

Go:   a && b || !c
来源：http://hz.mhx1999.top/gtazdhmrob.html

Ruby: a && b || !c
来源：http://hz.xinyue.icu/gtuttehpvq.html

C#:   a && b || !c
来源：http://hz.dashuyun.cn/gtqytufskr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhijiandao.cn/gtpwkpqgks.html

Py:   if not data: return
来源：http://hz.shangyingyoupin.top/gtnsurijyp.html

PHP:  if (!$data) { return; }
来源：http://hz.daxiang520.top/gtuhpkvsrx.html

JS:   if (!data) return;
来源：http://hz.feifeiyinyue.top/gtzmsegkwa.html

TS:   if (!data) return;
来源：http://hz.zhengqikj.top/gtocgjsubw.html

Java: if (data == null) return;
来源：http://hz.tanke756.top/gtzqdztdku.html

Go:   if data == nil { return }
来源：http://hz.cucudq.cn/gtykpkizop.html

Ruby: return if data.nil?
来源：http://hz.yanxiufei.cn/gtulxfopkl.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtkokvoosl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbxpmsavc.html

C. 函数与作用域
来源：http://hz.jlsjyb.cn/gtazfbjlom.html

================================================================================
来源：http://hz.svipenyu.cn/gtyphpmbsz.html

[C01] 定义函数
来源：http://hz.mhx1999.top/gtksvtrynr.html

Py:   def add(a, b): return a + b
来源：http://hz.ybcxt.top/gtxjcyfokl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtpebxxwgx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sweek.top/gtqhbtrecb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gtsipsnjxk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtmzgzdnhk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gaohongyu789.top/gtlbsihmbl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sysykeji.top/gtbcpmdqzg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtmwnlyybr.html

[C02] 默认参数
来源：http://hz.sufxvd.cn/gtrwbrfznr.html

Py:   def greet(name="World"): return name
来源：http://hz.fzhhl.top/gtmzjrcptw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aizwys.cn/gtnxmdwrli.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cdnleiting.top/gtvbeblqiz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.kuanghao11.cn/gtbdawtoms.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yongpay.top/gttbmrurjf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sufxvd.cn/gtcjumfibb.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgufenzy.top/gtudxnteeg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinyuanbaomall.cn/gtetlprfki.html

[C03] 可变参数
来源：http://hz.hnqzz.top/gtofzoojnc.html

Py:   def total(*args): return sum(args)
来源：http://hz.xingfuxueyuan.xyz/gtyufrvvxw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.52xcode.cn/gtkwoiozlu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnxiangtu.top/gtmzgsycdm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xziqi.cn/gttmxcthzx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.svipenyu.cn/gtyelbazyp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.dianchejie.cn/gtlsmabbmg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yueranfly.top/gtoeeltvxm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.smart0.xyz/gtdshyzoqj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hammf.cn/gtmuzppjwk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.52xcode.cn/gtmvizigtr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.fengsongda.top/gtbdnlxoef.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtmqfqywnu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ydzc1.top/gtojdvqsbt.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hysaishi.cn/gtzqsrqjzw.html

Go:   // 无：用配置结构体参数
来源：http://hz.hammf.cn/gtiwadipko.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtereninte.html

C#:   f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gteoehmeff.html

[C05] 返回多个值
来源：http://hz.daria6918.cn/gtnppnpiro.html

Py:   return a, b
来源：http://hz.hnqzz.top/gtitlizdbj.html

PHP:  return [$a, $b];
来源：http://hz.gzhubu.top/gtdygllnjt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hysaishi.cn/gtspcbxbdb.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtgeuchyqj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.9152youxi.cn/gtxgmwodlw.html

Go:   return a, b
来源：http://hz.fzhhl.top/gtnxwujlxl.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtiabwkvgs.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.vqdsnc.cn/gtbwinchlx.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigufen.top/gtlyljnqau.html

Py:   square = lambda x: x * x
来源：http://hz.yangfankeji.com/gtmmhqfspg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jqgufenzy.top/gtdycnjhuk.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtilidqmlb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dianchejie.cn/gtssiyyzoi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jianghu66.top/gtvtlddejz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj20258888.top/gtdjusrjvc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.vqdsnc.cn/gtvbvtsumb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tianlin.xyz/gtcgvzlbte.html

[C07] 把函数作为参数传入
来源：http://hz.nanxuanxn.top/gtftfshrmq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yanxiufei.cn/gtmpkuoepd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gogol.net.cn/gtbtslpduk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ydzc1.top/gtqinwswik.html

TS:   arr.map(String)
来源：http://hz.haohaochexian.top/gtkzsoulfj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tian-w.cn/gtrgncemjx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenzaomai.com/gthbubujzg.html

Ruby: arr.map(&:upcase)
来源：http://hz.birdmap.top/gtvokifajy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhoulong.xyz/gtclmxxfko.html

[C08] 闭包
来源：http://hz.zhiwuduotai.top/gtqehwvlty.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangshuangyany.cn/gtkcvtegcn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aibaodan.cn/gtjcadllzl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtunlybsdw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gtcssrtavr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuetiantiany.cn/gtxgxtxstb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hywenlv.cn/gtqhhszklh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.c1oappe.top/gtjzacmjfg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtdwyvfhei.html

[C09] 递归
来源：http://hz.nanxinkj.top/gtdpwemzed.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhengqikj.top/gtnalsqzjt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.kuanghao11.cn/gtmxfhfmrq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guowangkeji.top/gtvttayktu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gthoflvutz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gaohongyu789.top/gthunasiey.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.haohaochexian.top/gtnwbgcwtj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtfzwxswbp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangkeji.top/gtyysvowlo.html

[C10] 变量作用域
来源：http://hz.feifeiyinyue.top/gtnmridrko.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.wangdashe.top/gtiapbtsex.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tianlin.xyz/gtlsjvzlnt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuanzhike.top/gtmfryrzdi.html

TS:   同 JS
来源：http://hz.wangdashe.top/gtqdxkwana.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtwitnzrba.html

Go:   花括号块级作用域
来源：http://hz.sysykeji.top/gtfhpolsmf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xziqi.cn/gtjpjwlbzt.html

C#:   块级作用域
来源：http://hz.sxryk.cn/gtoydersqv.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gtzmegmvep.html

Py:   from module import func
来源：http://hz.chenzaomai.com/gtoqkoddui.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hfpthk.cn/gtdasoowyu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.52xcode.cn/gtnhwvcesu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gogol.net.cn/gtceaseoav.html

Java: import java.util.List;
来源：http://hz.daxiang520.top/gtsizesery.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zdqjudy.top/gtjxzwarlw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgufenzy.top/gtatrihzpe.html

C#:   using System.Text;
来源：http://hz.hysaishi.cn/gtsxmeogkt.html

[C12] 立即执行函数 IIFE
来源：http://hz.shuidangran.top/gtioicojmi.html

Py:   (lambda: print("run"))()
来源：http://hz.ybcxt.top/gtiiuhvxyy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhongyouzk.top/gtpufuifwc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtdzekzcue.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtgnryaudv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xziqi.cn/gtocmxhhur.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhongyouzk.top/gtpwlckffi.html

Ruby: -> { puts "run" }.call
来源：http://hz.cdnleiting.top/gtvusobtiw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtryuptfqc.html

[C13] 类型声明 / 类型注解
来源：http://hz.bjfxy.top/gtmvzybycw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.kuanghao11.cn/gtejowdrpr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtumkcqnbh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cqqwz.cn/gtjimbrnjp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtoudpgbir.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gtqhsrozpp.html

Go:   func add(a, b int) int
来源：http://hz.chenzaomai.com/gtzmovanej.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.birdmap.top/gtmezcppnd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ybcxt.top/gtuzcmshbx.html

[C14] 泛型函数
来源：http://hz.ehwqpu.com/gtemindunk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258.top/gtegvksttt.html

PHP:  // 无泛型
来源：http://hz.yangfankeji.com/gtgrjuplzz.html

JS:   // 无泛型
来源：http://hz.zhaomingkeji.xyz/gtsbcmsncr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hysaishi.cn/gtcygwirng.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.316326.xyz/gtjvvgzpnv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinqigfzy.top/gtzivtyhyv.html

Ruby: # 无泛型
来源：http://hz.jyoumei.cn/gtvralvvey.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cdnleiting.top/gtthziblpj.html

[C15] 解构 / 展开参数
来源：http://hz.gaohongyu789.top/gtedoyminx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnqzz.top/gtrguyqewq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.snrcjt.cn/gtkxvtktbb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gtfbdsopnj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.52xcode.cn/gtitywvybo.html

Java: // 无解构
来源：http://hz.yj202588.top/gtrzmfsqes.html

Go:   // 无解构
来源：http://hz.nwbrower.top/gtuhllofxd.html

Ruby: a, b = pair
来源：http://hz.havefunace.top/gtvogatpld.html

C#:   var (a, b) = pair;
来源：http://hz.xinyue.icu/gttkrquxjj.html

[C16] 函数 / 方法重载
来源：http://hz.jlsjyb.cn/gtctuchxnc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gtyfsathre.html

PHP:  // 无重载
来源：http://hz.cqqwz.cn/gtgdrwiqwc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.feifeiyinyue.top/gttwchqhtd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daxiang520.top/gtvgdyytun.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pengpengdd.cyou/gtbmjxxlbq.html

Go:   // 无重载：用不同函数名
来源：http://hz.xziqi.cn/gtykwlkymg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gaohongyu789.top/gtxptzzwoz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shangyingyoupin.top/gtkhtfwefg.html

================================================================================
来源：http://hz.sufxvd.cn/gtfxllvvek.html

D. 数组 / 列表 / 集合
来源：http://hz.daxiang520.top/gtujrfohew.html

================================================================================
来源：http://hz.nanxuanxn.top/gtxzmhlawu.html

[D01] 创建数组 / 列表
来源：http://hz.chenjidiqi.icu/gtjkoknptq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tianlin.xyz/gthuoppmig.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shzxlz.cn/gtmcxkhdxi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.iojbl.cn/gtgperjqgt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hfpthk.cn/gtzuskgwom.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xingfuxueyuan.xyz/gtzkscjqme.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jyoumei.cn/gthcsxvuxf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.snrcjt.cn/gthaglgdai.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.iojbl.cn/gtvvazmrdj.html

[D02] 追加元素到末尾
来源：http://hz.yj202588.top/gtybtcjsnr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.meibo888.top/gtkdfpjyyt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.316326.xyz/gtpygrjjzy.html

JS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtdwmalyrb.html

TS:   arr.push(4);
来源：http://hz.hfpthk.cn/gtvsqdgjqw.html

Java: list.add(4);
来源：http://hz.chenjidiqi.icu/gtbpvozvzx.html

Go:   arr = append(arr, 4)
来源：http://hz.haohaochexian.top/gtrmkoiflj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxuanxn.top/gtqymsppxq.html

C#:   list.Add(4);
来源：http://hz.zhaomingkeji.xyz/gtkchpvbwl.html

[D03] 在指定位置插入元素
来源：http://hz.tanke756.top/gtfflzpfdl.html

Py:   arr.insert(0, 0)
来源：http://hz.zhengqikj.top/gtyhagbbuv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gogol.net.cn/gtmtkvmluf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guannengcc.top/gtzeqwrspn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zycfv.cn/gteulupcrk.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtzawfcjfo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.guowangkeji.top/gtmmqeeiid.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jianghu66.top/gtmlnpgclj.html

C#:   list.Insert(0, 0);
来源：http://hz.cashguo.top/gtqgzyvqee.html

[D04] 删除元素
来源：http://hz.9152youxi.cn/gtkzzhdzrm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cqqwz.cn/gtwxzvklaa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yongpay.top/gtbsnawvbl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxuanxn.top/gtinnbjgqn.html

TS:   arr.splice(0, 1);
来源：http://hz.hywenlv.cn/gtjdijmucc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.redwolf501.top/gtslzboaos.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuanzhike.top/gtpqufxidd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cheryme.top/gtrhnizrqh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.quarkkingdee.top/gtdmvybwel.html

[D05] 访问与修改元素
来源：http://hz.cashguo.top/gtxturyzdy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtkysicgxf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxinkj.top/gtcfyrjprh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.52xcode.cn/gtiohrxkht.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtzrrumuzp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nanxinkj.top/gtumsnvyts.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.redwolf501.top/gtomtdqlhc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtyyamprmu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtbgguekiy.html

[D06] 数组长度
来源：http://hz.hammf.cn/gthahqxope.html

Py:   len(arr)
来源：http://hz.ydzc1.top/gttaygmoev.html

PHP:  count($arr);
来源：http://hz.jinghuilouyu.cn/gtcclkqskt.html

JS:   arr.length
来源：http://hz.zhijiandao.cn/gtstxlvwjx.html

TS:   arr.length
来源：http://hz.yj20258888.top/gtjveyrzue.html

Java: list.size();
来源：http://hz.iojbl.cn/gtuwblegil.html

Go:   len(arr)
来源：http://hz.ydjk.org.cn/gteauzvwlz.html

Ruby: arr.length; arr.size
来源：http://hz.guowangkeji.top/gtqfvbisso.html

C#:   list.Count;
来源：http://hz.yonumen.top/gtxngdwdsy.html

[D07] 切片 / 取子数组
来源：http://hz.redwolf501.top/gtqouykkyf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gzhubu.top/gtylhdoxvr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gtszbwcfhl.html

JS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtcdledwrx.html

TS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gtyxojzrbl.html

Java: list.subList(1, 4);
来源：http://hz.xylfe.cn/gtysbqpscw.html

Go:   arr[1:4]
来源：http://hz.yanxiufei.cn/gtfowxrdya.html

Ruby: arr[1, 3]
来源：http://hz.jinqigfzy.top/gtztwhiblh.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangdashe.top/gtkgupuhlt.html

[D08] 合并两个数组
来源：http://hz.jqgufenzy.top/gtkhzqcvex.html

Py:   a + b;  a.extend(b)
来源：http://hz.fzhhl.top/gtwoqueclm.html

PHP:  array_merge($a, $b);
来源：http://hz.xuanzx.com/gtyqcmywnh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hammf.cn/gtbqcrkryl.html

TS:   [...a, ...b];
来源：http://hz.jianghu66.top/gtywmedjjd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dashuyun.cn/gtjykcqqka.html

Go:   append(a, b...)
来源：http://hz.hammf.cn/gtgzkdxeeg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.meibo888.top/gtgylbddnf.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinghuilouyu.cn/gtszhowlya.html

[D09] 排序（升序）
来源：http://hz.kuanghao11.cn/gtjdphvvsx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtwprflxns.html

PHP:  sort($arr);
来源：http://hz.fengsongda.top/gtgjlmmtxd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.bjfxy.top/gtoiacatei.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.redwolf501.top/gtptmnfxxa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ppjwa.cn/gtxdhwlxmb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtkdiehtdw.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtdogvtwyn.html

C#:   list.Sort();
来源：http://hz.daxiang520.top/gtlvaihita.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenzaomai.com/gtasrtqqdw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yvedp.cn/gtrwtjoznc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangkeji.top/gtsywdvhaq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.vqdsnc.cn/gtxitfoegx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtlrjnwdsr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xylfe.cn/gttmhmrjcq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhengqikj.top/gttnwlnkay.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gogol.net.cn/gthjhrtpyl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangshuangyany.cn/gthfbizvrm.html

[D11] 反转数组
来源：http://hz.svipenyu.cn/gtsxqoqafg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gogol.net.cn/gtwshsyyay.html

PHP:  array_reverse($arr);
来源：http://hz.yangfankeji.com/gtzkhskpak.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dashuyun.cn/gtyeiiztyj.html

TS:   [...arr].reverse();
来源：http://hz.9152youxi.cn/gttzrxzekj.html

Java: Collections.reverse(list);
来源：http://hz.tanke756.top/gtvnchhwiu.html

Go:   slices.Reverse(arr)
来源：http://hz.ppjwa.cn/gthblzuzql.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtstwiwhcy.html

C#:   list.Reverse();
来源：http://hz.zhengqikj.top/gtujtopnxg.html

[D12] 查找元素下标
来源：http://hz.tian-w.cn/gtieiwbvvd.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnxiangtu.top/gtzxipmyue.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dashuyun.cn/gtsbpnmxxj.html


<!-- 参考信息 -->