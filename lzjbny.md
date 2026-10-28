代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnxiangtu.top/gtugxybejm.html

Java: x instanceof Number
来源：http://hz.hammf.cn/gtgcmnhvcg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sufxvd.cn/gtpeajstzd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuetiantiany.cn/gthurgvbgm.html

C#:   x is int or double or decimal
来源：http://hz.yueranfly.top/gtdaumeliu.html

[B14] 判断值是否在集合内
来源：http://hz.hfpthk.cn/gtdagyaizf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.redwolf501.top/gtvmbrytlr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydzc1.top/gtorcyenwm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cheryme.top/gtjdbsemsx.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gzhubu.top/gtgprggfgi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.wangdashe.top/gtqisdrigs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dashuyun.cn/gtmrhmtjee.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hfpthk.cn/gtyyteiddy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cdnleiting.top/gtpldlgqad.html

[B15] 布尔运算与取反
来源：http://hz.nanxinkj.top/gtduwsvunl.html

Py:   a and b or not c
来源：http://hz.birdmap.top/gtbjqmtczm.html

PHP:  $a && $b || !$c
来源：http://hz.xuetiantiany.cn/gtgycegped.html

JS:   a && b || !c
来源：http://hz.hnxiangtu.top/gtbsochgdn.html

TS:   a && b || !c
来源：http://hz.yj202588.top/gtugfpbahh.html

Java: a && b || !c
来源：http://hz.tian-w.cn/gtgmamfjhp.html

Go:   a && b || !c
来源：http://hz.gzhubu.top/gtkjmgxsuh.html

Ruby: a && b || !c
来源：http://hz.guannengcc.top/gtigmhwhsk.html

C#:   a && b || !c
来源：http://hz.yj20258888.top/gtnciqaxuo.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.dashuyun.cn/gtsltoxhbo.html

Py:   if not data: return
来源：http://hz.cheryme.top/gtmbvwubqm.html

PHP:  if (!$data) { return; }
来源：http://hz.tanke756.top/gtxefbpzdb.html

JS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtgcrypawp.html

TS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtyigwrhjj.html

Java: if (data == null) return;
来源：http://hz.jqgufenzy.top/gturtkojik.html

Go:   if data == nil { return }
来源：http://hz.gaohongyu789.top/gtfpqvuzbi.html

Ruby: return if data.nil?
来源：http://hz.cucudq.cn/gtwiqsgeqx.html

C#:   if (data == null) return;
来源：http://hz.dashuyun.cn/gtivfukrpw.html

================================================================================
来源：http://hz.sxryk.cn/gtddacygdo.html

C. 函数与作用域
来源：http://hz.zhiwuduotai.top/gtmflmfczz.html

================================================================================
来源：http://hz.chenzaomai.com/gtzyjwxdyf.html

[C01] 定义函数
来源：http://hz.yueranfly.top/gtqmrjhwli.html

Py:   def add(a, b): return a + b
来源：http://hz.redwolf501.top/gthqdkeetf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtqjwialcw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtrhwohhsd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhiwuduotai.top/gtooupbiwx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtkqhhtwmf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhaomingkeji.xyz/gtrszyyzil.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yuanzhike.top/gtiyyvfgde.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtmuanwsmf.html

[C02] 默认参数
来源：http://hz.yj20258888.top/gtyxdecybp.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gtzdsrtmmz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhijiandao.cn/gtbakaeedj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yueranfly.top/gtznfyexmk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xingfuxueyuan.xyz/gttbjldvtm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yvedp.cn/gtroqymovd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.aibaodan.cn/gtneqmpuli.html

Ruby: def greet(name = "World") = name
来源：http://hz.yueranfly.top/gtyqnpnylz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.smart0.xyz/gtqkoxuimv.html

[C03] 可变参数
来源：http://hz.yangfankeji.com/gtbjxxpckj.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhixingplan.top/gtxrdqwbnz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jyoumei.cn/gtvybmprgf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtgnyktqte.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtrerfhsta.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtjamuiuex.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.svipenyu.cn/gtenjfsbti.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.pycfn.com/gtvpmwpdsx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.guannengcc.top/gtrvzhjhgn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nanxinkj.top/gtjrrubshg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhijiandao.cn/gtyvauozlb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shanyushiyangtech.top/gtrgfirrpn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtvyagtjit.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.dashuyun.cn/gtflvwjbtz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhaomingkeji.xyz/gtecfwdgqx.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigufen.top/gtrkppkczm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtzohqrfix.html

C#:   f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtdtispogj.html

[C05] 返回多个值
来源：http://hz.jinqigufen.top/gtxftdxncn.html

Py:   return a, b
来源：http://hz.andypj.xyz/gtshgscbhu.html

