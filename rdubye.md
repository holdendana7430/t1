代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ydzc1.top/gtwiwkladf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yonumen.top/gtgepwgpgd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gotoacloud.top/gtmpwwyoua.html

[B12] 跳出多层循环
来源：http://hz.ydzc1.top/gtscrrcchw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cucudq.cn/gtojwdonoy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xingfuxueyuan.xyz/gtkgonptqm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtmotxdxoq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gthmbdfnzp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtmzhdettr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xingfuxueyuan.xyz/gtozrxysrm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinqigfzy.top/gtrfihbmcl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.havefunace.top/gtpedaozjj.html

[B13] 判断是否为数字
来源：http://hz.pycfn.com/gtitlmwyef.html

Py:   isinstance(x, (int, float))
来源：http://hz.guannengcc.top/gtpghybyds.html

PHP:  is_numeric($x)
来源：http://hz.fengsongda.top/gtcguqkqge.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangtech.top/gttxoqjjaw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pengpengdd.cyou/gtlmlkiitk.html

Java: x instanceof Number
来源：http://hz.jinghuilouyu.cn/gtxpdjrdna.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yangfankeji.com/gtpiyhxwer.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jiagoushi.top/gtlsocovvs.html

C#:   x is int or double or decimal
来源：http://hz.fengsongda.top/gtwpbasycq.html

[B14] 判断值是否在集合内
来源：http://hz.snrcjt.cn/gtivchxqzx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuanzx.com/gtxdcknpaf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hysaishi.cn/gtvhvxjvxx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.guowangkeji.top/gtgdawcfyo.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gthtsuffan.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhengqikj.top/gtieraaqbd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenlongwang.top/gtfbkludbz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cdnleiting.top/gtkltqapwi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yuxming.cn/gtxqydesto.html

[B15] 布尔运算与取反
来源：http://hz.xziqi.cn/gtmqpcqbui.html

Py:   a and b or not c
来源：http://hz.yonumen.top/gtulokaeuy.html

PHP:  $a && $b || !$c
来源：http://hz.jiagoushi.top/gtbqqgpqyx.html

JS:   a && b || !c
来源：http://hz.yj20258.top/gtrrkmzydq.html

TS:   a && b || !c
来源：http://hz.dianchejie.cn/gtyafxfjih.html

Java: a && b || !c
来源：http://hz.jianghu66.top/gtvmrxtmrv.html

Go:   a && b || !c
来源：http://hz.haohaochexian.top/gtylifrphs.html

Ruby: a && b || !c
来源：http://hz.yonumen.top/gtfgmsmgfg.html

C#:   a && b || !c
来源：http://hz.cucudq.cn/gtkwwhsqaa.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ehwqpu.com/gtkhpxawsd.html

Py:   if not data: return
来源：http://hz.shanyushiyangkeji.top/gtvcsofaif.html

PHP:  if (!$data) { return; }
来源：http://hz.wangshuangyany.cn/gtkvrqlwio.html

JS:   if (!data) return;
来源：http://hz.hnqzz.top/gtcotlpzpz.html

TS:   if (!data) return;
来源：http://hz.smart0.xyz/gtbrzbztcd.html

Java: if (data == null) return;
来源：http://hz.shangyingyoupin.top/gtqktjmkxj.html

Go:   if data == nil { return }
来源：http://hz.hnqzz.top/gtbocqmfqx.html

Ruby: return if data.nil?
来源：http://hz.ivvv.top/gtcquqczvc.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtqhlwegho.html

================================================================================
来源：http://hz.xinyue.icu/gtythgdyof.html

C. 函数与作用域
来源：http://hz.jinghuilouyu.cn/gthomagcuz.html

================================================================================
来源：http://hz.cheryme.top/gtevgewnhp.html

[C01] 定义函数
来源：http://hz.sufxvd.cn/gtzspdsizr.html

Py:   def add(a, b): return a + b
来源：http://hz.quarkkingdee.top/gtvofblhwt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gttmxnwpag.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.smart0.xyz/gtgytamplc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.c1oappe.top/gtrmyakohg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtbqobqljq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.havefunace.top/gtwcpwuihr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhijiandao.cn/gtpsthffwn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nwbrower.top/gtuvccjkfa.html

[C02] 默认参数
来源：http://hz.hfpthk.cn/gtovhtnpyd.html

Py:   def greet(name="World"): return name
来源：http://hz.ehwqpu.com/gtugpsnjxd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258888.top/gteucmrdal.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jiagoushi.top/gtvxocemds.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtzosqymup.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ehwqpu.com/gtozfjvehq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ybcxt.top/gtnkglrgwi.html

Ruby: def greet(name = "World") = name
来源：http://hz.daria6918.cn/gtbsfsofgc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.mhx1999.top/gtcfadlvvb.html

