代发 wailian999

================================================================================
来源：http://hz.shuidangran.top/gtfsjeyede.html

C. 函数与作用域
来源：http://hz.tianlin.xyz/gtwrgiiuqv.html

================================================================================
来源：http://hz.hammf.cn/gtpvsdrgvp.html

[C01] 定义函数
来源：http://hz.zycfv.cn/gtxngcqusg.html

Py:   def add(a, b): return a + b
来源：http://hz.shzxlz.cn/gtuyyaastc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gttidasxmv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gogol.net.cn/gtdakrbyqn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gtwneugzwx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtomxtpact.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.bjfxy.top/gthbwmqceg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sufxvd.cn/gtttvzkymh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yongpay.top/gtwkqnsdef.html

[C02] 默认参数
来源：http://hz.jiagoushi.top/gtpyythfua.html

Py:   def greet(name="World"): return name
来源：http://hz.jinyuanbaomall.cn/gtkzhtxxae.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ppjwa.cn/gtdvlcqwdx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gtduxzhdpi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tian-w.cn/gtqvpkdyai.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.guowangkeji.top/gtfdfexqyz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.vqdsnc.cn/gtgaeanzpr.html

Ruby: def greet(name = "World") = name
来源：http://hz.fzhhl.top/gtmrqgqmqw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj202588.top/gtkzmtzvfw.html

[C03] 可变参数
来源：http://hz.cqqwz.cn/gtymvemmlg.html

Py:   def total(*args): return sum(args)
来源：http://hz.tianlin.xyz/gtbaqlignj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pengpengdd.cyou/gthzsbfzan.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shangyingyoupin.top/gtzbczpgzf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gtgtqufzkg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gteaywshkg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenlongwang.top/gtyepdymbe.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.9152youxi.cn/gtlmwjuhuv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yanxiufei.cn/gtaqymyilh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aibaodan.cn/gtwmegofvt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnqzz.top/gtpteadhpj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhaomingkeji.xyz/gtjdujffqj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtxmbwcmjy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.dashuyun.cn/gttuyijjss.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenjidiqi.icu/gtfrpzmfoi.html

Go:   // 无：用配置结构体参数
来源：http://hz.vqdsnc.cn/gtenqyzuwk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtjdljckju.html

C#:   f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtppejakdg.html

[C05] 返回多个值
来源：http://hz.ywan-chungtsiang.top/gtmvcomdsk.html

Py:   return a, b
来源：http://hz.yanxiufei.cn/gteunziwbb.html

PHP:  return [$a, $b];
来源：http://hz.bjfxy.top/gtrjxoichp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cdnleiting.top/gtbvvibilr.html

TS:   return { a, b };
来源：http://hz.jinghuilouyu.cn/gtavzfweaq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cqqwz.cn/gtwgviqlhk.html

Go:   return a, b
来源：http://hz.hnqzz.top/gtywnlosto.html

Ruby: return a, b
来源：http://hz.cashguo.top/gtknhkzonk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dashuyun.cn/gtbbrpuqbr.html

[C06] 匿名函数 / lambda
来源：http://hz.zhiwuduotai.top/gtwxhypsrz.html

Py:   square = lambda x: x * x
来源：http://hz.ydjk.org.cn/gtsbxtwvnx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuetiantiany.cn/gtmuurklwf.html

JS:   const square = x => x * x;
来源：http://hz.jqgfzy.top/gtidponcef.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yangfankeji.com/gtnhekvqfz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gogol.net.cn/gtobolrlph.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yongpay.top/gttvrtynhv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.quarkkingdee.top/gtbllujtvb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydjk.org.cn/gtqcoqjwba.html

[C07] 把函数作为参数传入
来源：http://hz.xinyue.icu/gtuygdghjy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.svipenyu.cn/gtgvlssamj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xingfuxueyuan.xyz/gtlwrrbxlp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cashguo.top/gttpixdfhv.html

TS:   arr.map(String)
来源：http://hz.52xcode.cn/gtpkobgcxb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhongyouzk.top/gtzrvtiexr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yangfankeji.com/gtmfzhejqh.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258888.top/gtaerfhfay.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hfpthk.cn/gtnbpuxfyt.html

[C08] 闭包
来源：http://hz.cashguo.top/gtabillmzg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigufen.top/gtmpgvfvsm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cdnleiting.top/gtmlumjlsf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtchyqwdtb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtnwcydvms.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cqqwz.cn/gthvwlvlwt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tianlin.xyz/gtzamdymoh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jyoumei.cn/gtahqnrsxe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtkjhtjnml.html

