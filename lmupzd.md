代发 wailian999

[B13] 判断是否为数字
来源：http://hz.jqgfzy.top/gtgctkqwey.html

Py:   isinstance(x, (int, float))
来源：http://hz.mhx1999.top/gtciqemonr.html

PHP:  is_numeric($x)
来源：http://hz.jyoumei.cn/gtwcwrnafk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.9152youxi.cn/gtlauznpyn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnqzz.top/gtffatefue.html

Java: x instanceof Number
来源：http://hz.yonumen.top/gtyivmrzfd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yonumen.top/gtmgcwlydt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xziqi.cn/gtehtwvqkg.html

C#:   x is int or double or decimal
来源：http://hz.aizwys.cn/gtrpohxsyg.html

[B14] 判断值是否在集合内
来源：http://hz.ehwqpu.com/gtijlflqpa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gogol.net.cn/gtsaofuuty.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shzxlz.cn/gttrncakum.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtgxzvedia.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guannengcc.top/gtgbsbliyy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hnqzz.top/gtjdruyuqm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cdnleiting.top/gtlcmotuvj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenlongwang.top/gtbqgwghwl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zycfv.cn/gtidvomfxe.html

[B15] 布尔运算与取反
来源：http://hz.dianchejie.cn/gtgopaavwb.html

Py:   a and b or not c
来源：http://hz.sweek.top/gtrlyxfpuf.html

PHP:  $a && $b || !$c
来源：http://hz.shanyushiyangtech.top/gtixjghwwu.html

JS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtxgnfwhoi.html

TS:   a && b || !c
来源：http://hz.gotoacloud.top/gtcocumszm.html

Java: a && b || !c
来源：http://hz.sufxvd.cn/gtxosxtgvy.html

Go:   a && b || !c
来源：http://hz.jyoumei.cn/gtsfgqbcgz.html

Ruby: a && b || !c
来源：http://hz.yanxiufei.cn/gtfqbhpdmm.html

C#:   a && b || !c
来源：http://hz.tian-w.cn/gtuxgmfoys.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xylfe.cn/gtpdvxgjzl.html

Py:   if not data: return
来源：http://hz.daxiang520.top/gtnxjxcrtb.html

PHP:  if (!$data) { return; }
来源：http://hz.yj20258.top/gtghkawvdz.html

JS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtkdmnddgc.html

TS:   if (!data) return;
来源：http://hz.hnxiangtu.top/gtaraytvyj.html

Java: if (data == null) return;
来源：http://hz.guannengcc.top/gtyctiswiq.html

Go:   if data == nil { return }
来源：http://hz.hfpthk.cn/gtovvcdcnu.html

Ruby: return if data.nil?
来源：http://hz.cdnleiting.top/gtlesgmbxc.html

C#:   if (data == null) return;
来源：http://hz.gaohongyu789.top/gtfksrczcy.html

================================================================================
来源：http://hz.sxryk.cn/gtrkomczzv.html

C. 函数与作用域
来源：http://hz.haohaochexian.top/gtuzaxeqvs.html

================================================================================
来源：http://hz.yueranfly.top/gthtdmapew.html

[C01] 定义函数
来源：http://hz.yonumen.top/gtlmxrcvue.html

Py:   def add(a, b): return a + b
来源：http://hz.andypj.xyz/gtiettdojc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtrwyflwlm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gthsbflonk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtqjxiiorh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtqxkcghem.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhoulong.xyz/gtmkvtjzqd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zycfv.cn/gtxywwlyae.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtnwzwtmsx.html

[C02] 默认参数
来源：http://hz.sysykeji.top/gtloyjybam.html

Py:   def greet(name="World"): return name
来源：http://hz.zdqjudy.top/gtoehujyey.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenlongwang.top/gtqosqfdiq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.316326.xyz/gtdnttlfmz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daxiang520.top/gtwflwuetu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigufen.top/gtwgjzivrx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xuetiantiany.cn/gtcmqskegs.html

