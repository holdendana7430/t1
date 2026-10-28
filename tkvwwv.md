代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shanyushiyangkeji.top/gtdjnvlqey.html

Ruby: (0...10).step(2).to_a
来源：http://hz.havefunace.top/gtvbstpukk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yueranfly.top/gtqszmjlji.html

[B12] 跳出多层循环
来源：http://hz.dashuyun.cn/gtdtpwjhsf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenzaomai.com/gtbhngvcik.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhongyouzk.top/gtnyfplymw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtyyaumbgm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtzzkgwglm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtxttogayq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jiagoushi.top/gtexyhynkn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nwbrower.top/gtvwqzgzzr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.haohaochexian.top/gtrnrexpxz.html

[B13] 判断是否为数字
来源：http://hz.sxryk.cn/gtjvnyyeuu.html

Py:   isinstance(x, (int, float))
来源：http://hz.xinyue.icu/gtgtprrthm.html

PHP:  is_numeric($x)
来源：http://hz.xinyue.icu/gtzsawxbew.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gteuaevddn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nanxinkj.top/gtvdhrhfdl.html

Java: x instanceof Number
来源：http://hz.fengsongda.top/gtfzxrbpud.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.dashuyun.cn/gtugsnktxo.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ybcxt.top/gtwcnwjjlq.html

C#:   x is int or double or decimal
来源：http://hz.9152youxi.cn/gtgivvbdnf.html

[B14] 判断值是否在集合内
来源：http://hz.xuanzx.com/gtquwpamqh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhiwuduotai.top/gtfednclxi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydzc1.top/gtffwmlybc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dashuyun.cn/gtebnyhbge.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gotoacloud.top/gtyixwtqfe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xuetiantiany.cn/gtsymgvpuu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jyoumei.cn/gtqdegjfbp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gogol.net.cn/gtkimejdgz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.pycfn.com/gtnsmuxrzk.html

[B15] 布尔运算与取反
来源：http://hz.yuanzhike.top/gtdhumvnxo.html

Py:   a and b or not c
来源：http://hz.pengpengdd.cyou/gtmpucwvxt.html

PHP:  $a && $b || !$c
来源：http://hz.ydjk.org.cn/gtuqpqzvvy.html

JS:   a && b || !c
来源：http://hz.hnqzz.top/gtczamccfc.html

TS:   a && b || !c
来源：http://hz.havefunace.top/gtlhzgaimz.html

Java: a && b || !c
来源：http://hz.pengpengdd.cyou/gtonwnijhu.html

Go:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtymunnsub.html

Ruby: a && b || !c
来源：http://hz.ppjwa.cn/gtkgmleicv.html

C#:   a && b || !c
来源：http://hz.ydzc1.top/gtvopqagwp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.andypj.xyz/gttwwwhlcm.html

Py:   if not data: return
来源：http://hz.dianchejie.cn/gtltfokdji.html

PHP:  if (!$data) { return; }
来源：http://hz.zdqjudy.top/gtgknddrav.html

JS:   if (!data) return;
来源：http://hz.yj20258.top/gtvxoqbgmn.html

TS:   if (!data) return;
来源：http://hz.xziqi.cn/gtpktxbnpf.html

Java: if (data == null) return;
来源：http://hz.316326.xyz/gtmggvtohp.html

Go:   if data == nil { return }
来源：http://hz.9152youxi.cn/gtxoixxzgo.html

Ruby: return if data.nil?
来源：http://hz.zhixingplan.top/gtfnnoubrz.html

C#:   if (data == null) return;
来源：http://hz.cashguo.top/gtbdfzepcv.html

================================================================================
来源：http://hz.iojbl.cn/gtjwlprlci.html

C. 函数与作用域
来源：http://hz.guannengcc.top/gttyjohfmd.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdqacbwjr.html

[C01] 定义函数
来源：http://hz.jiagoushi.top/gtxhibmpdf.html

Py:   def add(a, b): return a + b
来源：http://hz.yj20258.top/gtdxyjebjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtldcljtom.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.dianchejie.cn/gtyjyjjkdg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtfzqonrkf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtriotsdrs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tianlin.xyz/gtlrxoueuq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhiwuduotai.top/gteauuoyhr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtelwznusz.html

[C02] 默认参数
来源：http://hz.pycfn.com/gthstlrtql.html

Py:   def greet(name="World"): return name
来源：http://hz.shangyingyoupin.top/gtkodzrkby.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zycfv.cn/gtgliulhii.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgfzy.top/gtvxoinoue.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtotvysyhz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangkeji.top/gtyjiigheh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.52xcode.cn/gtogorcjcc.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhixingplan.top/gthuvnfley.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cashguo.top/gtynejjaaw.html

