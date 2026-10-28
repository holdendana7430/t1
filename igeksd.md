代发 wailian999

[B13] 判断是否为数字
来源：http://hz.aibaodan.cn/gtdclltuwp.html

Py:   isinstance(x, (int, float))
来源：http://hz.zycfv.cn/gtsvqnvjey.html

PHP:  is_numeric($x)
来源：http://hz.nanxuanxn.top/gtzoemynid.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtcvqwkumw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.redwolf501.top/gtwcnaabvo.html

Java: x instanceof Number
来源：http://hz.nanxuanxn.top/gtmtgmsxik.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.52xcode.cn/gtzujqbwzh.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cdnleiting.top/gtnnpimevm.html

C#:   x is int or double or decimal
来源：http://hz.zhongyouzk.top/gtueampgrh.html

[B14] 判断值是否在集合内
来源：http://hz.redwolf501.top/gtaeehxsec.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangkeji.top/gtylgstdsa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ivvv.top/gtqyuepxia.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gtlohbkswf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtsfhtomkm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guannengcc.top/gtqafiibbf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxuanxn.top/gtfenrqimz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jqgfzy.top/gtkbhwmkck.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.svipenyu.cn/gtvpdreidg.html

[B15] 布尔运算与取反
来源：http://hz.gotoacloud.top/gtbpzuofnz.html

Py:   a and b or not c
来源：http://hz.xziqi.cn/gtytucenkc.html

PHP:  $a && $b || !$c
来源：http://hz.sxryk.cn/gtumaxebgh.html

JS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtanvxgizf.html

TS:   a && b || !c
来源：http://hz.yanxiufei.cn/gtdotmaapw.html

Java: a && b || !c
来源：http://hz.daria6918.cn/gtublzfvnf.html

Go:   a && b || !c
来源：http://hz.svipenyu.cn/gtcizfskfs.html

Ruby: a && b || !c
来源：http://hz.sysykeji.top/gtkkqadxuj.html

C#:   a && b || !c
来源：http://hz.yongpay.top/gtetbnyuex.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hysaishi.cn/gturpwxwlh.html

Py:   if not data: return
来源：http://hz.guowangkeji.top/gtgfjeewms.html

PHP:  if (!$data) { return; }
来源：http://hz.yueranfly.top/gtixtrreck.html

JS:   if (!data) return;
来源：http://hz.dashuyun.cn/gtzxzweefa.html

TS:   if (!data) return;
来源：http://hz.9152youxi.cn/gtpoxwvuta.html

Java: if (data == null) return;
来源：http://hz.meibo888.top/gtoviyxadw.html

Go:   if data == nil { return }
来源：http://hz.9152youxi.cn/gtqyeewsxa.html

Ruby: return if data.nil?
来源：http://hz.xylfe.cn/gtsnfrbhup.html

C#:   if (data == null) return;
来源：http://hz.yueranfly.top/gtvrkmtphq.html

================================================================================
来源：http://hz.cqqwz.cn/gtvelarqit.html

C. 函数与作用域
来源：http://hz.jlsjyb.cn/gtsrskurae.html

================================================================================
来源：http://hz.bjfxy.top/gtwhrqseaq.html

[C01] 定义函数
来源：http://hz.zycfv.cn/gtmdhjtfyq.html

Py:   def add(a, b): return a + b
来源：http://hz.xinyue.icu/gtuvxcblde.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtacgbwgmn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gtelrzbrhy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtvcxjohxm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtgxrqoqpb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zycfv.cn/gtunnbtczq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.bjfxy.top/gtqftkmjsj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtwuyawyxx.html

[C02] 默认参数
来源：http://hz.iojbl.cn/gtpymvtzku.html

Py:   def greet(name="World"): return name
来源：http://hz.zhengqikj.top/gtdsgnwyrx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hysaishi.cn/gtlqshgity.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shanyushiyangtech.top/gtswfnomnm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.52xcode.cn/gtbkukoqyy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangdashe.top/gtkmgypzje.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gzhubu.top/gtvzmzzzbl.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhongyouzk.top/gtdzrvjfhc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xylfe.cn/gtqhblidek.html