[C09] 递归
来源：http://hz.ehwqpu.com/gtsluyznmx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtxcturwsx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shzxlz.cn/gtffcaevkq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtigzejvwd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pengpengdd.cyou/gtoecywnps.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jiagoushi.top/gtoxbmatzv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cqqwz.cn/gtgqkxrcrj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gotoacloud.top/gthmanxwhw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.0kj1m.cn/gtwizutetk.html

[C10] 变量作用域
来源：http://hz.sufxvd.cn/gtchavgoma.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuanzhike.top/gtwdxqnbbx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gotoacloud.top/gtyuyprfmj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gogol.net.cn/gtmjexvycm.html

TS:   同 JS
来源：http://hz.bjfxy.top/gtytowdelv.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtlbvoaryx.html

Go:   花括号块级作用域
来源：http://hz.zhiwuduotai.top/gtkeqmpxke.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.feifeiyinyue.top/gtfmyicoop.html

C#:   块级作用域
来源：http://hz.jinqigufen.top/gtgnzdmrye.html

[C11] 模块导入与导出
来源：http://hz.zhongyouzk.top/gtjawqqanx.html

Py:   from module import func
来源：http://hz.meibo888.top/gtbuelsopv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cucudq.cn/gtqgacadir.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.daria6918.cn/gtbgggyzmt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tanke756.top/gtkwmldozy.html

Java: import java.util.List;
来源：http://hz.hnxiangtu.top/gtrewolhoh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gttlxyulqm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydzc1.top/gtbrkkbtlk.html

C#:   using System.Text;
来源：http://hz.jiagoushi.top/gtkbvhclmz.html

[C12] 立即执行函数 IIFE
来源：http://hz.meibo888.top/gtnrepimwu.html

Py:   (lambda: print("run"))()
来源：http://hz.xuanzx.com/gtcnmrizlk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yvedp.cn/gtnjrnfmsb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gttwjgrhvz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yvedp.cn/gtpwgsulzb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.316326.xyz/gtsggqdadn.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jqgfzy.top/gtvfxfrrdz.html

Ruby: -> { puts "run" }.call
来源：http://hz.kuanghao11.cn/gtmkxwwwwo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuxming.cn/gtbvexmrys.html

[C13] 类型声明 / 类型注解
来源：http://hz.hongshengwenyu.top/gtbhotujba.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuetiantiany.cn/gtqejqcixc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aizwys.cn/gtegmqdrao.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sweek.top/gtbqbtwghb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtzjmhxjpt.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtenkwddqx.html

Go:   func add(a, b int) int
来源：http://hz.hfpthk.cn/gttyxtdyyr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhixingplan.top/gtyzukybuz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dashuyun.cn/gtgfdbketf.html

[C14] 泛型函数
来源：http://hz.quarkkingdee.top/gtttlkggmm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ehwqpu.com/gtiqtrvcon.html

PHP:  // 无泛型
来源：http://hz.52xcode.cn/gtjsdadguz.html

JS:   // 无泛型
来源：http://hz.nwbrower.top/gtsrjhxqzk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hysaishi.cn/gtmdvpquji.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.snrcjt.cn/gtkhpcadvb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xinyue.icu/gtljdigbww.html

Ruby: # 无泛型
来源：http://hz.ybcxt.top/gtxwhpvzkc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gteruabtdl.html

[C15] 解构 / 展开参数
来源：http://hz.ydzc1.top/gtcooddkoo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.smart0.xyz/gtnmnrtbgi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhaomingkeji.xyz/gtydkwqhaz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cheryme.top/gtjivkfpud.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fengsongda.top/gtqvwqwdjf.html

Java: // 无解构
来源：http://hz.jqgufenzy.top/gtpomzctju.html

Go:   // 无解构
来源：http://hz.xziqi.cn/gtvgycaych.html

Ruby: a, b = pair
来源：http://hz.aibaodan.cn/gtnratbmul.html

C#:   var (a, b) = pair;
来源：http://hz.sweek.top/gtoccvnfhd.html

[C16] 函数 / 方法重载
来源：http://hz.snrcjt.cn/gtkbarfohd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xuanzx.com/gtzaibccct.html

PHP:  // 无重载
来源：http://hz.nwbrower.top/gtlkopanny.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenjidiqi.icu/gttagjgqjs.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenzaomai.com/gtqqsrxxdl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nwbrower.top/gtkrizqtpj.html

Go:   // 无重载：用不同函数名
来源：http://hz.gogol.net.cn/gtgexqbxrx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pycfn.com/gtadtqmlnv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guowangkeji.top/gtzmkdqruz.html

================================================================================
来源：http://hz.nanxinkj.top/gtfhdcpjsq.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gtyxrolqgq.html

================================================================================
来源：http://hz.ydzc1.top/gttclvrqif.html