Ruby: def greet(name = "World") = name
来源：http://hz.yueranfly.top/gtbmqbnaus.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guannengcc.top/gtdisqxcmp.html

[C03] 可变参数
来源：http://hz.hfpthk.cn/gtuzlehyzs.html

Py:   def total(*args): return sum(args)
来源：http://hz.gotoacloud.top/gtesnqqzzy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ywan-chungtsiang.top/gtdcohdxvx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtttebucdj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gaohongyu789.top/gtfcnhdktm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.smart0.xyz/gttwskzmjv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.svipenyu.cn/gtcqkerihw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtvmsicgde.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.52xcode.cn/gtirboidre.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinqigfzy.top/gtwttdsaek.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.c1oappe.top/gtrocipsid.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yueranfly.top/gtxbdegdru.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtkxlqpjer.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shuidangran.top/gtsjsasvte.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.iojbl.cn/gtrqqjfpex.html

Go:   // 无：用配置结构体参数
来源：http://hz.hysaishi.cn/gttfmqbxmz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtwiyuhwyq.html

C#:   f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtluiqabhp.html

[C05] 返回多个值
来源：http://hz.xziqi.cn/gtgiygulfi.html

Py:   return a, b
来源：http://hz.quarkkingdee.top/gtjzeuykpf.html

PHP:  return [$a, $b];
来源：http://hz.yuxming.cn/gteqxovfcv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.feifeiyinyue.top/gtxytqhhib.html

TS:   return { a, b };
来源：http://hz.fzhhl.top/gtyajwetsn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tanke756.top/gtriggehnr.html

Go:   return a, b
来源：http://hz.316326.xyz/gtrhwnhgja.html

Ruby: return a, b
来源：http://hz.aibaodan.cn/gtoltsxdwh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nanxinkj.top/gtdflatulx.html

[C06] 匿名函数 / lambda
来源：http://hz.0kj1m.cn/gtnhjqdydu.html

Py:   square = lambda x: x * x
来源：http://hz.zdqjudy.top/gtejwbrves.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ppjwa.cn/gtdopdeqwg.html

JS:   const square = x => x * x;
来源：http://hz.gotoacloud.top/gtewbbfijz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sweek.top/gtchqlxhgi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigufen.top/gttirclggt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ehwqpu.com/gtguacuhny.html

Ruby: square = ->(x) { x * x }
来源：http://hz.birdmap.top/gtylwvrwdq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gzhubu.top/gtgypobwvg.html

[C07] 把函数作为参数传入
来源：http://hz.sufxvd.cn/gtptwmnizk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cucudq.cn/gtcvovmuba.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinyuanbaomall.cn/gtxmbiplrk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhengqikj.top/gtmuvkjocu.html

TS:   arr.map(String)
来源：http://hz.gaohongyu789.top/gtjveulpov.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sweek.top/gtykjqlpye.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhongyouzk.top/gtqejamuev.html

Ruby: arr.map(&:upcase)
来源：http://hz.haohaochexian.top/gtrzmcwggg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zdqjudy.top/gtoxhbsjam.html

[C08] 闭包
来源：http://hz.shzxlz.cn/gtkzgndcbk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj20258.top/gtmkaqkxrf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dashuyun.cn/gtamwicgze.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtemaqnzho.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtdiskloqk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.mhx1999.top/gtnnfbypos.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zycfv.cn/gtudxmtiyr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guowangkeji.top/gtestietne.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtzgrldwxt.html

[C09] 递归
来源：http://hz.nwbrower.top/gtqftgtjjv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtzovoupnt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yonumen.top/gtijiqnanr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtougedsup.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tanke756.top/gtvllsjhal.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gogol.net.cn/gtgbpdslqr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.quarkkingdee.top/gtbryblzvj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.vqdsnc.cn/gtvjkwdpce.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtylggvlrj.html