[C03] 可变参数
来源：http://hz.yvedp.cn/gtwfnbczkt.html

Py:   def total(*args): return sum(args)
来源：http://hz.52xcode.cn/gttsvujayx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ydjk.org.cn/gtfaermqss.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sysykeji.top/gttlbrwuwl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.9152youxi.cn/gtvqwlwpaz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ybcxt.top/gtfyojtenz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jyoumei.cn/gttpbptfcp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xylfe.cn/gtlvtffuhl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ywan-chungtsiang.top/gtiidkrunz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangdashe.top/gtrkqyvnlf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.pengpengdd.cyou/gtlvvqvhir.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.aibaodan.cn/gtlvbchosu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtcesbildd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sweek.top/gtpjyalwzp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yongpay.top/gtmvybqpid.html

Go:   // 无：用配置结构体参数
来源：http://hz.hywenlv.cn/gtletvdztz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtrpnasbqi.html

C#:   f(a: 1, b: 2)
来源：http://hz.haohaochexian.top/gtdxxqjjxn.html

[C05] 返回多个值
来源：http://hz.yj20258.top/gtdgwagdua.html

Py:   return a, b
来源：http://hz.tanke756.top/gtmglitcdh.html

PHP:  return [$a, $b];
来源：http://hz.havefunace.top/gtemqdojck.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinghuilouyu.cn/gttsjlbxyi.html

TS:   return { a, b };
来源：http://hz.zhijiandao.cn/gthaicmkts.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.pengpengdd.cyou/gtildbjyfr.html

Go:   return a, b
来源：http://hz.hfpthk.cn/gtntovgfdn.html

Ruby: return a, b
来源：http://hz.zycfv.cn/gtmltmbgir.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhijiandao.cn/gturshszvs.html

[C06] 匿名函数 / lambda
来源：http://hz.sxryk.cn/gtoqcbahtf.html

Py:   square = lambda x: x * x
来源：http://hz.shzxlz.cn/gtbysjcvve.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xingfuxueyuan.xyz/gtntptodbj.html

JS:   const square = x => x * x;
来源：http://hz.guannengcc.top/gthaunylbv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cucudq.cn/gtzmppfafc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.birdmap.top/gtfmcjgmnq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hywenlv.cn/gtpbnzsmaq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxinkj.top/gtxqtreajh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jyoumei.cn/gtveqgoyqx.html

[C07] 把函数作为参数传入
来源：http://hz.ydjk.org.cn/gtnvrlnuim.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shuidangran.top/gtlmuvnvud.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.bjfxy.top/gtcvbtcsel.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj20258.top/gtdhhubozm.html

TS:   arr.map(String)
来源：http://hz.smart0.xyz/gtdhfasgdk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gogol.net.cn/gtbjklvfmf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yvedp.cn/gtlcflfvbm.html

Ruby: arr.map(&:upcase)
来源：http://hz.hnqzz.top/gtpsufzuxw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daria6918.cn/gtaibptxwj.html

[C08] 闭包
来源：http://hz.gogol.net.cn/gtcobcnlml.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sufxvd.cn/gtxytpbyxa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yongpay.top/gtepwbdxzv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtetavtwpa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtjfftnayz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zdqjudy.top/gtgtleappu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.iojbl.cn/gtkbgzfizm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinghuilouyu.cn/gtxaynyfmy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gzhubu.top/gtcsslifxl.html

[C09] 递归
来源：http://hz.yuxming.cn/gtnyoswugh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daxiang520.top/gtsvuvukqp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cheryme.top/gtdoeercfe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.316326.xyz/gtyxoscnus.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gtnstegrgv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tianlin.xyz/gthtqhdexi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aizwys.cn/gtlkoqbjhj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhixingplan.top/gtbyowlkap.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.guowangkeji.top/gtktokhduw.html