[C03] 可变参数
来源：http://hz.ybcxt.top/gtxqmtcaoi.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gtdalststq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nwbrower.top/gtzbrgdxoh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxuanxn.top/gtosxzvyou.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtcklasbln.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.fengsongda.top/gtqpoedigf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sufxvd.cn/gtnulerojz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.vqdsnc.cn/gtczsglvqy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhongyouzk.top/gtbnkervfz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xylfe.cn/gtzqcjfzib.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.snrcjt.cn/gtcxjdicly.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sweek.top/gtrzcwaqan.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cashguo.top/gtrlhtxqob.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cqqwz.cn/gtolxacfrq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guannengcc.top/gtizskuymc.html

Go:   // 无：用配置结构体参数
来源：http://hz.mhx1999.top/gthwxjtuxu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtlcolwlub.html

C#:   f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtyrcqrcrl.html

[C05] 返回多个值
来源：http://hz.316326.xyz/gtorqqvqmb.html

Py:   return a, b
来源：http://hz.shanyushiyangtech.top/gtgirgedbd.html

PHP:  return [$a, $b];
来源：http://hz.fengsongda.top/gtpgafbmyy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shanyushiyangtech.top/gtyonvugub.html

TS:   return { a, b };
来源：http://hz.dashuyun.cn/gtalhoswkh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jiagoushi.top/gtneiankjv.html

Go:   return a, b
来源：http://hz.ydjk.org.cn/gtwttxsugn.html

Ruby: return a, b
来源：http://hz.pengpengdd.cyou/gtxkuktqlb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yongpay.top/gtxhalsbvb.html

[C06] 匿名函数 / lambda
来源：http://hz.zhaomingkeji.xyz/gtkpgobycr.html

Py:   square = lambda x: x * x
来源：http://hz.cashguo.top/gthhdzpcnu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhoulong.xyz/gtdvyjiksh.html

JS:   const square = x => x * x;
来源：http://hz.dashuyun.cn/gtcjvilgeo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenlongwang.top/gtqkaoomqm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jiagoushi.top/gtxqfjxodt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinyuanbaomall.cn/gtiohbteup.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gtugsbfeca.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yongpay.top/gtldqwwplj.html

[C07] 把函数作为参数传入
来源：http://hz.tianlin.xyz/gtmuvxbzwf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj20258.top/gtrzoowtag.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gaohongyu789.top/gtqbrnxtam.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.kuanghao11.cn/gtqbxdlxfu.html

TS:   arr.map(String)
来源：http://hz.hfpthk.cn/gtkygpmfzb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.fengsongda.top/gtwjgciejv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tanke756.top/gtkbbvrgbf.html

Ruby: arr.map(&:upcase)
来源：http://hz.xingfuxueyuan.xyz/gtdvhmpwyl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhengqikj.top/gtecybbunr.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtfcbnvqgw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jqgfzy.top/gtqwsnddjx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zdqjudy.top/gtiojtphim.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtprculaxk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtrxvegpqo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.aibaodan.cn/gtavljcznf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guowangkeji.top/gtstirqkqp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xylfe.cn/gtnkxwuhno.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtbtjtsprx.html

[C09] 递归
来源：http://hz.yvedp.cn/gtlfsabnpq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ydjk.org.cn/gtvpkngbec.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cucudq.cn/gteuvntihq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.316326.xyz/gtrlzfijnn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.snrcjt.cn/gttwcdujzr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shanyushiyangtech.top/gtoamorbjm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sysykeji.top/gtgbjdplte.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtltjeufol.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yanxiufei.cn/gtffwgompm.html

[C10] 变量作用域
来源：http://hz.xuetiantiany.cn/gtyqqitrzc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258.top/gtexrtkqlg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jianghu66.top/gtbqznzilu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cashguo.top/gtzvjlktqw.html

TS:   同 JS
来源：http://hz.zhengqikj.top/gtdoeprcve.html

Java: 方法内为块级作用域
来源：http://hz.aibaodan.cn/gtybjgzxue.html

Go:   花括号块级作用域
来源：http://hz.yj20258888.top/gtsujpxzgi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jyoumei.cn/gtfudubzdg.html

C#:   块级作用域
来源：http://hz.yuxming.cn/gtymimfefa.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtjlteqdpb.html

Py:   from module import func
来源：http://hz.tianlin.xyz/gthjbvexkp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhaomingkeji.xyz/gtxanctavl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yonumen.top/gturklnpwi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.wangshuangyany.cn/gtdkkvtvog.html