[C03] 可变参数
来源：http://hz.daria6918.cn/gtgteztsji.html

Py:   def total(*args): return sum(args)
来源：http://hz.cucudq.cn/gtnvdlbfqf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hywenlv.cn/gtxrtelejf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.havefunace.top/gtnfhcynvx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenzaomai.com/gtccmshmai.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenjidiqi.icu/gtwyldnqah.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.aizwys.cn/gtriqyklbq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gaohongyu789.top/gtagstrrya.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yueranfly.top/gthxwzdwmw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.smart0.xyz/gtnblnhmyn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yueranfly.top/gtbdfayjmv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yueranfly.top/gtiznjsoch.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shuidangran.top/gtxxixcuvz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jyoumei.cn/gtywmbxydz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxinkj.top/gtkegmazsa.html

Go:   // 无：用配置结构体参数
来源：http://hz.cashguo.top/gtzdsngopx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtfkhcsjpy.html

C#:   f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtqjtfkxpf.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gtfxmmdats.html

Py:   return a, b
来源：http://hz.havefunace.top/gtlpmdjrgu.html

PHP:  return [$a, $b];
来源：http://hz.guannengcc.top/gtizetnamt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xylfe.cn/gtgghizwcl.html

TS:   return { a, b };
来源：http://hz.ybcxt.top/gtkpjqsisr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xingfuxueyuan.xyz/gttiwleawz.html

Go:   return a, b
来源：http://hz.gogol.net.cn/gtfyjioakk.html

Ruby: return a, b
来源：http://hz.shanyushiyangtech.top/gtceqvpujq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.9152youxi.cn/gtivsfxkju.html

[C06] 匿名函数 / lambda
来源：http://hz.zhongyouzk.top/gtkhndadvv.html

Py:   square = lambda x: x * x
来源：http://hz.yuanzhike.top/gtvuyjjrmj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sufxvd.cn/gtnodxdjfo.html

JS:   const square = x => x * x;
来源：http://hz.nwbrower.top/gtxjkuwvuo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinqigfzy.top/gtmytcodos.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ivvv.top/gtvntkqolz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guannengcc.top/gteslwiylu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxuanxn.top/gtbnnjgqfd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtkaxireja.html

[C07] 把函数作为参数传入
来源：http://hz.hnxiangtu.top/gtyharbjiz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinqigufen.top/gtsxrcfmdg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhaomingkeji.xyz/gthjywaulx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ybcxt.top/gtejknfkxg.html

TS:   arr.map(String)
来源：http://hz.ivvv.top/gtlxpdinqd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xuanzx.com/gtaymvybql.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.pengpengdd.cyou/gtkmkcoawf.html

Ruby: arr.map(&:upcase)
来源：http://hz.hnqzz.top/gtvconipnf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sxryk.cn/gtxwqhsyzo.html

[C08] 闭包
来源：http://hz.shanyushiyangtech.top/gtsyxrnejs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shangyingyoupin.top/gtqykgkvbo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.smart0.xyz/gtkuawkmoc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gthcqdvxnu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtfasygxct.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zycfv.cn/gtmokwlsgo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.52xcode.cn/gtubcyptfo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hammf.cn/gtmvileoir.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtestjqxwn.html

[C09] 递归
来源：http://hz.jlsjyb.cn/gtiaxmmbye.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258.top/gtksewpomc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhoulong.xyz/gtflojshke.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtmfefvmct.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtoehkavqo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtobghvafe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhiwuduotai.top/gtlvofzhdv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ybcxt.top/gtnuovmxki.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnqzz.top/gtrvdqyauk.html

[C10] 变量作用域
来源：http://hz.wangdashe.top/gtraucxizh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhaomingkeji.xyz/gtepaubwpf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhixingplan.top/gtnpleskxt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shanyushiyangtech.top/gtdxahyzti.html

TS:   同 JS
来源：http://hz.cucudq.cn/gtdocrfcvz.html

Java: 方法内为块级作用域
来源：http://hz.yueranfly.top/gtqtzeqigz.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangkeji.top/gtfbyedwca.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yanxiufei.cn/gtfkpaamna.html

C#:   块级作用域
来源：http://hz.wangdashe.top/gtsoibhswd.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gtcpmewbuy.html

Py:   from module import func
来源：http://hz.ybcxt.top/gtlowdzzsa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.snrcjt.cn/gthsrvdfzt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.andypj.xyz/gtemxetrbz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.havefunace.top/gtsvuxdjgd.html

Java: import java.util.List;
来源：http://hz.zhoulong.xyz/gtxssbxtrn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sysykeji.top/gtumufnobh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.mhx1999.top/gthzrsfmfu.html