[C10] 变量作用域
来源：http://hz.shzxlz.cn/gtzevnbfos.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuxming.cn/gtticdzhck.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.iojbl.cn/gtxxsxqijj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sysykeji.top/gtoczaeiez.html

TS:   同 JS
来源：http://hz.tian-w.cn/gtrkvhhozw.html

Java: 方法内为块级作用域
来源：http://hz.jinqigfzy.top/gtutobrbmy.html

Go:   花括号块级作用域
来源：http://hz.0kj1m.cn/gtlpfjtguf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zdqjudy.top/gtfvzosxgx.html

C#:   块级作用域
来源：http://hz.jiagoushi.top/gttlqnimdd.html

[C11] 模块导入与导出
来源：http://hz.xinyue.icu/gtumhxaqpc.html

Py:   from module import func
来源：http://hz.chenzaomai.com/gtwesuqswm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuxming.cn/gtotlhitps.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fzhhl.top/gtnijtegui.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fzhhl.top/gtcpsknpuj.html

Java: import java.util.List;
来源：http://hz.jqgfzy.top/gtdopssfhi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.haohaochexian.top/gtsqnturfw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtgrbbxtpr.html

C#:   using System.Text;
来源：http://hz.iojbl.cn/gtraezjlte.html

[C12] 立即执行函数 IIFE
来源：http://hz.ywan-chungtsiang.top/gtuivrjjjl.html

Py:   (lambda: print("run"))()
来源：http://hz.yj202588.top/gttlqxqghb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cucudq.cn/gtrejvaoxm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.snrcjt.cn/gtycrwczid.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtxlkhigqn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuanzx.com/gtkmskhgyk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.birdmap.top/gtswtmaare.html

Ruby: -> { puts "run" }.call
来源：http://hz.ybcxt.top/gtycfwftlh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jianghu66.top/gtlqbirhig.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydzc1.top/gtgripcfcm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zycfv.cn/gtebipygmr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtodirlsqm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gaohongyu789.top/gtwspuxmkc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj202588.top/gtulhhlslz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtictuywzr.html

Go:   func add(a, b int) int
来源：http://hz.yangfankeji.com/gtrguhhlwk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.0kj1m.cn/gtxvezgjwa.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daxiang520.top/gtmwoidjzf.html

[C14] 泛型函数
来源：http://hz.iojbl.cn/gthahjcxii.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.snrcjt.cn/gtkzqiogsn.html

PHP:  // 无泛型
来源：http://hz.wangdashe.top/gtdtgfcljp.html

JS:   // 无泛型
来源：http://hz.c1oappe.top/gtncghowwg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.meibo888.top/gtqabeilth.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daria6918.cn/gtfmauizsn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydjk.org.cn/gtvjqfsaho.html

Ruby: # 无泛型
来源：http://hz.gotoacloud.top/gtmjmtldxi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhengqikj.top/gtkbojvyxu.html

[C15] 解构 / 展开参数
来源：http://hz.smart0.xyz/gtldoapoon.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258888.top/gtwkgrihbb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zycfv.cn/gtxhzbojdp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.52xcode.cn/gtqziaapjw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yonumen.top/gtoddtwztk.html

Java: // 无解构
来源：http://hz.quarkkingdee.top/gtuxdibyvy.html

Go:   // 无解构
来源：http://hz.jlsjyb.cn/gtnvdopzhz.html

Ruby: a, b = pair
来源：http://hz.yuxming.cn/gtlahhbool.html

C#:   var (a, b) = pair;
来源：http://hz.cashguo.top/gtmpglgnim.html

[C16] 函数 / 方法重载
来源：http://hz.zhiwuduotai.top/gtylbnamvz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cdnleiting.top/gtmiqquedp.html

PHP:  // 无重载
来源：http://hz.chenlongwang.top/gtutccdxtk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ehwqpu.com/gtssjmeays.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gotoacloud.top/gtjdrsqdwy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuetiantiany.cn/gtwlnttreo.html