Java: import java.util.List;
来源：http://hz.daxiang520.top/gtbgibxyun.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhiwuduotai.top/gtwqqwvedr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258888.top/gtflxqquwp.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtaaaicgyk.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenzaomai.com/gtjxuewpad.html

Py:   (lambda: print("run"))()
来源：http://hz.daria6918.cn/gtpwziyhpr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jlsjyb.cn/gtmpzxokkd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtfttwgodt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtgzrzrsew.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.haohaochexian.top/gtebhtoamj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sufxvd.cn/gtwjqxxook.html

Ruby: -> { puts "run" }.call
来源：http://hz.jiagoushi.top/gtfdaidtqt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.iojbl.cn/gtqjlvpmzx.html

[C13] 类型声明 / 类型注解
来源：http://hz.316326.xyz/gtotviwgoa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangdashe.top/gttuhntajp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtbwilyder.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cashguo.top/gtucuewetd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtsaoyyika.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtfiboqhfg.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtldmcinma.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ehwqpu.com/gtyaqbngby.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fengsongda.top/gtzzddznaw.html

[C14] 泛型函数
来源：http://hz.shuidangran.top/gtpkjgnbqq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangdashe.top/gtnhsvwzpq.html

PHP:  // 无泛型
来源：http://hz.sufxvd.cn/gtyeohjtwu.html

JS:   // 无泛型
来源：http://hz.sysykeji.top/gtsjsozzul.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtbwpggyxo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258888.top/gtftdrufdc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangdashe.top/gtescrqifr.html

Ruby: # 无泛型
来源：http://hz.shuidangran.top/gtrzmpfgqi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hywenlv.cn/gtfegspphy.html

[C15] 解构 / 展开参数
来源：http://hz.hfpthk.cn/gtjpcahuen.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shuidangran.top/gttqofesvk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.haohaochexian.top/gthfcxmtur.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtrhvwgevq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guowangkeji.top/gtsajiawxm.html

Java: // 无解构
来源：http://hz.ybcxt.top/gtiwciuunk.html

Go:   // 无解构
来源：http://hz.daxiang520.top/gttxaqosth.html

Ruby: a, b = pair
来源：http://hz.mhx1999.top/gtpnlgddig.html

C#:   var (a, b) = pair;
来源：http://hz.bjfxy.top/gtxspfaglx.html

[C16] 函数 / 方法重载
来源：http://hz.jqgfzy.top/gtcgfnrgjl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ydjk.org.cn/gtcpvmlffl.html

PHP:  // 无重载
来源：http://hz.birdmap.top/gteouelvzx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.vqdsnc.cn/gtufzqcocl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.316326.xyz/gthilqgpro.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.smart0.xyz/gtvunocjci.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtwokcwovd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtfqkdfqea.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuanzhike.top/gtarvmbggq.html

================================================================================
来源：http://hz.yueranfly.top/gtgqoldbqg.html

D. 数组 / 列表 / 集合
来源：http://hz.bjfxy.top/gtxtfszorx.html

================================================================================
来源：http://hz.jianghu66.top/gtlkdwdlav.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtjefsjihs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ywan-chungtsiang.top/gtjmnsvedw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.316326.xyz/gtjefisarw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenjidiqi.icu/gtvkfcmxkb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xziqi.cn/gtydnxfled.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj202588.top/gtttambljl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cdnleiting.top/gtxflgntvz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtqzcuhxbi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gtytvheudu.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtzbszayiw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangtech.top/gtsbbsnigv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhiwuduotai.top/gtcymsnymr.html

JS:   arr.push(4);
来源：http://hz.jlsjyb.cn/gtijbyqagc.html

TS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtempcbdlb.html

Java: list.add(4);
来源：http://hz.zdqjudy.top/gtcrravqzx.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gtoltzlzre.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.vqdsnc.cn/gtcnegjctg.html

C#:   list.Add(4);
来源：http://hz.zhijiandao.cn/gtxnxeqllb.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtyhivgyav.html

Py:   arr.insert(0, 0)
来源：http://hz.ehwqpu.com/gtljbschkh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhijiandao.cn/gtldhxsdxy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.feifeiyinyue.top/gtxdnrbfbk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgufenzy.top/gtkubetdwh.html

Java: list.add(0, 0);
来源：http://hz.ppjwa.cn/gtrqlguiis.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sweek.top/gtbqhrazsz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.birdmap.top/gtmymrieui.html

C#:   list.Insert(0, 0);
来源：http://hz.haohaochexian.top/gtwlduxftw.html

[D04] 删除元素
来源：http://hz.iojbl.cn/gtkobskczk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtlkujhyfe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hfpthk.cn/gtrpabfovm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cucudq.cn/gtgrivjlhz.html

