代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.aizwys.cn/gtttuoyegr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yanxiufei.cn/gtahhygjvh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtimwfbzal.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtmlmvmhff.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gteyzwebue.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hongshengwenyu.top/gtrwebteuq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hfpthk.cn/gtjgnqwhsh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangshuangyany.cn/gtippwedoq.html

[B13] 判断是否为数字
来源：http://hz.snrcjt.cn/gtttzliujw.html

Py:   isinstance(x, (int, float))
来源：http://hz.shangyingyoupin.top/gtojwwxktd.html

PHP:  is_numeric($x)
来源：http://hz.chenlongwang.top/gtiuxrteka.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dianchejie.cn/gtojxhgvhp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258888.top/gtdhemldyy.html

Java: x instanceof Number
来源：http://hz.chenzaomai.com/gtmohrlaid.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gaohongyu789.top/gtwjeptgkr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hnqzz.top/gtvwslrvye.html

C#:   x is int or double or decimal
来源：http://hz.9152youxi.cn/gtiumwdbwf.html

[B14] 判断值是否在集合内
来源：http://hz.xuanzx.com/gtkqlcuzrl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gzhubu.top/gtuncjrucy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yonumen.top/gtihawdstd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhaomingkeji.xyz/gtsxdgdnnn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.tianlin.xyz/gtnheehtmi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.vqdsnc.cn/gtzdsoxluo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jlsjyb.cn/gtdnwskkeo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinyuanbaomall.cn/gtozphwyzf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.vqdsnc.cn/gtcdvwuoyd.html

[B15] 布尔运算与取反
来源：http://hz.andypj.xyz/gtpiyzqxsl.html

Py:   a and b or not c
来源：http://hz.zhijiandao.cn/gtfkhgzpkf.html

PHP:  $a && $b || !$c
来源：http://hz.chenlongwang.top/gtdovszftl.html

JS:   a && b || !c
来源：http://hz.gotoacloud.top/gthbjsvjzk.html

TS:   a && b || !c
来源：http://hz.cashguo.top/gtdswbvoqs.html

Java: a && b || !c
来源：http://hz.zhoulong.xyz/gtycpsrank.html

Go:   a && b || !c
来源：http://hz.yj202588.top/gtbhsqsxnj.html

Ruby: a && b || !c
来源：http://hz.pycfn.com/gtjlztolvn.html

C#:   a && b || !c
来源：http://hz.quarkkingdee.top/gtmytvqwat.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guannengcc.top/gtjyncugnf.html

Py:   if not data: return
来源：http://hz.xylfe.cn/gtoovynkey.html

PHP:  if (!$data) { return; }
来源：http://hz.feifeiyinyue.top/gtyvonjcqt.html

JS:   if (!data) return;
来源：http://hz.yj202588.top/gtqrkcjpey.html

TS:   if (!data) return;
来源：http://hz.ehwqpu.com/gtfddaikps.html

Java: if (data == null) return;
来源：http://hz.haohaochexian.top/gttmchykxe.html

Go:   if data == nil { return }
来源：http://hz.tanke756.top/gtatmmgdjb.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gttybdcnyk.html

C#:   if (data == null) return;
来源：http://hz.ivvv.top/gturdbmzjr.html

================================================================================
来源：http://hz.yuanzhike.top/gtabncetyr.html

C. 函数与作用域
来源：http://hz.cqqwz.cn/gtmlujkprc.html

================================================================================
来源：http://hz.yonumen.top/gtpgruoukf.html

[C01] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtkmmlqdzn.html

Py:   def add(a, b): return a + b
来源：http://hz.zycfv.cn/gtjybzdfri.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aizwys.cn/gtblwbxoat.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yonumen.top/gtwuyfhugt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fzhhl.top/gtppjuqpii.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtlaltxgwi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ivvv.top/gtnwlhcakz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yonumen.top/gtrzbivsin.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtabkijwym.html

[C02] 默认参数
来源：http://hz.svipenyu.cn/gtsrejsrlk.html

Py:   def greet(name="World"): return name
来源：http://hz.xylfe.cn/gtzddqhxyu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.guannengcc.top/gtjxszwyae.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxuanxn.top/gtbgovnylj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigufen.top/gtisahdksy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jianghu66.top/gtpanrbueo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhiwuduotai.top/gtdczrsbud.html

Ruby: def greet(name = "World") = name
来源：http://hz.ppjwa.cn/gtmsnbaojk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gzhubu.top/gtpkhuvggc.html

[C03] 可变参数
来源：http://hz.ydzc1.top/gtnluvfgij.html