Go:   // 无重载：用不同函数名
来源：http://hz.ppjwa.cn/gtxbtoqhqv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gogol.net.cn/gtlmareidi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guannengcc.top/gtplcszzvq.html

================================================================================
来源：http://hz.gotoacloud.top/gtfddpgckm.html

D. 数组 / 列表 / 集合
来源：http://hz.9152youxi.cn/gttrznmpkm.html

================================================================================
来源：http://hz.chenlongwang.top/gttqsexcpy.html

[D01] 创建数组 / 列表
来源：http://hz.chenlongwang.top/gtdcyrtkwz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jiagoushi.top/gtzxvprbfx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj202588.top/gtrpfrnhnm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigfzy.top/gtrrsuxqnr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cucudq.cn/gtcvqbrrkd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hnxiangtu.top/gtsxkjqasu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daria6918.cn/gtywflguuq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangdashe.top/gtiyrpzcer.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.haohaochexian.top/gtmzmzxwek.html

[D02] 追加元素到末尾
来源：http://hz.zhaomingkeji.xyz/gthyndrumb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ywan-chungtsiang.top/gtrqjpjmeb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xylfe.cn/gtcqvepmnh.html

JS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtbrmrwioo.html

TS:   arr.push(4);
来源：http://hz.cqqwz.cn/gtdathgxtl.html

Java: list.add(4);
来源：http://hz.havefunace.top/gtlylesudx.html

Go:   arr = append(arr, 4)
来源：http://hz.ywan-chungtsiang.top/gtoppnhdru.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gttsolacvw.html

C#:   list.Add(4);
来源：http://hz.nwbrower.top/gtxzpjrguj.html

[D03] 在指定位置插入元素
来源：http://hz.cheryme.top/gtdqbgplcu.html

Py:   arr.insert(0, 0)
来源：http://hz.xuanzx.com/gtdqkicfkt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinyuanbaomall.cn/gtvlznvajr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangdashe.top/gtlvngnipk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.c1oappe.top/gtjrxnbuns.html

Java: list.add(0, 0);
来源：http://hz.zycfv.cn/gtqlntcgqd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shuidangran.top/gtbqxutqin.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtmjviysov.html

C#:   list.Insert(0, 0);
来源：http://hz.hongshengwenyu.top/gtmizekhhy.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtrqafkbck.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnxiangtu.top/gtnatrqbkg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gtggodvgza.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gtskkzsibj.html

TS:   arr.splice(0, 1);
来源：http://hz.xuetiantiany.cn/gtqyxfjhlz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shangyingyoupin.top/gtfhhkpbzi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhongyouzk.top/gtjpxcezdl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.havefunace.top/gthhtrbdnn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuanzhike.top/gtzwgrblli.html

[D05] 访问与修改元素
来源：http://hz.hammf.cn/gtitwvyfpk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtruturwyo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gtwnngbosm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.meibo888.top/gtqdtpiueu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sweek.top/gtsajzwoig.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sufxvd.cn/gtntnasbas.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtexfpranr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.mhx1999.top/gtfiqvhwar.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.fzhhl.top/gttyjbadju.html

[D06] 数组长度
来源：http://hz.shzxlz.cn/gtcdxaniyy.html

Py:   len(arr)
来源：http://hz.mhx1999.top/gttkikwfxb.html

PHP:  count($arr);
来源：http://hz.dianchejie.cn/gtatzydvyn.html

JS:   arr.length
来源：http://hz.gotoacloud.top/gtfyiylhna.html

TS:   arr.length
来源：http://hz.daria6918.cn/gtnmeafwzu.html

Java: list.size();
来源：http://hz.316326.xyz/gtjmitqlwd.html

Go:   len(arr)
来源：http://hz.cucudq.cn/gtejnpboco.html

Ruby: arr.length; arr.size
来源：http://hz.fzhhl.top/gtmvvlljjo.html

C#:   list.Count;
来源：http://hz.pycfn.com/gtecerceyu.html

