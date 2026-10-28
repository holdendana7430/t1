代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tanke756.top/gtjluneaql.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinyuanbaomall.cn/gtfjzzwsdr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.daria6918.cn/gtnepfdoia.html

[B12] 跳出多层循环
来源：http://hz.meibo888.top/gtoizjysii.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tanke756.top/gtmdahjrpy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.smart0.xyz/gtizugaplm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gtrqgcblfi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtmcngifee.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gthmgvztza.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.fengsongda.top/gttsngdwyc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.tian-w.cn/gtilfutdyq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.aibaodan.cn/gtjxxzlbyi.html

[B13] 判断是否为数字
来源：http://hz.jlsjyb.cn/gtjbdqfapf.html

Py:   isinstance(x, (int, float))
来源：http://hz.meibo888.top/gtwgkqlwoc.html

PHP:  is_numeric($x)
来源：http://hz.nwbrower.top/gtnqmjooji.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gtneeesqhn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtwgkyngpb.html

Java: x instanceof Number
来源：http://hz.redwolf501.top/gtgwvqoxzy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.c1oappe.top/gtvzpukejz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.dianchejie.cn/gtaighrgle.html

C#:   x is int or double or decimal
来源：http://hz.cashguo.top/gtturlryrz.html

[B14] 判断值是否在集合内
来源：http://hz.yueranfly.top/gtplzcynsf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.bjfxy.top/gtncpljvjf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nwbrower.top/gtmkdlyoqo.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtnafivzwr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.kuanghao11.cn/gtadfbshpf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tanke756.top/gtjhskrshe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shangyingyoupin.top/gtamzqaysh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.havefunace.top/gtpyxaqbsf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ivvv.top/gtirtmynug.html

[B15] 布尔运算与取反
来源：http://hz.zhongyouzk.top/gtvlbztofs.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtmfcpmcwu.html

PHP:  $a && $b || !$c
来源：http://hz.cheryme.top/gtqhfzchxx.html

JS:   a && b || !c
来源：http://hz.quarkkingdee.top/gteyfulrwy.html

TS:   a && b || !c
来源：http://hz.ybcxt.top/gtranghymp.html

Java: a && b || !c
来源：http://hz.ehwqpu.com/gtifakqdqr.html

Go:   a && b || !c
来源：http://hz.zhixingplan.top/gtybtmmihw.html

Ruby: a && b || !c
来源：http://hz.zhijiandao.cn/gtkfstodks.html

C#:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtfacuplqx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shanyushiyangtech.top/gtwukdjzvv.html

Py:   if not data: return
来源：http://hz.svipenyu.cn/gtyelivsiq.html

PHP:  if (!$data) { return; }
来源：http://hz.chenjidiqi.icu/gtipijksoa.html

JS:   if (!data) return;
来源：http://hz.nwbrower.top/gtrehqexdy.html

TS:   if (!data) return;
来源：http://hz.xingfuxueyuan.xyz/gtygwddamt.html

Java: if (data == null) return;
来源：http://hz.yj202588.top/gtsdsnflda.html

Go:   if data == nil { return }
来源：http://hz.guowangkeji.top/gtdcxdaknr.html

Ruby: return if data.nil?
来源：http://hz.52xcode.cn/gtazmydanz.html

C#:   if (data == null) return;
来源：http://hz.xuanzx.com/gtssmlqwwa.html

================================================================================
来源：http://hz.jinqigufen.top/gtaiqggoaz.html

C. 函数与作用域
来源：http://hz.gaohongyu789.top/gtkmwrqbua.html

================================================================================
来源：http://hz.jinqigufen.top/gtuwnyqdez.html

[C01] 定义函数
来源：http://hz.daxiang520.top/gtbrnmogyd.html

Py:   def add(a, b): return a + b
来源：http://hz.ydjk.org.cn/gtlwxwrkdj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtnfxhmxep.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cdnleiting.top/gtzosavpru.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hfpthk.cn/gtwmwachfj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtleptayea.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgufenzy.top/gtpqamaskj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sxryk.cn/gtckgkssdo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gtuvnnpfcw.html

[C02] 默认参数
来源：http://hz.guowangkeji.top/gtsbbiroqr.html

Py:   def greet(name="World"): return name
来源：http://hz.kuanghao11.cn/gtysittcdn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhixingplan.top/gtojzohhtw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nwbrower.top/gtexgydvef.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtksftstfn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.c1oappe.top/gtccoxzcda.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.wangshuangyany.cn/gtqyygvamx.html

Ruby: def greet(name = "World") = name
来源：http://hz.yvedp.cn/gtgoieoumo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.c1oappe.top/gtaaoldwre.html

[C03] 可变参数
来源：http://hz.fzhhl.top/gtrtvyrcdj.html