C#:   using System.Text;
来源：http://hz.jinghuilouyu.cn/gtcgklylqf.html

[C12] 立即执行函数 IIFE
来源：http://hz.sysykeji.top/gtrkmykkvv.html

Py:   (lambda: print("run"))()
来源：http://hz.hongshengwenyu.top/gtwxaxepjn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.smart0.xyz/gtiatbgbwq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gtlicnbfdg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aizwys.cn/gtbyrzpsdo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhengqikj.top/gtouroijak.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yangfankeji.com/gtcgdolzfn.html

Ruby: -> { puts "run" }.call
来源：http://hz.xinyue.icu/gtjylgzfin.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shangyingyoupin.top/gthxwplqyx.html

[C13] 类型声明 / 类型注解
来源：http://hz.9152youxi.cn/gtiwjfppxn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gogol.net.cn/gtdtmuqkke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtzxjupvfs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hammf.cn/gtsuaalioe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtjvqxhttv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtxaixvapq.html

Go:   func add(a, b int) int
来源：http://hz.ydjk.org.cn/gtzjjjmpwp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guowangkeji.top/gtqpaubmow.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.meibo888.top/gtxsqvotqo.html

[C14] 泛型函数
来源：http://hz.svipenyu.cn/gtsizohlir.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuanzhike.top/gtmuorbajt.html

PHP:  // 无泛型
来源：http://hz.jyoumei.cn/gteamdqpbp.html

JS:   // 无泛型
来源：http://hz.zhixingplan.top/gtqmuxoynj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fengsongda.top/gtngzvxixf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daria6918.cn/gtuhjbikhe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuanzhike.top/gtcdtamzjh.html

Ruby: # 无泛型
来源：http://hz.wangshuangyany.cn/gtkwhbjlso.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.316326.xyz/gtwpaxmkra.html

[C15] 解构 / 展开参数
来源：http://hz.yongpay.top/gtnajavcow.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.redwolf501.top/gtwqmiqevw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.0kj1m.cn/gtprniwgpt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtqametopi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xuanzx.com/gtxrtlyjtx.html

Java: // 无解构
来源：http://hz.chenjidiqi.icu/gtnvfdudqb.html

Go:   // 无解构
来源：http://hz.gogol.net.cn/gtltvjumds.html

Ruby: a, b = pair
来源：http://hz.yangfankeji.com/gtbgcbzoqm.html

C#:   var (a, b) = pair;
来源：http://hz.ybcxt.top/gtwqalcdcl.html

[C16] 函数 / 方法重载
来源：http://hz.gogol.net.cn/gttvhejzgw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cucudq.cn/gthbefsvaz.html

PHP:  // 无重载
来源：http://hz.xziqi.cn/gtntzywjjl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ydzc1.top/gtebahouxf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtauspvzuh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhengqikj.top/gtbattvqcp.html

Go:   // 无重载：用不同函数名
来源：http://hz.tanke756.top/gtvjopltid.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xinyue.icu/gtvnjqxivi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daria6918.cn/gtddofpfbb.html

================================================================================
来源：http://hz.aizwys.cn/gtwleotbif.html

D. 数组 / 列表 / 集合
来源：http://hz.wangdashe.top/gtfgcfgqwg.html

================================================================================
来源：http://hz.nanxinkj.top/gtkyrlvhmg.html

[D01] 创建数组 / 列表
来源：http://hz.9152youxi.cn/gtgtlqodlg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cqqwz.cn/gtkpcjpkat.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.c1oappe.top/gtnonbxtjr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gogol.net.cn/gthmrbxogr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jlsjyb.cn/gtfyyetygw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yangfankeji.com/gtgujfbtol.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tian-w.cn/gtfxcsjgcq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guannengcc.top/gtcbnplzqh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenjidiqi.icu/gtseilvuno.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtpyxybygq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hammf.cn/gtxtsvmsag.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gzhubu.top/gtwqzkzeta.html

JS:   arr.push(4);
来源：http://hz.sxryk.cn/gtlqujzmcp.html

TS:   arr.push(4);
来源：http://hz.yuxming.cn/gtfkehsnpn.html

Java: list.add(4);
来源：http://hz.sxryk.cn/gtenscxvkq.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gtmmindgwn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gtrcxfjjph.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gtuanpraud.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gteyjcvuec.html

Py:   arr.insert(0, 0)
来源：http://hz.zhiwuduotai.top/gtkkpbxnkr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgufenzy.top/gtyznbwscp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigufen.top/gtpyogfbta.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ywan-chungtsiang.top/gtqnnkzbrk.html

Java: list.add(0, 0);
来源：http://hz.pycfn.com/gtgjfxdhdh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.mhx1999.top/gtlnkesjmg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigfzy.top/gtsuutsnrs.html