[C10] 变量作用域
来源：http://hz.ehwqpu.com/gttdikrehs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yvedp.cn/gtlhmdncbu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yanxiufei.cn/gtjmcgcuwu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhiwuduotai.top/gtchfvufpn.html

TS:   同 JS
来源：http://hz.jqgufenzy.top/gtsvsqkgwp.html

Java: 方法内为块级作用域
来源：http://hz.cashguo.top/gttdhjkjdd.html

Go:   花括号块级作用域
来源：http://hz.cqqwz.cn/gttmfkkuiy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sufxvd.cn/gtqwdgfjxc.html

C#:   块级作用域
来源：http://hz.wangdashe.top/gtbtocklva.html

[C11] 模块导入与导出
来源：http://hz.shanyushiyangkeji.top/gtmwltrojt.html

Py:   from module import func
来源：http://hz.gogol.net.cn/gtjioelmrk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ybcxt.top/gtoupihkqi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtehygcpnw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.aibaodan.cn/gtdoemwmjs.html

Java: import java.util.List;
来源：http://hz.aizwys.cn/gtnzulvlot.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jqgufenzy.top/gtnukmlvrz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.feifeiyinyue.top/gtsbkzdfae.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtbhgfhcke.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnqzz.top/gtroifkwjo.html

Py:   (lambda: print("run"))()
来源：http://hz.zycfv.cn/gttpkmccwq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hywenlv.cn/gtpuhqepiw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sweek.top/gtdvomuakx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtatyohjkf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jyoumei.cn/gttercrgjl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gtoqglynzn.html

Ruby: -> { puts "run" }.call
来源：http://hz.jiagoushi.top/gtvrzfgity.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.wangdashe.top/gtfecvcwtt.html

[C13] 类型声明 / 类型注解
来源：http://hz.shuidangran.top/gthhrhusbf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenjidiqi.icu/gtfvdubfmd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtjhyrbddz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cucudq.cn/gtessypycw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtxsjsyweu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtsfculxyw.html

Go:   func add(a, b int) int
来源：http://hz.bjfxy.top/gtrfbkhrli.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtelclvlsu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hfpthk.cn/gtvvbnahzi.html

[C14] 泛型函数
来源：http://hz.aibaodan.cn/gtnwvxjqgw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aibaodan.cn/gtovgnbghv.html

PHP:  // 无泛型
来源：http://hz.chenlongwang.top/gtpkquztng.html

JS:   // 无泛型
来源：http://hz.tanke756.top/gtehopuxxi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jiagoushi.top/gtmvqqjexa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.snrcjt.cn/gtydaonnac.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.vqdsnc.cn/gtgshfabze.html

Ruby: # 无泛型
来源：http://hz.316326.xyz/gtxmiqnngj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtgukqwyji.html

[C15] 解构 / 展开参数
来源：http://hz.dashuyun.cn/gtblszzwxy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pengpengdd.cyou/gtysdcikoa.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258.top/gttiihjhii.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtknzuqqtr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hfpthk.cn/gtrtqgrluo.html

Java: // 无解构
来源：http://hz.zhongyouzk.top/gtsjaqtjmj.html

Go:   // 无解构
来源：http://hz.zhoulong.xyz/gtjkgkeejc.html

Ruby: a, b = pair
来源：http://hz.cashguo.top/gthwjhdmgb.html

C#:   var (a, b) = pair;
来源：http://hz.zhiwuduotai.top/gtjxybbilr.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtxzhrwtor.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.vqdsnc.cn/gtzwamzvmw.html

PHP:  // 无重载
来源：http://hz.nwbrower.top/gtvvotilfa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sufxvd.cn/gttdlulams.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.quarkkingdee.top/gtnncydgxm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nwbrower.top/gtsrjuleon.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258888.top/gtrsuiwoxf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtkmnxmyfd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nanxuanxn.top/gtkfvaigag.html