PHP:  return [$a, $b];
来源：http://hz.gaohongyu789.top/gtaytrmnxs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gogol.net.cn/gtnyktlfiw.html

TS:   return { a, b };
来源：http://hz.wangshuangyany.cn/gtarwgxocl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhoulong.xyz/gtucicwfoi.html

Go:   return a, b
来源：http://hz.shangyingyoupin.top/gtnsbkxcbg.html

Ruby: return a, b
来源：http://hz.316326.xyz/gtfrqfxlyc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.bjfxy.top/gtksnopjhv.html

[C06] 匿名函数 / lambda
来源：http://hz.jinghuilouyu.cn/gtgnopbenw.html

Py:   square = lambda x: x * x
来源：http://hz.ydjk.org.cn/gtbgpzujrv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yueranfly.top/gtlxdswflv.html

JS:   const square = x => x * x;
来源：http://hz.haohaochexian.top/gtpaklhafr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhijiandao.cn/gtwlsprodq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ybcxt.top/gtkhconacq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tian-w.cn/gtvhnuwhnd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.mhx1999.top/gtzilofkob.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.meibo888.top/gtxljsvaqe.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigfzy.top/gtclvpgrea.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sysykeji.top/gtlsdyckpp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tianlin.xyz/gtlqokhaui.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daxiang520.top/gtnujwvdls.html

TS:   arr.map(String)
来源：http://hz.quarkkingdee.top/gtyhmorbsg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.svipenyu.cn/gtslgvroap.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.feifeiyinyue.top/gtvlyxserh.html

Ruby: arr.map(&:upcase)
来源：http://hz.snrcjt.cn/gtwsjteiez.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.tian-w.cn/gtpngrojuv.html

[C08] 闭包
来源：http://hz.9152youxi.cn/gtuodmwimt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yueranfly.top/gtxxxoqnse.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangtech.top/gtqorkukms.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtwyjwwklr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtiqbkrukg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.0kj1m.cn/gtxqudceci.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hammf.cn/gtqbqofmwk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yvedp.cn/gthfczwpux.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtaiktpoat.html

[C09] 递归
来源：http://hz.snrcjt.cn/gtfeafnmna.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenzaomai.com/gtzpybqzcb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.dianchejie.cn/gtmdjqtfep.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gthbfpfave.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gtdazyrmnd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenjidiqi.icu/gtgbhxrhkm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigfzy.top/gtsabpjevo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jyoumei.cn/gtqovbjkpl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnxiangtu.top/gtqwxljdgj.html

[C10] 变量作用域
来源：http://hz.yonumen.top/gtlevphmrl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258.top/gttdbralpm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangkeji.top/gtulvsfbqg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnxiangtu.top/gtzpfymhxx.html

TS:   同 JS
来源：http://hz.pycfn.com/gttjtppmkh.html

Java: 方法内为块级作用域
来源：http://hz.redwolf501.top/gtdkjfcfri.html

Go:   花括号块级作用域
来源：http://hz.pycfn.com/gtdgxafgly.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.vqdsnc.cn/gtjzxvfbxw.html

C#:   块级作用域
来源：http://hz.feifeiyinyue.top/gtlzgzthfy.html

[C11] 模块导入与导出
来源：http://hz.hongshengwenyu.top/gttmfzupqa.html

Py:   from module import func
来源：http://hz.0kj1m.cn/gtrjikaalm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj20258.top/gtcsvmksdh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangtech.top/gtoyjnkovl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.aizwys.cn/gtnskzhjzd.html

Java: import java.util.List;
来源：http://hz.gogol.net.cn/gtklzdpzpt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jianghu66.top/gthpgacikc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigufen.top/gttmjebmlg.html

C#:   using System.Text;
来源：http://hz.ppjwa.cn/gtgpcqvgvm.html

[C12] 立即执行函数 IIFE
来源：http://hz.haohaochexian.top/gtcgodeinl.html

Py:   (lambda: print("run"))()
来源：http://hz.smart0.xyz/gtckbbcxeg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtulbtuenc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.feifeiyinyue.top/gtftbrkzcf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtlthovkjc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ydjk.org.cn/gtpcslqefz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jyoumei.cn/gtjospwkum.html

Ruby: -> { puts "run" }.call
来源：http://hz.52xcode.cn/gtcewyuiuo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258.top/gtcnpenczx.html

[C13] 类型声明 / 类型注解
来源：http://hz.jlsjyb.cn/gtpxpcpokx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hongshengwenyu.top/gtsikdiqlx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtlsluqwzn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zycfv.cn/gtushrmroc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtjqdkagfi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtfhyqeomo.html

Go:   func add(a, b int) int
来源：http://hz.yuxming.cn/gtizudhkyl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgfzy.top/gtwoeihvac.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydzc1.top/gtqwqssnyn.html