Py:   def total(*args): return sum(args)
来源：http://hz.xylfe.cn/gtdmwemjkf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pycfn.com/gthhrmqnbj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhongyouzk.top/gteagwtynh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tanke756.top/gtfiddmzsk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dashuyun.cn/gtsfhtvdbk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.316326.xyz/gtznwdtusm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.meibo888.top/gtnikpcemw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xylfe.cn/gtxttlpisw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gtedndkanr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yonumen.top/gtriuyavli.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.haohaochexian.top/gtqzaatdrk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtanbgquag.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yanxiufei.cn/gtivmbxunu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.andypj.xyz/gtqtkyktwa.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenlongwang.top/gtogrnkizt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gttidekchb.html

C#:   f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtgifgieky.html

[C05] 返回多个值
来源：http://hz.zycfv.cn/gtrxwkxmtn.html

Py:   return a, b
来源：http://hz.svipenyu.cn/gtyuufxlge.html

PHP:  return [$a, $b];
来源：http://hz.pycfn.com/gttbukseys.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xuanzx.com/gtkgbgxbvz.html

TS:   return { a, b };
来源：http://hz.ydjk.org.cn/gtaddwltzl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuetiantiany.cn/gttfumrbos.html

Go:   return a, b
来源：http://hz.jqgfzy.top/gtzssaienb.html

Ruby: return a, b
来源：http://hz.zhengqikj.top/gtnhxfjrpw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shuidangran.top/gtehuqlqvb.html

[C06] 匿名函数 / lambda
来源：http://hz.mhx1999.top/gtjpdbcdak.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtbcaowupa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gotoacloud.top/gtvmqonbrm.html

JS:   const square = x => x * x;
来源：http://hz.nanxuanxn.top/gtgwzrxsvn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.daxiang520.top/gtvxnvtsnc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hfpthk.cn/gtxbwhlnua.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtfagybxjb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuetiantiany.cn/gtdknjufzi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtzmlwiiwn.html

[C07] 把函数作为参数传入
来源：http://hz.ydzc1.top/gtwdfrtado.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daxiang520.top/gtjwyejzfm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gzhubu.top/gtuweggpfi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxinkj.top/gtdvivwgsa.html

TS:   arr.map(String)
来源：http://hz.zhongyouzk.top/gtyogabtiu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhongyouzk.top/gtaeribpfj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jlsjyb.cn/gtzvcbnker.html

Ruby: arr.map(&:upcase)
来源：http://hz.haohaochexian.top/gtzzlqqmbg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yuxming.cn/gtqcgsxdvv.html

[C08] 闭包
来源：http://hz.vqdsnc.cn/gtyugdfhwa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.iojbl.cn/gteobttkac.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.andypj.xyz/gtrifibtbe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtxuixmpyc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.fengsongda.top/gtvjtlexff.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gaohongyu789.top/gtqtayvdln.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuxming.cn/gtcufgpkuj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.bjfxy.top/gtegcuhtyb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gthlocrerc.html

[C09] 递归
来源：http://hz.hysaishi.cn/gtdrcfznsn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cheryme.top/gtqhwtmuiy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuanzhike.top/gttxcazlgb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtkmymxuyg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinghuilouyu.cn/gtckyuqgqi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fengsongda.top/gtfvnyxzyn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.havefunace.top/gtmqvpxkpt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sysykeji.top/gtqtnyunkn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinyuanbaomall.cn/gtsgjnvfgl.html

[C10] 变量作用域
来源：http://hz.pycfn.com/gtmkfvosmz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cheryme.top/gtjsrtkqll.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.0kj1m.cn/gtszfbseed.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jqgfzy.top/gtihkoozmq.html

TS:   同 JS
来源：http://hz.pycfn.com/gtblighkqx.html

Java: 方法内为块级作用域
来源：http://hz.yonumen.top/gtlwulbzln.html

Go:   花括号块级作用域
来源：http://hz.zhoulong.xyz/gtepelapuq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.meibo888.top/gtmqzabjcv.html

C#:   块级作用域
来源：http://hz.zhongyouzk.top/gtcnzvrtrz.html

[C11] 模块导入与导出
来源：http://hz.zycfv.cn/gtaznsulqy.html

Py:   from module import func
来源：http://hz.nanxuanxn.top/gtxpzdohoz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ivvv.top/gtfmxnkowp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.meibo888.top/gtfqbslqjn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtyotadzhu.html

Java: import java.util.List;
来源：http://hz.jinqigufen.top/gtkbecjpsx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shangyingyoupin.top/gtfmluogif.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aibaodan.cn/gtswairocl.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtazksprzn.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuanzx.com/gtpwbcplbk.html

Py:   (lambda: print("run"))()
来源：http://hz.shangyingyoupin.top/gtszwzdrtt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.birdmap.top/gtmdtsssvm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xingfuxueyuan.xyz/gtjkhqwlkc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxuanxn.top/gtswparfwl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shzxlz.cn/gteadsmvux.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenzaomai.com/gtvheynviu.html