Py:   def total(*args): return sum(args)
来源：http://hz.ywan-chungtsiang.top/gtnainbolf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jqgufenzy.top/gtzyuxueis.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gtepqehhes.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtncevpnvp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yangfankeji.com/gtzgmtpqst.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ivvv.top/gtszjbkbxv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nwbrower.top/gthfotjovi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shangyingyoupin.top/gtfxbkkfpe.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hammf.cn/gtmnimbxfk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhiwuduotai.top/gtoubrpcph.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenzaomai.com/gtnmaugvge.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtgtitqqrw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tianlin.xyz/gtrmjvqbst.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xingfuxueyuan.xyz/gttrrfqxqz.html

Go:   // 无：用配置结构体参数
来源：http://hz.hywenlv.cn/gtksrxtwcv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtbcqpvywg.html

C#:   f(a: 1, b: 2)
来源：http://hz.shzxlz.cn/gtmiaguauv.html

[C05] 返回多个值
来源：http://hz.yanxiufei.cn/gtsfppakiy.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gtjyxvibsx.html

PHP:  return [$a, $b];
来源：http://hz.birdmap.top/gtsemotrto.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.snrcjt.cn/gtszfeezcw.html

TS:   return { a, b };
来源：http://hz.zhixingplan.top/gtzcjnfpwf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.wangshuangyany.cn/gtgjearepp.html

Go:   return a, b
来源：http://hz.jinyuanbaomall.cn/gtdwmhkxdh.html

Ruby: return a, b
来源：http://hz.aibaodan.cn/gtzsajwsnq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.kuanghao11.cn/gtowmkxktn.html

[C06] 匿名函数 / lambda
来源：http://hz.gzhubu.top/gtykdiypul.html

Py:   square = lambda x: x * x
来源：http://hz.vqdsnc.cn/gtdzezddcu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cqqwz.cn/gtsmwtzghi.html

JS:   const square = x => x * x;
来源：http://hz.yueranfly.top/gtissvgwwu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jiagoushi.top/gthboogrey.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pycfn.com/gthnrkaovf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.0kj1m.cn/gtmqnssaed.html

Ruby: square = ->(x) { x * x }
来源：http://hz.haohaochexian.top/gtegqenlcb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gogol.net.cn/gthqjiwwmd.html

[C07] 把函数作为参数传入
来源：http://hz.yongpay.top/gtlluxoewu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gtfznzdkba.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.meibo888.top/gtbmojqnva.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj20258.top/gtoqulycdy.html

TS:   arr.map(String)
来源：http://hz.xingfuxueyuan.xyz/gtkflhdlyg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.redwolf501.top/gtlixovbcr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shangyingyoupin.top/gtsgalmfbu.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258.top/gtnculxbzq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258888.top/gtxlsbgykl.html

[C08] 闭包
来源：http://hz.jinqigfzy.top/gtbceuiwhl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shuidangran.top/gtvojaemjl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gotoacloud.top/gtftplkcld.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.vqdsnc.cn/gtsfkxuwac.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtveubfxlg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.andypj.xyz/gtwqlfejuw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuxming.cn/gtchumyieq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sufxvd.cn/gtnhtfjnce.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtndmfdhvw.html

[C09] 递归
来源：http://hz.nwbrower.top/gtfpcfwcvg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtyercekwb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aibaodan.cn/gtnzrbmwrt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtxaqajtar.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.svipenyu.cn/gtcatxsdjf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuanzhike.top/gtalvzmxuz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.vqdsnc.cn/gtzzpoqhmj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fengsongda.top/gtrbyzfsqx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.guannengcc.top/gtpfjrhwiw.html

[C10] 变量作用域
来源：http://hz.jiagoushi.top/gtrlftsnup.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hfpthk.cn/gtbzenujyf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gotoacloud.top/gtzossxkxi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ywan-chungtsiang.top/gtztpmfioa.html

TS:   同 JS
来源：http://hz.xylfe.cn/gtlhvryzll.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gtofzvdngo.html

Go:   花括号块级作用域
来源：http://hz.cashguo.top/gtmhmwfqlc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.feifeiyinyue.top/gtftmtstvu.html

C#:   块级作用域
来源：http://hz.0kj1m.cn/gtmkakagqy.html

[C11] 模块导入与导出
来源：http://hz.yuxming.cn/gtuajelhpl.html

Py:   from module import func
来源：http://hz.jianghu66.top/gtcgecjvdt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shangyingyoupin.top/gtedmycjlw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sweek.top/gtjvvbdgti.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shzxlz.cn/gtprmjjikr.html

Java: import java.util.List;
来源：http://hz.quarkkingdee.top/gtqorsqoat.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.fzhhl.top/gtfocjeimf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.redwolf501.top/gtvwsswnzs.html

C#:   using System.Text;
来源：http://hz.feifeiyinyue.top/gtcjtrilis.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinyuanbaomall.cn/gtqcobwhnd.html