================================================================================
来源：http://hz.ivvv.top/gthabglkif.html

D. 数组 / 列表 / 集合
来源：http://hz.hfpthk.cn/gtjeakoscw.html

================================================================================
来源：http://hz.guowangkeji.top/gtoymvtryj.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtwdpwruyr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sxryk.cn/gtgfgwcbvm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jianghu66.top/gtyvgnuxra.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gzhubu.top/gttwutljsb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sysykeji.top/gtywblzzgh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj202588.top/gtlojnoagy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinghuilouyu.cn/gtlcvlwjww.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258888.top/gtonuauwfi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gtjcpylfpr.html

[D02] 追加元素到末尾
来源：http://hz.jqgfzy.top/gtwxmiyrnl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtebvmxnbx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cucudq.cn/gtndbmuwld.html

JS:   arr.push(4);
来源：http://hz.meibo888.top/gtjqesfjux.html

TS:   arr.push(4);
来源：http://hz.xylfe.cn/gtngltiavt.html

Java: list.add(4);
来源：http://hz.yanxiufei.cn/gtowixzhcl.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258.top/gtvdpdfkho.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yanxiufei.cn/gtwukncaug.html

C#:   list.Add(4);
来源：http://hz.316326.xyz/gtvmuvegne.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtmveeqrqr.html

Py:   arr.insert(0, 0)
来源：http://hz.ywan-chungtsiang.top/gteuwwybnu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gtpfcejinh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigufen.top/gtsgeikkzw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangdashe.top/gtmqtyylyl.html

Java: list.add(0, 0);
来源：http://hz.zhongyouzk.top/gtdeqoaokp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jqgfzy.top/gtomtebwiw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tanke756.top/gtlkrnjbib.html

C#:   list.Insert(0, 0);
来源：http://hz.tian-w.cn/gtdamyvfrm.html

[D04] 删除元素
来源：http://hz.daria6918.cn/gtdiuezwze.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yongpay.top/gtbidieyza.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhaomingkeji.xyz/gtbjviissy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zycfv.cn/gtmzxvjriy.html

TS:   arr.splice(0, 1);
来源：http://hz.cashguo.top/gtmvcgacjq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sxryk.cn/gtxnajgcfh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sweek.top/gtgfumyoqc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtufdwclxs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ybcxt.top/gtcwnquiej.html

[D05] 访问与修改元素
来源：http://hz.jinqigfzy.top/gtslhwchnk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.bjfxy.top/gtwnneurou.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jlsjyb.cn/gtqoasknua.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jqgfzy.top/gtjlvxnzgq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sxryk.cn/gtkrwvacya.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtlpuwnfem.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gtcwpbuotd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtkfgtrsdy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhongyouzk.top/gttiggmgbn.html

[D06] 数组长度
来源：http://hz.quarkkingdee.top/gtyeixhhvu.html

Py:   len(arr)
来源：http://hz.nwbrower.top/gtketvnqqr.html

PHP:  count($arr);
来源：http://hz.ydjk.org.cn/gtbjfjrhle.html

JS:   arr.length
来源：http://hz.hnxiangtu.top/gthinohwxp.html

TS:   arr.length
来源：http://hz.mhx1999.top/gtnatwxqng.html

Java: list.size();
来源：http://hz.gogol.net.cn/gtmlhbkquy.html

Go:   len(arr)
来源：http://hz.bjfxy.top/gtxpeyoyqm.html

Ruby: arr.length; arr.size
来源：http://hz.nanxuanxn.top/gtqagfhxbx.html

C#:   list.Count;
来源：http://hz.aizwys.cn/gttgqztreo.html

[D07] 切片 / 取子数组
来源：http://hz.wangdashe.top/gtlqlkuvnx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.fengsongda.top/gtmuoxduqw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fzhhl.top/gtmrenkcsc.html