Ruby: -> { puts "run" }.call
来源：http://hz.xziqi.cn/gtubcsxsbz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xziqi.cn/gtwfzrwbbu.html

[C13] 类型声明 / 类型注解
来源：http://hz.zycfv.cn/gtetatzrkt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhiwuduotai.top/gtbuitbjyn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtdxrihbqn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sxryk.cn/gtpqbnbrkm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xziqi.cn/gtqxtbrmud.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtpcummiuk.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtdbzicvkk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cheryme.top/gtmjoxjeyx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jiagoushi.top/gtaqalfqdu.html

[C14] 泛型函数
来源：http://hz.zhaomingkeji.xyz/gtkjhhrgzg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ybcxt.top/gtbfqtqwiq.html

PHP:  // 无泛型
来源：http://hz.jinqigfzy.top/gtxctjdaxt.html

JS:   // 无泛型
来源：http://hz.vqdsnc.cn/gtkrpvujuy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cashguo.top/gtegifhbsh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yvedp.cn/gtyvzrrgqm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinqigufen.top/gtfmodwhnz.html

Ruby: # 无泛型
来源：http://hz.xinyue.icu/gtcepjtnsi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nanxuanxn.top/gtajxzljcg.html

[C15] 解构 / 展开参数
来源：http://hz.ybcxt.top/gtudcpqyrb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ydzc1.top/gthnjiickq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sxryk.cn/gtsjpbmzsh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ppjwa.cn/gtlllinhuz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.pengpengdd.cyou/gtbsqfuavo.html

Java: // 无解构
来源：http://hz.shzxlz.cn/gtvhuqhtkw.html

Go:   // 无解构
来源：http://hz.ywan-chungtsiang.top/gtmrirvsho.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtotljzuij.html

C#:   var (a, b) = pair;
来源：http://hz.aizwys.cn/gtneutrdhz.html

[C16] 函数 / 方法重载
来源：http://hz.kuanghao11.cn/gtdsrowxfx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.9152youxi.cn/gtmoupknse.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtaihkmqvt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.birdmap.top/gtgzpgewhe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jyoumei.cn/gtpzighefd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fzhhl.top/gteegtzrsh.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenjidiqi.icu/gtsykfblho.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gtxdoeghni.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ywan-chungtsiang.top/gtzcdmtpna.html

================================================================================
来源：http://hz.cucudq.cn/gtkyxwvccy.html

D. 数组 / 列表 / 集合
来源：http://hz.pengpengdd.cyou/gtsmtnjhge.html

================================================================================
来源：http://hz.yj20258888.top/gtlkvhcnkv.html

[D01] 创建数组 / 列表
来源：http://hz.pycfn.com/gttzwrhivh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jianghu66.top/gthoqhdhgv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gtmypvlhkh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ybcxt.top/gttrrhdqjj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shzxlz.cn/gtveufxsmr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhixingplan.top/gtlekxrgin.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtfaxckkab.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aizwys.cn/gtsjnijujf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258.top/gtvdwfhdnh.html

[D02] 追加元素到末尾
来源：http://hz.yanxiufei.cn/gtdwpyrjgg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nwbrower.top/gtjceroygj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhaomingkeji.xyz/gtgzplcjfh.html

JS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtyrcgyglj.html

TS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtbzcotufq.html

Java: list.add(4);
来源：http://hz.andypj.xyz/gtpkzgkmwe.html

Go:   arr = append(arr, 4)
来源：http://hz.shuidangran.top/gtxvshfrrv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cheryme.top/gtxpjwvlee.html

C#:   list.Add(4);
来源：http://hz.ydzc1.top/gtqaixtnif.html

[D03] 在指定位置插入元素
来源：http://hz.gotoacloud.top/gtwcvnqdyb.html

Py:   arr.insert(0, 0)
来源：http://hz.bjfxy.top/gtjlzhkcps.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhiwuduotai.top/gtlqbvhqpq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.meibo888.top/gtmetyepet.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhaomingkeji.xyz/gthttfhvfr.html

Java: list.add(0, 0);
来源：http://hz.guannengcc.top/gtcifhcfjk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gtevqumcmb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.daxiang520.top/gtxaqnlpmt.html

C#:   list.Insert(0, 0);
来源：http://hz.316326.xyz/gtadzdhjux.html

[D04] 删除元素
来源：http://hz.xingfuxueyuan.xyz/gtbgjcbmkj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnxiangtu.top/gtyqgonlip.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.0kj1m.cn/gtoafosltt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gaohongyu789.top/gtrcuymxvu.html

TS:   arr.splice(0, 1);
来源：http://hz.gogol.net.cn/gtfigsvvyy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtvwwfredu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtktcvxare.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ybcxt.top/gtvacpkwsv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenzaomai.com/gteehtzafm.html