C#:   list.Insert(0, 0);
来源：http://hz.jinyuanbaomall.cn/gttlmkopmg.html

[D04] 删除元素
来源：http://hz.zycfv.cn/gtncpggkhh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydjk.org.cn/gtacbawafe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ywan-chungtsiang.top/gtszsdhcer.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jqgfzy.top/gteppggiim.html

TS:   arr.splice(0, 1);
来源：http://hz.hysaishi.cn/gtyklyulfn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jyoumei.cn/gteewckwnh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtvbtnocjt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtnaigcymw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuxming.cn/gtdmywmywt.html

[D05] 访问与修改元素
来源：http://hz.xylfe.cn/gtzcwrppky.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtcaefaagl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ivvv.top/gtaojnxopy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ehwqpu.com/gtsdenlzpc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.svipenyu.cn/gtqrjmmnlr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.bjfxy.top/gtkxtuhzqe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hnqzz.top/gtusxcveob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtxmewkjcp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gaohongyu789.top/gtsyzvrtys.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtcxmwpgtx.html

Py:   len(arr)
来源：http://hz.xuanzx.com/gttoyqxnyn.html

PHP:  count($arr);
来源：http://hz.tanke756.top/gtewlksjvi.html

JS:   arr.length
来源：http://hz.sufxvd.cn/gtugxjzpzs.html

TS:   arr.length
来源：http://hz.kuanghao11.cn/gtxutgnszg.html

Java: list.size();
来源：http://hz.jinqigfzy.top/gtgtpwahfm.html

Go:   len(arr)
来源：http://hz.nanxuanxn.top/gtjixblsvg.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gttjwrtsoq.html

C#:   list.Count;
来源：http://hz.cdnleiting.top/gtdkxhhsto.html

[D07] 切片 / 取子数组
来源：http://hz.meibo888.top/gtnpymukak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dianchejie.cn/gtzwreqviz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258.top/gtrocrfwuv.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtbrcvxfam.html

TS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gtpvhmrcwa.html

Java: list.subList(1, 4);
来源：http://hz.daria6918.cn/gtculuuymc.html

Go:   arr[1:4]
来源：http://hz.daxiang520.top/gthinfqkjj.html

Ruby: arr[1, 3]
来源：http://hz.gotoacloud.top/gtbvyknpwh.html

C#:   list.GetRange(1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtgkhmnlex.html

[D08] 合并两个数组
来源：http://hz.yj20258.top/gtupernwbq.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinyuanbaomall.cn/gtlpdxiapc.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258888.top/gtmzwupgay.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jiagoushi.top/gtnoysaozw.html

TS:   [...a, ...b];
来源：http://hz.hammf.cn/gtioggccmu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj202588.top/gttrkezjey.html

Go:   append(a, b...)
来源：http://hz.cashguo.top/gtgkugofaf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.svipenyu.cn/gtcflumuog.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258888.top/gtiramqhqs.html

[D09] 排序（升序）
来源：http://hz.hysaishi.cn/gtyqegwnvz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtsxzeoiae.html

PHP:  sort($arr);
来源：http://hz.hongshengwenyu.top/gtdsxorkyl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cashguo.top/gthnalbafl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hammf.cn/gtluborneb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jiagoushi.top/gtsonptjmd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtlqfravxa.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gthklsxjwd.html

C#:   list.Sort();
来源：http://hz.hnxiangtu.top/gtpwlcuhqk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.snrcjt.cn/gtaabtsdbu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guowangkeji.top/gtzbwjzwcv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtxhaevdus.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtmsxvpyhl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtdwofhwfz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.birdmap.top/gtrzcinjtg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cheryme.top/gthwvtwpig.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ehwqpu.com/gtyjskciuf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ppjwa.cn/gtknftoizw.html

[D11] 反转数组
来源：http://hz.xuanzx.com/gtqhjhwfqr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ppjwa.cn/gtyuqvqror.html

PHP:  array_reverse($arr);
来源：http://hz.52xcode.cn/gthinfltwz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tian-w.cn/gtyqnmwlgp.html

TS:   [...arr].reverse();
来源：http://hz.daria6918.cn/gtulgjjxqx.html

Java: Collections.reverse(list);
来源：http://hz.havefunace.top/gtizrixdve.html

Go:   slices.Reverse(arr)
来源：http://hz.mhx1999.top/gtfyytmfys.html

Ruby: arr.reverse
来源：http://hz.fengsongda.top/gtjhbcpgde.html

C#:   list.Reverse();
来源：http://hz.yj20258.top/gtisshsfxg.html

[D12] 查找元素下标
来源：http://hz.dashuyun.cn/gtlopuolfd.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhoulong.xyz/gtuhukoiym.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ppjwa.cn/gtqqszegdr.html


<!-- 参考信息 -->