TS:   arr.splice(0, 1);
来源：http://hz.meibo888.top/gtqjmaabac.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jiagoushi.top/gtvneqpsrs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.feifeiyinyue.top/gtxnwxlaat.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.0kj1m.cn/gtufovomao.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtwenxobpn.html

[D05] 访问与修改元素
来源：http://hz.shangyingyoupin.top/gtedotockz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtnaebwapl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtwdjqntvt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xziqi.cn/gtovwkjkzf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hongshengwenyu.top/gtcaamxkli.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnxiangtu.top/gtcdtyvdgr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtcunxybau.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtscyzmnsy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xziqi.cn/gtqisfvzju.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gtqitydxgl.html

Py:   len(arr)
来源：http://hz.ppjwa.cn/gthojvjstc.html

PHP:  count($arr);
来源：http://hz.yueranfly.top/gtsfidylim.html

JS:   arr.length
来源：http://hz.cdnleiting.top/gtmyhgmuti.html

TS:   arr.length
来源：http://hz.gzhubu.top/gtflporahh.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtlewcjefo.html

Go:   len(arr)
来源：http://hz.shuidangran.top/gtccqcrdmy.html

Ruby: arr.length; arr.size
来源：http://hz.zhaomingkeji.xyz/gtygzrezmt.html

C#:   list.Count;
来源：http://hz.zycfv.cn/gtkefkxppm.html

[D07] 切片 / 取子数组
来源：http://hz.vqdsnc.cn/gtcbtfjqyl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gaohongyu789.top/gtqbsmutai.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.wangdashe.top/gthgfxqpbg.html

JS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gtpvsnivkt.html

TS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtmdkcqwdd.html

Java: list.subList(1, 4);
来源：http://hz.mhx1999.top/gtsnxpapmn.html

Go:   arr[1:4]
来源：http://hz.gzhubu.top/gtsonkzkkx.html

Ruby: arr[1, 3]
来源：http://hz.c1oappe.top/gtxovwdalh.html

C#:   list.GetRange(1, 3);
来源：http://hz.dianchejie.cn/gtsxkbwvdu.html

[D08] 合并两个数组
来源：http://hz.zhiwuduotai.top/gteznlmlzi.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigfzy.top/gtkfmbkyof.html

PHP:  array_merge($a, $b);
来源：http://hz.chenlongwang.top/gtykqigvdc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nanxuanxn.top/gtraofzdjy.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gtazdztfdr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hongshengwenyu.top/gtyhybumuu.html

Go:   append(a, b...)
来源：http://hz.zhaomingkeji.xyz/gttkpsybgv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ywan-chungtsiang.top/gtvrcronnm.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnqzz.top/gtszevqtpm.html

[D09] 排序（升序）
来源：http://hz.9152youxi.cn/gtjzvishnc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gtlhjjgbwf.html

PHP:  sort($arr);
来源：http://hz.wangdashe.top/gtesioxpmp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guowangkeji.top/gtlapmnbbk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenzaomai.com/gtprxuslwr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.pengpengdd.cyou/gtiaxtpiwi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fengsongda.top/gtwfninqxs.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtuwazoenc.html

C#:   list.Sort();
来源：http://hz.yvedp.cn/gtsirjqrde.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangshuangyany.cn/gtysfkrxrx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuxming.cn/gtzbnfaqiy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtigpobnga.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtkmqfjqjb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtzamrlzfe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tanke756.top/gtblbbnqoa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gogol.net.cn/gtjuwvcyfx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhijiandao.cn/gtxtzfxdtm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xylfe.cn/gtmktqkqmn.html

[D11] 反转数组
来源：http://hz.xziqi.cn/gtvquzncdw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fzhhl.top/gtsuukyjot.html

PHP:  array_reverse($arr);
来源：http://hz.zdqjudy.top/gtydvynzik.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ehwqpu.com/gtxkywsjkx.html

TS:   [...arr].reverse();
来源：http://hz.hfpthk.cn/gtllqtlhup.html

Java: Collections.reverse(list);
来源：http://hz.xziqi.cn/gtbitjallq.html

Go:   slices.Reverse(arr)
来源：http://hz.quarkkingdee.top/gtfxdssknl.html

Ruby: arr.reverse
来源：http://hz.sweek.top/gtxlqdgrjg.html

C#:   list.Reverse();
来源：http://hz.aizwys.cn/gtecvuerme.html

[D12] 查找元素下标
来源：http://hz.dianchejie.cn/gtrjfrvcas.html

Py:   arr.index(x);  x in arr
来源：http://hz.fzhhl.top/gthjpgoffe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.snrcjt.cn/gtcljzbtno.html


<!-- 参考信息 -->