[C14] 泛型函数
来源：http://hz.hnqzz.top/gtogbjczst.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtijhuscot.html

PHP:  // 无泛型
来源：http://hz.yj20258.top/gtyeghermq.html

JS:   // 无泛型
来源：http://hz.cashguo.top/gtojnmjfah.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgufenzy.top/gtkxglfrzv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhixingplan.top/gtfjjnuzth.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.andypj.xyz/gtakvkpkim.html

Ruby: # 无泛型
来源：http://hz.zhengqikj.top/gtzhjlqymg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangdashe.top/gtvxronspl.html

[C15] 解构 / 展开参数
来源：http://hz.yanxiufei.cn/gtzyjmhfwu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shanyushiyangkeji.top/gtsublshoe.html

PHP:  [$a, $b] = $pair;
来源：http://hz.52xcode.cn/gtfutsrurj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yangfankeji.com/gtpnftgaho.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fengsongda.top/gtpwstsghh.html

Java: // 无解构
来源：http://hz.ppjwa.cn/gtjfntbkld.html

Go:   // 无解构
来源：http://hz.kuanghao11.cn/gtsgtmjcty.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtpambqyqo.html

C#:   var (a, b) = pair;
来源：http://hz.jinghuilouyu.cn/gtehepdbfv.html

[C16] 函数 / 方法重载
来源：http://hz.ybcxt.top/gtvlxwpbhl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guannengcc.top/gtbpekemnw.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gtqeagucmk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxinkj.top/gtlvzwhwki.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daxiang520.top/gtskvyyjgf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinghuilouyu.cn/gtkpzomhzz.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuxming.cn/gtuulwqmyz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ydzc1.top/gtvusjykor.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cucudq.cn/gtyypznlpg.html

================================================================================
来源：http://hz.iojbl.cn/gtdccgufxh.html

D. 数组 / 列表 / 集合
来源：http://hz.chenjidiqi.icu/gtlyndxwzs.html

================================================================================
来源：http://hz.sysykeji.top/gtgwkdmnxw.html

[D01] 创建数组 / 列表
来源：http://hz.jinghuilouyu.cn/gtswbxhbig.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xinyue.icu/gtncxszhyx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aibaodan.cn/gtbpzegutx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guannengcc.top/gtdoxkoxeq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhaomingkeji.xyz/gtchyfzndy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cucudq.cn/gtlvmgcdyw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cqqwz.cn/gttcwkohjm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sweek.top/gtzdhexepr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tanke756.top/gtrtmdcgsl.html

[D02] 追加元素到末尾
来源：http://hz.zhengqikj.top/gtsvsolaup.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cheryme.top/gtcxdpijbn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gteeardbdw.html

JS:   arr.push(4);
来源：http://hz.hfpthk.cn/gtchlufjsr.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtllaontci.html

Java: list.add(4);
来源：http://hz.cashguo.top/gtenxghhcz.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgufenzy.top/gtrtdjhaoz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhengqikj.top/gtxcxdmvhf.html

C#:   list.Add(4);
来源：http://hz.0kj1m.cn/gtfcvzwldt.html

[D03] 在指定位置插入元素
来源：http://hz.jlsjyb.cn/gtondixcek.html

Py:   arr.insert(0, 0)
来源：http://hz.sweek.top/gthyavrhno.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dianchejie.cn/gtbkpypfia.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ybcxt.top/gtbsvkktly.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtbtjbsqcj.html

Java: list.add(0, 0);
来源：http://hz.cqqwz.cn/gtibvnjdor.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jiagoushi.top/gtgurbvcmx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtqdakrxmw.html

C#:   list.Insert(0, 0);
来源：http://hz.birdmap.top/gtbkkjqaug.html

[D04] 删除元素
来源：http://hz.havefunace.top/gtfdlgdxll.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ivvv.top/gtgfwsistv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ydzc1.top/gtfpnajvne.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tanke756.top/gturygcfww.html

TS:   arr.splice(0, 1);
来源：http://hz.shzxlz.cn/gtypprtgjf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shuidangran.top/gtghfslgrs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenlongwang.top/gtxqrgezmn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tianlin.xyz/gtdmdvwljh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.dianchejie.cn/gtreixegzu.html

[D05] 访问与修改元素
来源：http://hz.wangdashe.top/gtcniwjnhr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtdwzsvbme.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ehwqpu.com/gtmvjndjdg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hfpthk.cn/gtomeqhpml.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258.top/gtgvdjvtku.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenzaomai.com/gtpnvvnmxn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtthysccjb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtnfzuqevf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.fengsongda.top/gtwvvvhska.html

[D06] 数组长度
来源：http://hz.gogol.net.cn/gtncwiwuiu.html