Py:   (lambda: print("run"))()
来源：http://hz.yonumen.top/gtywnaimub.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hysaishi.cn/gtbgafplse.html

JS:   (() => { console.log("run"); })();
来源：http://hz.52xcode.cn/gticxodwfo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtkxpifbkn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hysaishi.cn/gtgwidezep.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhengqikj.top/gtuxxmfgam.html

Ruby: -> { puts "run" }.call
来源：http://hz.quarkkingdee.top/gtqyxdxtsk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yueranfly.top/gtevyrqjod.html

[C13] 类型声明 / 类型注解
来源：http://hz.mhx1999.top/gtafwugwct.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gtwdtkpmbk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtvnjgzkbk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gzhubu.top/gtrhpanmsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sufxvd.cn/gtnzfdseqo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtabgvczkg.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtjybnoqwg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nwbrower.top/gtgarzaqqg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dashuyun.cn/gtkiykorzg.html

[C14] 泛型函数
来源：http://hz.jinyuanbaomall.cn/gtriesirxe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258888.top/gtznziycvz.html

PHP:  // 无泛型
来源：http://hz.ydjk.org.cn/gtearlbvxw.html

JS:   // 无泛型
来源：http://hz.jinqigfzy.top/gtuajwuocl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.316326.xyz/gtccwgtsxk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydzc1.top/gtawcqfmjm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yvedp.cn/gtnzbbfvpe.html

Ruby: # 无泛型
来源：http://hz.aizwys.cn/gttyunkvmz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shzxlz.cn/gtbratvjot.html

[C15] 解构 / 展开参数
来源：http://hz.hysaishi.cn/gtrqcvnbby.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258888.top/gttbfhwacx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ivvv.top/gticpzssmz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtajdznfbe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gotoacloud.top/gtdydijtvu.html

Java: // 无解构
来源：http://hz.chenlongwang.top/gtnjhqkpof.html

Go:   // 无解构
来源：http://hz.xuetiantiany.cn/gtprnbncad.html

Ruby: a, b = pair
来源：http://hz.guannengcc.top/gtmeiiauya.html

C#:   var (a, b) = pair;
来源：http://hz.xuetiantiany.cn/gtzhqgvyyh.html

[C16] 函数 / 方法重载
来源：http://hz.aibaodan.cn/gtasksaani.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gtdxlhlxmc.html

PHP:  // 无重载
来源：http://hz.316326.xyz/gtbyupqmll.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cqqwz.cn/gtqsxfvokw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yvedp.cn/gtkvshzwrz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhixingplan.top/gtemvcoylb.html

Go:   // 无重载：用不同函数名
来源：http://hz.feifeiyinyue.top/gtpjxrzwnr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.tanke756.top/gttywrpkbi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gogol.net.cn/gtpvsrantv.html

================================================================================
来源：http://hz.ivvv.top/gttkqaasge.html

D. 数组 / 列表 / 集合
来源：http://hz.zhiwuduotai.top/gtrdretwni.html

================================================================================
来源：http://hz.gotoacloud.top/gtgayoreux.html

[D01] 创建数组 / 列表
来源：http://hz.pengpengdd.cyou/gtbcgdzkkd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj20258888.top/gttvufraaz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.pengpengdd.cyou/gtghoynkhp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.52xcode.cn/gtkbjzaiyq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.kuanghao11.cn/gtjybyornx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tianlin.xyz/gtzjkzxbak.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guannengcc.top/gtagsiwslh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yonumen.top/gtfuielfof.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zycfv.cn/gtycnynqxh.html

[D02] 追加元素到末尾
来源：http://hz.ehwqpu.com/gtsurjoleb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.redwolf501.top/gtohmixily.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gotoacloud.top/gtqktkwawz.html

JS:   arr.push(4);
来源：http://hz.xziqi.cn/gtzyuthyyu.html

TS:   arr.push(4);
来源：http://hz.dashuyun.cn/gteuopvzog.html

Java: list.add(4);
来源：http://hz.jqgfzy.top/gtsmzccmgy.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangkeji.top/gtjpsllsfj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinyuanbaomall.cn/gtqjsavgtf.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtlxdqzvom.html

[D03] 在指定位置插入元素
来源：http://hz.dianchejie.cn/gtfjmpfjxz.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtuhfmdzfr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.mhx1999.top/gtlwlmoavm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.iojbl.cn/gtbilbmcdi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yanxiufei.cn/gtpcckcitw.html

Java: list.add(0, 0);
来源：http://hz.zhongyouzk.top/gthahrougz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tianlin.xyz/gtutuyscjr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnxiangtu.top/gttqxdbasq.html

C#:   list.Insert(0, 0);
来源：http://hz.gogol.net.cn/gtuykinbxm.html