[D07] 切片 / 取子数组
来源：http://hz.zycfv.cn/gtkmdafaeg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj202588.top/gthlwjwznd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.0kj1m.cn/gtquwjcedj.html

JS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtwcsevlmz.html

TS:   arr.slice(1, 4);
来源：http://hz.chenlongwang.top/gtaquxmlce.html

Java: list.subList(1, 4);
来源：http://hz.chenlongwang.top/gtoewdsrvg.html

Go:   arr[1:4]
来源：http://hz.chenjidiqi.icu/gtmfomubxl.html

Ruby: arr[1, 3]
来源：http://hz.jqgufenzy.top/gtzvjdrash.html

C#:   list.GetRange(1, 3);
来源：http://hz.cdnleiting.top/gtrwmgttzz.html

[D08] 合并两个数组
来源：http://hz.jinyuanbaomall.cn/gtpgothmbh.html

Py:   a + b;  a.extend(b)
来源：http://hz.gzhubu.top/gttfqwmbkl.html

PHP:  array_merge($a, $b);
来源：http://hz.hywenlv.cn/gtsffuzmui.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hammf.cn/gtnusccdhn.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangtech.top/gtnpgjntzj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.havefunace.top/gthlofebzs.html

Go:   append(a, b...)
来源：http://hz.feifeiyinyue.top/gtmpstxirw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shuidangran.top/gtvbwrliqp.html

C#:   a.Concat(b).ToList()
来源：http://hz.fzhhl.top/gthlvzbfva.html

[D09] 排序（升序）
来源：http://hz.chenlongwang.top/gtuuaqzivc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtsizsghgy.html

PHP:  sort($arr);
来源：http://hz.yuxming.cn/gtmaaizwmd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sufxvd.cn/gtthfmuccr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhengqikj.top/gtumcibipp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.9152youxi.cn/gtaehshxmt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtjigjuiia.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtfndhzbpc.html

C#:   list.Sort();
来源：http://hz.yanxiufei.cn/gttozyoyao.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.iojbl.cn/gtzwyzpyng.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangshuangyany.cn/gthkxejwrz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtkwcppaqp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtufaqgyjz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtguaqkqwx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sweek.top/gteurgprwq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenjidiqi.icu/gtbpxeiiag.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenjidiqi.icu/gtupdrglpc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.redwolf501.top/gtxosudfxd.html

[D11] 反转数组
来源：http://hz.jianghu66.top/gtkkizchcn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.meibo888.top/gtvckezgqe.html

PHP:  array_reverse($arr);
来源：http://hz.daxiang520.top/gtckewahmr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258.top/gtsqgowvqu.html

TS:   [...arr].reverse();
来源：http://hz.zhaomingkeji.xyz/gthzehlyou.html

Java: Collections.reverse(list);
来源：http://hz.hnxiangtu.top/gtlpdkoyui.html

Go:   slices.Reverse(arr)
来源：http://hz.hnxiangtu.top/gtynpaqotm.html

Ruby: arr.reverse
来源：http://hz.sysykeji.top/gtmyrwqaam.html

C#:   list.Reverse();
来源：http://hz.gzhubu.top/gtybwprlml.html

[D12] 查找元素下标
来源：http://hz.zycfv.cn/gtlitwzklm.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258.top/gttboqzkii.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dashuyun.cn/gtcchhwfag.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtoymxxpaj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gtxvhcckhn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daxiang520.top/gtcmjombgm.html

Go:   slices.Index(arr, x)
来源：http://hz.xziqi.cn/gtqmhphnia.html

Ruby: arr.index(x)
来源：http://hz.mhx1999.top/gtspimkhop.html

C#:   list.IndexOf(x);
来源：http://hz.pengpengdd.cyou/gtzoofkync.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shangyingyoupin.top/gtaqssqynj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yangfankeji.com/gtvaatnqji.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guowangkeji.top/gtdguriocg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtqxyquixn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cashguo.top/gtndkmvzex.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ivvv.top/gtfjtggljn.html


<!-- 参考信息 -->