Py:   len(arr)
来源：http://hz.zdqjudy.top/gtcdkrbfkn.html

PHP:  count($arr);
来源：http://hz.aibaodan.cn/gtfksntfen.html

JS:   arr.length
来源：http://hz.daxiang520.top/gtzvqlyybd.html

TS:   arr.length
来源：http://hz.jlsjyb.cn/gtujvlzmgg.html

Java: list.size();
来源：http://hz.gogol.net.cn/gtkodjhliu.html

Go:   len(arr)
来源：http://hz.smart0.xyz/gtelychycl.html

Ruby: arr.length; arr.size
来源：http://hz.hysaishi.cn/gtwkekpkux.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtdsbyjuao.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gtkewaxqwy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhiwuduotai.top/gtwlxadvqc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhengqikj.top/gtvgncvjls.html

JS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtkdnaugij.html

TS:   arr.slice(1, 4);
来源：http://hz.cashguo.top/gtdcssgjlb.html

Java: list.subList(1, 4);
来源：http://hz.fengsongda.top/gtioitywaq.html

Go:   arr[1:4]
来源：http://hz.aizwys.cn/gtroxhsweb.html

Ruby: arr[1, 3]
来源：http://hz.xinyue.icu/gtxofrdxyu.html

C#:   list.GetRange(1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtinbtqfkv.html

[D08] 合并两个数组
来源：http://hz.chenjidiqi.icu/gtivbeytji.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigfzy.top/gtfamoxjhp.html

PHP:  array_merge($a, $b);
来源：http://hz.0kj1m.cn/gtmfmblizf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zycfv.cn/gtytqttydb.html

TS:   [...a, ...b];
来源：http://hz.c1oappe.top/gthsbsasqf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zdqjudy.top/gtdjbhulaf.html

Go:   append(a, b...)
来源：http://hz.xingfuxueyuan.xyz/gtxgyvmjbm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenlongwang.top/gtiachxjlr.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhaomingkeji.xyz/gtrgpjpkhr.html

[D09] 排序（升序）
来源：http://hz.hfpthk.cn/gtakbuhgle.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gturyxjbhi.html

PHP:  sort($arr);
来源：http://hz.aibaodan.cn/gtczqrlfwr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.wangdashe.top/gtnfluuhdu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangdashe.top/gtpmacoqvp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.9152youxi.cn/gtqjypqpts.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtqxubtwud.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtcufkgzqg.html

C#:   list.Sort();
来源：http://hz.cheryme.top/gtjnpjvobc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.0kj1m.cn/gtkumiokxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.pengpengdd.cyou/gtvakwuccq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shuidangran.top/gtrifhrxbu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gtzhhjspgp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtjkwjqgbo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fengsongda.top/gtfmqvygqi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cqqwz.cn/gtfhwlzjdq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhijiandao.cn/gteyncbapn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hysaishi.cn/gtuujbntwi.html

[D11] 反转数组
来源：http://hz.yongpay.top/gtynuyjzjm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.haohaochexian.top/gtnfjpubgr.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gteozikaax.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yanxiufei.cn/gtufyiaivn.html

TS:   [...arr].reverse();
来源：http://hz.iojbl.cn/gtgyglxbzh.html

Java: Collections.reverse(list);
来源：http://hz.aizwys.cn/gtjgouptge.html

Go:   slices.Reverse(arr)
来源：http://hz.andypj.xyz/gtngrkgqsc.html

Ruby: arr.reverse
来源：http://hz.0kj1m.cn/gtybcrlyne.html

C#:   list.Reverse();
来源：http://hz.jinqigufen.top/gttuqklwox.html

[D12] 查找元素下标
来源：http://hz.zhiwuduotai.top/gtdgwikcnx.html

Py:   arr.index(x);  x in arr
来源：http://hz.ppjwa.cn/gtpuhvnnnz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangdashe.top/gtlcckilpb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sweek.top/gtpmdvfnds.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtwjsqtzkr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.aibaodan.cn/gtbmoxhben.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gtwgtlxcng.html

Ruby: arr.index(x)
来源：http://hz.xuanzx.com/gtghgwkuvp.html

C#:   list.IndexOf(x);
来源：http://hz.hywenlv.cn/gtddmdkxrq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhiwuduotai.top/gtrflvlbue.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sysykeji.top/gthbblvydi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtnmfywwom.html

JS:   arr.filter(x => x > 3)
来源：http://hz.havefunace.top/gtduxtrvpx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtompfvjuj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtvzgxmokv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cqqwz.cn/gtykzyqeil.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fengsongda.top/gtbypqyhvo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daria6918.cn/gtodsdorui.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gaohongyu789.top/gtfimbdtve.html


<!-- 参考信息 -->