[D01] 创建数组 / 列表
来源：http://hz.aibaodan.cn/gtxpgbdlmz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtjnaoykzy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sweek.top/gtvnfiyfxy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.feifeiyinyue.top/gteutlqtmf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pycfn.com/gtheuzruyb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhengqikj.top/gtopxnabcp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.wangshuangyany.cn/gtbxvvdkho.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinqigufen.top/gtzozbeayp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtkhfxbspp.html

[D02] 追加元素到末尾
来源：http://hz.zhaomingkeji.xyz/gtuvlarifm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangdashe.top/gtcppdcsap.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinghuilouyu.cn/gtymbuxmlj.html

JS:   arr.push(4);
来源：http://hz.c1oappe.top/gtwvtkddyd.html

TS:   arr.push(4);
来源：http://hz.yj20258888.top/gtrtzexqql.html

Java: list.add(4);
来源：http://hz.shanyushiyangkeji.top/gtnzzhtuoe.html

Go:   arr = append(arr, 4)
来源：http://hz.redwolf501.top/gtalxwqday.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yueranfly.top/gtklqwgged.html

C#:   list.Add(4);
来源：http://hz.yueranfly.top/gtdndigukf.html

[D03] 在指定位置插入元素
来源：http://hz.sweek.top/gtkkvdqlbj.html

Py:   arr.insert(0, 0)
来源：http://hz.snrcjt.cn/gtxlsuewky.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnxiangtu.top/gtnfqnpeaj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxinkj.top/gtuolrkhrz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yuanzhike.top/gtgfamycds.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gtuxyugior.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.andypj.xyz/gtzdegkutn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydjk.org.cn/gtyclvoatj.html

C#:   list.Insert(0, 0);
来源：http://hz.yj202588.top/gtixrccvbg.html

[D04] 删除元素
来源：http://hz.ybcxt.top/gtshcrlnxm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenjidiqi.icu/gtyaunpkme.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pycfn.com/gtlkgzpptb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxinkj.top/gtzucrryzf.html

TS:   arr.splice(0, 1);
来源：http://hz.tianlin.xyz/gtmlmxuwpt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fengsongda.top/gtrwadqgiu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gtrwasthrj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shzxlz.cn/gteusuvsxs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.bjfxy.top/gtwqsqqema.html

[D05] 访问与修改元素
来源：http://hz.xuetiantiany.cn/gtovcqsyxo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtdnsmuymb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xinyue.icu/gtnggmqcly.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aibaodan.cn/gthofehigk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigufen.top/gtwauvbyhn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhiwuduotai.top/gtybwgfaxa.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtohnrxsnq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtozgpbbdz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.smart0.xyz/gtorhddwiv.html

[D06] 数组长度
来源：http://hz.9152youxi.cn/gtfiarqtke.html

Py:   len(arr)
来源：http://hz.hnqzz.top/gtfxzjznka.html

PHP:  count($arr);
来源：http://hz.zhaomingkeji.xyz/gtnodxastt.html

JS:   arr.length
来源：http://hz.tanke756.top/gtgxbfbuwi.html

TS:   arr.length
来源：http://hz.ehwqpu.com/gtsjtdxcgc.html

Java: list.size();
来源：http://hz.yongpay.top/gtpfdphvlt.html

Go:   len(arr)
来源：http://hz.cheryme.top/gtmcijswha.html

Ruby: arr.length; arr.size
来源：http://hz.zhiwuduotai.top/gttpjlqllu.html

C#:   list.Count;
来源：http://hz.sxryk.cn/gtydmgosqb.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gtggvgtogj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zdqjudy.top/gtkthsshrx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenzaomai.com/gtmmgkdjfr.html

JS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtritslkfn.html

TS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gthgejlqad.html

Java: list.subList(1, 4);
来源：http://hz.zhongyouzk.top/gtmssdkdcv.html

Go:   arr[1:4]
来源：http://hz.jiagoushi.top/gtypomlnkl.html

Ruby: arr[1, 3]
来源：http://hz.feifeiyinyue.top/gtqyolyucw.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgufenzy.top/gtvksxveyc.html

[D08] 合并两个数组
来源：http://hz.ydzc1.top/gtbmjggbaq.html

Py:   a + b;  a.extend(b)
来源：http://hz.cheryme.top/gtlbzomwhp.html

PHP:  array_merge($a, $b);
来源：http://hz.haohaochexian.top/gtnilpxsje.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yvedp.cn/gtonlonhti.html

TS:   [...a, ...b];
来源：http://hz.nwbrower.top/gtnvoxydqg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jqgfzy.top/gtdtfabisb.html