[D04] 删除元素
来源：http://hz.zhiwuduotai.top/gtmccdqhae.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aizwys.cn/gtaltmjnxh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgfzy.top/gtovlhyxny.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gtgljnuhnj.html

TS:   arr.splice(0, 1);
来源：http://hz.316326.xyz/gtbvmuyunn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hywenlv.cn/gthclpbgpg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gtyqeblewv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhiwuduotai.top/gtztnsrmyq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.redwolf501.top/gtucaocbfz.html

[D05] 访问与修改元素
来源：http://hz.zycfv.cn/gtioaljuln.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtjcqmjgvh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangshuangyany.cn/gtnebgzsor.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ehwqpu.com/gtjhsqwhua.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guannengcc.top/gtcccmhyie.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.smart0.xyz/gtxddfjlow.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xylfe.cn/gtbnpoztgw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.52xcode.cn/gtwvrnaatm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yueranfly.top/gtgxkbuqom.html

[D06] 数组长度
来源：http://hz.shanyushiyangkeji.top/gtdefjymdn.html

Py:   len(arr)
来源：http://hz.bjfxy.top/gtybmwwvjy.html

PHP:  count($arr);
来源：http://hz.nanxinkj.top/gthfknfaul.html

JS:   arr.length
来源：http://hz.yangfankeji.com/gtaoympzlh.html

TS:   arr.length
来源：http://hz.fengsongda.top/gtqztrofge.html

Java: list.size();
来源：http://hz.fengsongda.top/gtkgpuaazz.html

Go:   len(arr)
来源：http://hz.ivvv.top/gtpjpiiqdw.html

Ruby: arr.length; arr.size
来源：http://hz.hammf.cn/gtcapckyaq.html

C#:   list.Count;
来源：http://hz.zhoulong.xyz/gtntduppkz.html

[D07] 切片 / 取子数组
来源：http://hz.shanyushiyangkeji.top/gtchmpecnc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zycfv.cn/gtooajtqjq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cucudq.cn/gthlujtsvj.html

JS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtaimvejsi.html

TS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtwmudwjgm.html

Java: list.subList(1, 4);
来源：http://hz.gzhubu.top/gtkbwcncyx.html

Go:   arr[1:4]
来源：http://hz.ywan-chungtsiang.top/gtwfrjaaqg.html

Ruby: arr[1, 3]
来源：http://hz.hnqzz.top/gtzibtkgsj.html

C#:   list.GetRange(1, 3);
来源：http://hz.shangyingyoupin.top/gtebcgajlp.html

[D08] 合并两个数组
来源：http://hz.shzxlz.cn/gtexvthqqy.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnqzz.top/gttkgnrriw.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxinkj.top/gtxlchwqwe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ivvv.top/gtgqyjibkn.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gthnhlytqt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.haohaochexian.top/gttvnowxfo.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gtyggoetna.html

Ruby: a + b;  a.concat(b)
来源：http://hz.havefunace.top/gtoigtvvow.html

C#:   a.Concat(b).ToList()
来源：http://hz.tian-w.cn/gtmhrihebz.html

[D09] 排序（升序）
来源：http://hz.kuanghao11.cn/gtoetnxtry.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtyzjcrtay.html

PHP:  sort($arr);
来源：http://hz.jqgfzy.top/gtpcbskulz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jlsjyb.cn/gtzherqiie.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ppjwa.cn/gtjryeeewm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cucudq.cn/gtnarwoqwg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gthurkrjgw.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtrjucglke.html

C#:   list.Sort();
来源：http://hz.yanxiufei.cn/gtqldfwlcp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jyoumei.cn/gtmomcyczb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtwabhcysk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtobqkqppv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtfverbaqu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhongyouzk.top/gtkbnjcaul.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.redwolf501.top/gtxqxdbbry.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangtech.top/gtngxmzrag.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuetiantiany.cn/gtlehaimhv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.vqdsnc.cn/gtnadwmrcc.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtorjibvxe.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guowangkeji.top/gtqrchqhwv.html

PHP:  array_reverse($arr);
来源：http://hz.hysaishi.cn/gtckfrabsl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yongpay.top/gtakkldrfu.html

TS:   [...arr].reverse();
来源：http://hz.yvedp.cn/gtzzmfixgf.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtlykskgfz.html

Go:   slices.Reverse(arr)
来源：http://hz.sxryk.cn/gtjnqvagco.html

Ruby: arr.reverse
来源：http://hz.gzhubu.top/gtltqrojec.html

C#:   list.Reverse();
来源：http://hz.fzhhl.top/gtrbokgvhs.html

[D12] 查找元素下标
来源：http://hz.ehwqpu.com/gtwiopbmon.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhijiandao.cn/gtucocvzgc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.316326.xyz/gtmhvqjngu.html


<!-- 参考信息 -->