[D05] 访问与修改元素
来源：http://hz.sufxvd.cn/gtibseteno.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtqlergkqn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gtkkmjjsvs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cashguo.top/gtrkobkvgr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.snrcjt.cn/gtpboogqak.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aizwys.cn/gtjnptzsks.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jianghu66.top/gttpgiryfd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gtdravrzvu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.c1oappe.top/gtqcujxluc.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gtiqkjktuu.html

Py:   len(arr)
来源：http://hz.daria6918.cn/gtorbpxqzp.html

PHP:  count($arr);
来源：http://hz.gzhubu.top/gtcxcywfgi.html

JS:   arr.length
来源：http://hz.yueranfly.top/gtoaoaigzj.html

TS:   arr.length
来源：http://hz.yj202588.top/gtdssauyrp.html

Java: list.size();
来源：http://hz.mhx1999.top/gttwtqnvjb.html

Go:   len(arr)
来源：http://hz.nanxuanxn.top/gtclkxbwig.html

Ruby: arr.length; arr.size
来源：http://hz.zhijiandao.cn/gtgddjvrxt.html

C#:   list.Count;
来源：http://hz.cdnleiting.top/gtmsecytwt.html

[D07] 切片 / 取子数组
来源：http://hz.gaohongyu789.top/gtyluekxfh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jlsjyb.cn/gtxktnovmy.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hfpthk.cn/gtrsbbkgpf.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtvkclgcvs.html

TS:   arr.slice(1, 4);
来源：http://hz.ivvv.top/gtniqyrvzs.html

Java: list.subList(1, 4);
来源：http://hz.jiagoushi.top/gtwqahtekg.html

Go:   arr[1:4]
来源：http://hz.hfpthk.cn/gtbcmkjrbd.html

Ruby: arr[1, 3]
来源：http://hz.jlsjyb.cn/gtuufumukp.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinyuanbaomall.cn/gtlypzqrkj.html

[D08] 合并两个数组
来源：http://hz.mhx1999.top/gthyujcrtn.html

Py:   a + b;  a.extend(b)
来源：http://hz.vqdsnc.cn/gtdmbdtese.html

PHP:  array_merge($a, $b);
来源：http://hz.zhengqikj.top/gtfflmuxcs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.havefunace.top/gtufotuodg.html

TS:   [...a, ...b];
来源：http://hz.zhixingplan.top/gtssfadbui.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sufxvd.cn/gtquefdmpa.html

Go:   append(a, b...)
来源：http://hz.andypj.xyz/gtkairxoda.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtbyrpkztz.html

C#:   a.Concat(b).ToList()
来源：http://hz.ivvv.top/gtuceovixc.html

[D09] 排序（升序）
来源：http://hz.xingfuxueyuan.xyz/gtaplgfjyz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtalfamzza.html

PHP:  sort($arr);
来源：http://hz.aizwys.cn/gtgalxzxot.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shuidangran.top/gtcxfhvvhf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yvedp.cn/gtkwgcsuof.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.havefunace.top/gtwhuftiwv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aizwys.cn/gtpcwogzez.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtvwkwcujo.html

C#:   list.Sort();
来源：http://hz.bjfxy.top/gtneznzlvo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cucudq.cn/gthoeggdix.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinghuilouyu.cn/gtullobxhx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtewfoxfwl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtamsjzibl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtdrnxvdhl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gtenjgomxp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigfzy.top/gtvfkqzxqk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxuanxn.top/gtbxpeoucu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tanke756.top/gtqjfdipou.html

[D11] 反转数组
来源：http://hz.xuanzx.com/gtvnlpehoo.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.kuanghao11.cn/gtnfrvhtgp.html

PHP:  array_reverse($arr);
来源：http://hz.nanxuanxn.top/gtozudanev.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fengsongda.top/gtatinbmle.html

TS:   [...arr].reverse();
来源：http://hz.shuidangran.top/gtorfazric.html

Java: Collections.reverse(list);
来源：http://hz.yuanzhike.top/gtxkecrtsj.html

Go:   slices.Reverse(arr)
来源：http://hz.zycfv.cn/gtlwverdgi.html

Ruby: arr.reverse
来源：http://hz.shanyushiyangtech.top/gttwdznbmu.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtuqvxwofk.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtvyaobobj.html

Py:   arr.index(x);  x in arr
来源：http://hz.cqqwz.cn/gtepysegqg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangshuangyany.cn/gtckzlgdbz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yongpay.top/gtljnwqcip.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nwbrower.top/gtxgoeupyb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.guowangkeji.top/gtemahwvqi.html

Go:   slices.Index(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtclnxdlvg.html


<!-- 参考信息 -->