Go:   append(a, b...)
来源：http://hz.andypj.xyz/gtyemiooes.html

Ruby: a + b;  a.concat(b)
来源：http://hz.andypj.xyz/gtoakaufkx.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gtlxjddnon.html

[D09] 排序（升序）
来源：http://hz.iojbl.cn/gteytzbxtj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtotsrsvkd.html

PHP:  sort($arr);
来源：http://hz.zhixingplan.top/gtiskgvapv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ywan-chungtsiang.top/gtmquikgyf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenlongwang.top/gtdjjbllbw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gtqhtkrkvx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtvmhorxol.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gtcldaipvy.html

C#:   list.Sort();
来源：http://hz.ivvv.top/gthowwnyee.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xziqi.cn/gtkkcsmagw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sysykeji.top/gttqmpkhwn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hywenlv.cn/gtnileyvwg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtygbwalpn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtcanzxwmk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangtech.top/gttkioqajf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinyuanbaomall.cn/gtiztibpbb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhengqikj.top/gtccvcqyln.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.aibaodan.cn/gtvpbuwojb.html

[D11] 反转数组
来源：http://hz.nanxinkj.top/gtyzhmnnkk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jianghu66.top/gtwqfprpnd.html

PHP:  array_reverse($arr);
来源：http://hz.shanyushiyangkeji.top/gtopdyexdz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtblcgvrkp.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gtwsaiejdx.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtekysogih.html

Go:   slices.Reverse(arr)
来源：http://hz.sysykeji.top/gtnbmvilhv.html

Ruby: arr.reverse
来源：http://hz.daxiang520.top/gtikyjgwyf.html

C#:   list.Reverse();
来源：http://hz.c1oappe.top/gtpzddfmsk.html

[D12] 查找元素下标
来源：http://hz.pycfn.com/gtsoajwmcr.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgfzy.top/gtewpllpyw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gaohongyu789.top/gtnynkdmcj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gtsmjwglzq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtcnjswwvk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.feifeiyinyue.top/gtuoaaagbx.html

Go:   slices.Index(arr, x)
来源：http://hz.fengsongda.top/gtcqhugppp.html

Ruby: arr.index(x)
来源：http://hz.yuxming.cn/gtumadywhy.html

C#:   list.IndexOf(x);
来源：http://hz.yuxming.cn/gtpjzdrqxq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtdmbjomjd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.aizwys.cn/gtszubgzbv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fzhhl.top/gtucdvxpdu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtlfioipdv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtjnoiafkx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.316326.xyz/gtbkbmbbha.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pengpengdd.cyou/gtytpujrne.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ehwqpu.com/gtvysrxhox.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dashuyun.cn/gthjpveiud.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuxming.cn/gthoutruuv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.svipenyu.cn/gtszhsazmp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cheryme.top/gtfhlavsji.html

JS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gtijbjjqaj.html

TS:   arr.map(x => x * 2)
来源：http://hz.cqqwz.cn/gtdpoituvv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hongshengwenyu.top/gtumrgxnup.html

Go:   // 手写循环
来源：http://hz.shangyingyoupin.top/gtggouodup.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ehwqpu.com/gtyfrmovou.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xylfe.cn/gtvxgrkbrk.html

[D15] 去重
来源：http://hz.aizwys.cn/gtvokhvnts.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gtwjdgpane.html

PHP:  array_unique($arr);
来源：http://hz.yuxming.cn/gtmkrdgeet.html

JS:   [...new Set(arr)]
来源：http://hz.guannengcc.top/gtydsafvgg.html

TS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtpdrgydlw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hysaishi.cn/gtruosxjdb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jqgufenzy.top/gtlpumivgb.html

Ruby: arr.uniq
来源：http://hz.chenlongwang.top/gtaczeyzcj.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgfzy.top/gtqjumsjla.html

[D16] 求和与平均值
来源：http://hz.jiagoushi.top/gtohajjlsd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xziqi.cn/gtqnofbysf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.daria6918.cn/gtudzxkiwn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtflnuvgoe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jyoumei.cn/gttuldujhn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.bjfxy.top/gtolgsbxvu.html

Go:   // 手写循环累加
来源：http://hz.yongpay.top/gtqnzpgrjl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gzhubu.top/gtynhxajdd.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenzaomai.com/gtcbqlxxsd.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gtdcaveeyh.html

Py:   max(arr);  min(arr)
来源：http://hz.nwbrower.top/gtxmdimtty.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydzc1.top/gtmiiofpza.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jiagoushi.top/gtsuqunetg.html

TS:   Math.max(...arr);
来源：http://hz.shangyingyoupin.top/gtytnallsd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yonumen.top/gtrjsbosqy.html


<!-- 参考信息 -->