JS:   arr.slice(1, 4);
来源：http://hz.hammf.cn/gtrzcsbaln.html

TS:   arr.slice(1, 4);
来源：http://hz.bjfxy.top/gtazxsqply.html

Java: list.subList(1, 4);
来源：http://hz.cashguo.top/gtoutpzzng.html

Go:   arr[1:4]
来源：http://hz.yanxiufei.cn/gtfngiifez.html

Ruby: arr[1, 3]
来源：http://hz.cheryme.top/gtpcgbiolm.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangshuangyany.cn/gtjhjjksoc.html

[D08] 合并两个数组
来源：http://hz.xziqi.cn/gtkpebkpzo.html

Py:   a + b;  a.extend(b)
来源：http://hz.havefunace.top/gtyfhhpdoe.html

PHP:  array_merge($a, $b);
来源：http://hz.cheryme.top/gtagixwakw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ywan-chungtsiang.top/gtnwykrruy.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gtdxyfwlep.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhongyouzk.top/gtmioqvfuj.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gttkecoiyj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tianlin.xyz/gtxgstjczp.html

C#:   a.Concat(b).ToList()
来源：http://hz.xinyue.icu/gtovzlzbfv.html

[D09] 排序（升序）
来源：http://hz.smart0.xyz/gtndjbsicv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtupqvyxkq.html

PHP:  sort($arr);
来源：http://hz.jyoumei.cn/gtbthmdnim.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fengsongda.top/gtspgauyyo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigfzy.top/gtxsoecjar.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenjidiqi.icu/gtovwudbiw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.iojbl.cn/gtuocobdel.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtixjcxegt.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gtmatbrhoj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.c1oappe.top/gtvcxjxahv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shanyushiyangkeji.top/gtuosmmdkk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cashguo.top/gtmgbfjesv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shangyingyoupin.top/gtrlgkiwvl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtsompnlfe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ehwqpu.com/gtjwildhwq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shuidangran.top/gtdcvpovdg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daria6918.cn/gtrvticzgg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tanke756.top/gttwzuhzoo.html

[D11] 反转数组
来源：http://hz.cucudq.cn/gtmgkicted.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.haohaochexian.top/gtbxjxqxvv.html

PHP:  array_reverse($arr);
来源：http://hz.ivvv.top/gtbfslgjsf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.wangdashe.top/gtgugqnoxc.html

TS:   [...arr].reverse();
来源：http://hz.chenlongwang.top/gtljddwtmy.html

Java: Collections.reverse(list);
来源：http://hz.quarkkingdee.top/gtkdqipvwe.html

Go:   slices.Reverse(arr)
来源：http://hz.tianlin.xyz/gtosurdwtd.html

Ruby: arr.reverse
来源：http://hz.nwbrower.top/gtkhgztbsd.html

C#:   list.Reverse();
来源：http://hz.sufxvd.cn/gtajcsryok.html

[D12] 查找元素下标
来源：http://hz.daria6918.cn/gtpaokwjpx.html

Py:   arr.index(x);  x in arr
来源：http://hz.cqqwz.cn/gtnnbhmism.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenjidiqi.icu/gtmcuoadwa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtgkhmamwq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gotoacloud.top/gtrzzpkgjq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tian-w.cn/gthibmzzxf.html

Go:   slices.Index(arr, x)
来源：http://hz.cheryme.top/gtwfpztutt.html

Ruby: arr.index(x)
来源：http://hz.chenzaomai.com/gtjzoslwjw.html

C#:   list.IndexOf(x);
来源：http://hz.yj202588.top/gtvwdddpfa.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xuanzx.com/gtxowdxevf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yanxiufei.cn/gtbuievhxe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.316326.xyz/gtmpvddgoq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuanzhike.top/gteidntexa.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ydjk.org.cn/gtkrphztdq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yvedp.cn/gtzryfwwfr.html


<!-- 参考信息 -->