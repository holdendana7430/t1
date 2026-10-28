代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hz.zycfv.cn/gtgaebifhl.html

[C03] 可变参数
来源：http://hz.zhongyouzk.top/gtbnimdxng.html

Py:   def total(*args): return sum(args)
来源：http://hz.hnqzz.top/gtlbvidjnz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xuanzx.com/gtijdlujrw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtljlkowlr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hongshengwenyu.top/gtfjpbgcxb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gtztvhfwib.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ppjwa.cn/gtxbrlyubr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gogol.net.cn/gtezdzyxru.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.feifeiyinyue.top/gtrseuvodp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hammf.cn/gtacxxrjib.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xingfuxueyuan.xyz/gtqktzexsk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shanyushiyangtech.top/gtklchrjuo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtychcnizh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cashguo.top/gtemmobwpx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.birdmap.top/gtrsigcbqn.html

Go:   // 无：用配置结构体参数
来源：http://hz.fengsongda.top/gtprebypfz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.andypj.xyz/gtxwfminjc.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtznqpwffw.html

[C05] 返回多个值
来源：http://hz.snrcjt.cn/gtqzsekhtx.html

Py:   return a, b
来源：http://hz.fzhhl.top/gtjxiextjv.html

PHP:  return [$a, $b];
来源：http://hz.hysaishi.cn/gtavlizplu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.birdmap.top/gtwxjqwsgo.html

TS:   return { a, b };
来源：http://hz.sweek.top/gtihtczwiz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.redwolf501.top/gtcspkgyfa.html

Go:   return a, b
来源：http://hz.cucudq.cn/gtkykqxwcc.html

Ruby: return a, b
来源：http://hz.hammf.cn/gterisqdkl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hfpthk.cn/gtbpsddpju.html

[C06] 匿名函数 / lambda
来源：http://hz.ppjwa.cn/gtkqhcpssu.html

Py:   square = lambda x: x * x
来源：http://hz.shuidangran.top/gtggpzxlal.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jqgufenzy.top/gtyrbcvqqo.html

JS:   const square = x => x * x;
来源：http://hz.sxryk.cn/gtwfahhewf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgfzy.top/gtsdiogykc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhixingplan.top/gtgrtakihe.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhixingplan.top/gtualvotzu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gttqiwenny.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sufxvd.cn/gtewghhaoi.html

[C07] 把函数作为参数传入
来源：http://hz.zhaomingkeji.xyz/gtgrhsbzly.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.bjfxy.top/gtmcylqsfl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tianlin.xyz/gttapwckkc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.pengpengdd.cyou/gtzcrkxwib.html

TS:   arr.map(String)
来源：http://hz.ybcxt.top/gtdfgkjoce.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhoulong.xyz/gtudpjlqye.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhaomingkeji.xyz/gtupsukmkd.html

Ruby: arr.map(&:upcase)
来源：http://hz.vqdsnc.cn/gtdjqlxkvn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shangyingyoupin.top/gtmprsewba.html

[C08] 闭包
来源：http://hz.iojbl.cn/gtscoaddrf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ehwqpu.com/gtemsbspyw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuetiantiany.cn/gtchfypycn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gtqcczcbrq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gttwvhqfyl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.smart0.xyz/gthxxsemnp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.aizwys.cn/gtlmgmjjgb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangdashe.top/gtsrxvxjfq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtwgcclueh.html

[C09] 递归
来源：http://hz.ivvv.top/gticsqtemn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.svipenyu.cn/gtxfhehmpn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ppjwa.cn/gtbinoikff.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtqjxlefbv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtkhzittdn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.52xcode.cn/gtcuhbeghu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tianlin.xyz/gtyjrirtjs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.redwolf501.top/gtwuiuwqik.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenjidiqi.icu/gtnewnuudu.html

[C10] 变量作用域
来源：http://hz.jinyuanbaomall.cn/gtpxxdsvte.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.bjfxy.top/gtrsldcpjx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhixingplan.top/gtldljgeto.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtthlouuve.html

TS:   同 JS
来源：http://hz.chenlongwang.top/gtjjqwyrke.html

Java: 方法内为块级作用域
来源：http://hz.pengpengdd.cyou/gthxnpxutn.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangkeji.top/gtenkfwfek.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yanxiufei.cn/gtlyhzzvmd.html

C#:   块级作用域
来源：http://hz.iojbl.cn/gtphdhjofd.html

[C11] 模块导入与导出
来源：http://hz.zycfv.cn/gtbdygemyu.html

Py:   from module import func
来源：http://hz.meibo888.top/gtpdbrcgqm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xinyue.icu/gtlheedlbr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yj20258.top/gtygjaqjzz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuxming.cn/gtrflxwprz.html

Java: import java.util.List;
来源：http://hz.xingfuxueyuan.xyz/gtgmjusphe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.pycfn.com/gtlgzclwsr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhaomingkeji.xyz/gthmxxlrxb.html

C#:   using System.Text;
来源：http://hz.smart0.xyz/gtbkssgmao.html

[C12] 立即执行函数 IIFE
来源：http://hz.jyoumei.cn/gtdkzoxutx.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtasofdwvn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.fzhhl.top/gtturhobqg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtllkmgvig.html

TS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtzefdeamt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hfpthk.cn/gttfakfvxl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.bjfxy.top/gtaleqokha.html

Ruby: -> { puts "run" }.call
来源：http://hz.sufxvd.cn/gtsearnaso.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gthfiwbgvh.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhijiandao.cn/gtvnlspcvu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xingfuxueyuan.xyz/gtwsjjdnjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtjkxflmog.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuanzhike.top/gtipicfmry.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sysykeji.top/gtqjrbdjqw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtznniilyk.html

Go:   func add(a, b int) int
来源：http://hz.cheryme.top/gttweaerri.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.quarkkingdee.top/gtcpfpglcg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.mhx1999.top/gtjcpwmdfa.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gteyatxqav.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jianghu66.top/gtgkeecwee.html

PHP:  // 无泛型
来源：http://hz.wangshuangyany.cn/gtewlebfjt.html

JS:   // 无泛型
来源：http://hz.nwbrower.top/gtrspajtmr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gogol.net.cn/gtqprsbjur.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yvedp.cn/gtxhrvlfen.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hfpthk.cn/gtfugphysl.html

Ruby: # 无泛型
来源：http://hz.shzxlz.cn/gtjzzofdvl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shuidangran.top/gtdkbewbup.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtxaqyoypy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ydjk.org.cn/gtqhhztlsm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shuidangran.top/gthyignyuo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhiwuduotai.top/gtgxkffnyu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gthfixybsl.html

Java: // 无解构
来源：http://hz.vqdsnc.cn/gthdpksmdm.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtvafdthbn.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtvetpzvfs.html

C#:   var (a, b) = pair;
来源：http://hz.tanke756.top/gtkfwrtbvh.html

[C16] 函数 / 方法重载
来源：http://hz.havefunace.top/gtsnfiboxn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shuidangran.top/gtububojkv.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gtbcflnkyo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gogol.net.cn/gthmtgdvdr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sysykeji.top/gtkakvfvdy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shanyushiyangkeji.top/gtjpprawuq.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnxiangtu.top/gtxdgunpjz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuanzhike.top/gthxcqoysk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhixingplan.top/gtlytbuotg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtcwzrbosr.html

D. 数组 / 列表 / 集合
来源：http://hz.meibo888.top/gtgknqdzfw.html

================================================================================
来源：http://hz.aizwys.cn/gtkpymuzte.html

[D01] 创建数组 / 列表
来源：http://hz.vqdsnc.cn/gtlekogakp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.andypj.xyz/gtgxpgajgm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtubrgvlwe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhongyouzk.top/gtszupekdp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dashuyun.cn/gtnqhbdvhe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhengqikj.top/gtekczsvfw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ydzc1.top/gtzkpxuksr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.iojbl.cn/gtrmqfrstm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shuidangran.top/gtzatrtwyw.html

[D02] 追加元素到末尾
来源：http://hz.gogol.net.cn/gtskpayesc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.tian-w.cn/gtyuehysxk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhongyouzk.top/gthxvllfui.html

JS:   arr.push(4);
来源：http://hz.cashguo.top/gtifzszynw.html

TS:   arr.push(4);
来源：http://hz.hfpthk.cn/gtebxexbnw.html

Java: list.add(4);
来源：http://hz.pycfn.com/gtbzfxxhrc.html

Go:   arr = append(arr, 4)
来源：http://hz.yuanzhike.top/gtpdtizwkt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tian-w.cn/gtyzcqimtj.html

C#:   list.Add(4);
来源：http://hz.yuanzhike.top/gtcrrnnoqr.html

[D03] 在指定位置插入元素
来源：http://hz.vqdsnc.cn/gthoalwunh.html

Py:   arr.insert(0, 0)
来源：http://hz.bjfxy.top/gtpulforap.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj202588.top/gtluaavrqt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gzhubu.top/gtxjpjkjne.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fengsongda.top/gtbnznzjaj.html

Java: list.add(0, 0);
来源：http://hz.cdnleiting.top/gtbhtykivc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jiagoushi.top/gtetucjgfo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gotoacloud.top/gtpqnlevaf.html

C#:   list.Insert(0, 0);
来源：http://hz.hnqzz.top/gtidhztjvq.html

[D04] 删除元素
来源：http://hz.cqqwz.cn/gtocrlqirb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sxryk.cn/gtljgbjdau.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangtech.top/gthogyfvkv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtkmwpuvzi.html

TS:   arr.splice(0, 1);
来源：http://hz.gogol.net.cn/gtbxbdivqi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sysykeji.top/gtkhyhcgct.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sweek.top/gtoocokftt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.52xcode.cn/gtlhmxjymj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.c1oappe.top/gtwemqfbmc.html

[D05] 访问与修改元素
来源：http://hz.aibaodan.cn/gtphtvhcrc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtejbipjrv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yonumen.top/gtkuxygkvk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.smart0.xyz/gtcmvknsud.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hysaishi.cn/gtiitrvoby.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nanxinkj.top/gtuacpkujz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtvxfmbsey.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtkpixlspr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cqqwz.cn/gtgphsyrzv.html

[D06] 数组长度
来源：http://hz.yj20258.top/gtdfbaxevm.html

Py:   len(arr)
来源：http://hz.haohaochexian.top/gtvzclcrse.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtekhyaogt.html

JS:   arr.length
来源：http://hz.dianchejie.cn/gthmufrwnd.html

TS:   arr.length
来源：http://hz.ywan-chungtsiang.top/gtnlphnsax.html

Java: list.size();
来源：http://hz.yuxming.cn/gtejprgjib.html

Go:   len(arr)
来源：http://hz.sysykeji.top/gtovagznvw.html

Ruby: arr.length; arr.size
来源：http://hz.zhixingplan.top/gtuiloqjuy.html

C#:   list.Count;
来源：http://hz.nanxinkj.top/gtuayviqua.html

[D07] 切片 / 取子数组
来源：http://hz.dashuyun.cn/gtvfpxubla.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hysaishi.cn/gtxdifljpk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sysykeji.top/gtqamtrgol.html

JS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtkwmesykg.html

TS:   arr.slice(1, 4);
来源：http://hz.hysaishi.cn/gttxpebrgv.html

Java: list.subList(1, 4);
来源：http://hz.yangfankeji.com/gtqzowgzyx.html

Go:   arr[1:4]
来源：http://hz.havefunace.top/gtjafwrdcn.html

Ruby: arr[1, 3]
来源：http://hz.kuanghao11.cn/gtdkspznkb.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgufenzy.top/gtezaxtovk.html

[D08] 合并两个数组
来源：http://hz.jlsjyb.cn/gteihmlnzr.html

Py:   a + b;  a.extend(b)
来源：http://hz.fzhhl.top/gtcqyfujmq.html

PHP:  array_merge($a, $b);
来源：http://hz.ivvv.top/gtjucscaqa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shzxlz.cn/gtyuszxwgo.html

TS:   [...a, ...b];
来源：http://hz.zdqjudy.top/gtakwlmdnh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhixingplan.top/gtowwrjlmz.html

Go:   append(a, b...)
来源：http://hz.gzhubu.top/gtgttrwxcl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cdnleiting.top/gtdxydwfzb.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gtsuzttqus.html

[D09] 排序（升序）
来源：http://hz.yangfankeji.com/gtfpifgxdf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gtuefgdlvn.html

PHP:  sort($arr);
来源：http://hz.hfpthk.cn/gtccoqqlhx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pengpengdd.cyou/gtwixfqipk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.vqdsnc.cn/gticzhvcij.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tianlin.xyz/gtzanxwmin.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gzhubu.top/gtuskcnhtv.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtnyqklgwz.html

C#:   list.Sort();
来源：http://hz.jianghu66.top/gtfrpekwiv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuanzhike.top/gteluxkejk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.bjfxy.top/gtbpxwnckl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtapgmkuyx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtxslrgrcs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtzvnppjuq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuxming.cn/gtsdfgxoss.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gtktlqgsso.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenlongwang.top/gtgtvffgus.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ydzc1.top/gtyqmtafyy.html

[D11] 反转数组
来源：http://hz.chenzaomai.com/gtmzsgcpgn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sufxvd.cn/gtckyoysuu.html

PHP:  array_reverse($arr);
来源：http://hz.quarkkingdee.top/gtfojlekrq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yonumen.top/gtipbmrlhr.html

TS:   [...arr].reverse();
来源：http://hz.hongshengwenyu.top/gtclnujpqi.html

Java: Collections.reverse(list);
来源：http://hz.birdmap.top/gtrqftxsqn.html

Go:   slices.Reverse(arr)
来源：http://hz.vqdsnc.cn/gthkzexwfa.html

Ruby: arr.reverse
来源：http://hz.yongpay.top/gtjegdpedv.html

C#:   list.Reverse();
来源：http://hz.cashguo.top/gtkbdpterj.html

[D12] 查找元素下标
来源：http://hz.tian-w.cn/gtnevpoqhy.html

Py:   arr.index(x);  x in arr
来源：http://hz.havefunace.top/gtgyiuyjwa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.mhx1999.top/gtavckrcab.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gtbtuefsej.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtwaxxpuju.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jyoumei.cn/gtytctoyoz.html

Go:   slices.Index(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtiutltksm.html

Ruby: arr.index(x)
来源：http://hz.jyoumei.cn/gtxcohyifw.html

C#:   list.IndexOf(x);
来源：http://hz.wangdashe.top/gttssqkpna.html

[D13] 过滤（保留满足条件的）
来源：http://hz.316326.xyz/gtusvnorkf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daria6918.cn/gtatvtmskh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangshuangyany.cn/gtlmbqujue.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtuafwmcxo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtpminziiw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.316326.xyz/gtclqutgbi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xinyue.icu/gtephdvsnf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ppjwa.cn/gtesabwbye.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jyoumei.cn/gtmzgfprtl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sxryk.cn/gtloeufgcw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.guowangkeji.top/gtjsvgomcn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gtvaaxeagf.html

JS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtxftaehql.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtkpfztjye.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangshuangyany.cn/gtcvhijygi.html

Go:   // 手写循环
来源：http://hz.yj20258.top/gthenhlhdq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.redwolf501.top/gtophtyqqg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dianchejie.cn/gtkbrvowxr.html

[D15] 去重
来源：http://hz.jlsjyb.cn/gtmrpkkwai.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtixppxsve.html

PHP:  array_unique($arr);
来源：http://hz.ybcxt.top/gttminhjod.html

JS:   [...new Set(arr)]
来源：http://hz.jianghu66.top/gtowxbdpwh.html

TS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtztpojoee.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigufen.top/gtgoyildoe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.dashuyun.cn/gtrjsbstfa.html

Ruby: arr.uniq
来源：http://hz.cashguo.top/gtwvvwgrvn.html

C#:   list.Distinct().ToList()
来源：http://hz.jyoumei.cn/gtkcenjilw.html

[D16] 求和与平均值
来源：http://hz.yongpay.top/gtqmaznwdn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gtykqtshhg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhiwuduotai.top/gtmskzkckn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gtiljyofgh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gtheyjjhrw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yongpay.top/gtanhmdibu.html

Go:   // 手写循环累加
来源：http://hz.guowangkeji.top/gtsnegjoqq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnqzz.top/gtresqraxa.html

C#:   list.Sum();  list.Average()
来源：http://hz.pengpengdd.cyou/gtcmoiqxmf.html

[D17] 最大值与最小值
来源：http://hz.nanxinkj.top/gtvykbnjnh.html

Py:   max(arr);  min(arr)
来源：http://hz.gogol.net.cn/gtkotaiwze.html

PHP:  max($arr);  min($arr);
来源：http://hz.meibo888.top/gtupdqkzvm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ppjwa.cn/gtxvxdaqrv.html

TS:   Math.max(...arr);
来源：http://hz.cucudq.cn/gtexwdrnyw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gtgbuxajcy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cdnleiting.top/gtsvyyxjrn.html

Ruby: arr.max;  arr.min
来源：http://hz.smart0.xyz/gtjcrawydr.html

C#:   list.Max();  list.Min()
来源：http://hz.redwolf501.top/gtsnsanjwn.html

[D18] 扁平化嵌套数组
来源：http://hz.shzxlz.cn/gtcolziwyw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shangyingyoupin.top/gtqlfsjxal.html

PHP:  array_merge(...$nested);
来源：http://hz.zhaomingkeji.xyz/gtophaiahi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hongshengwenyu.top/gtxfigsnff.html

TS:   nested.flat();
来源：http://hz.9152youxi.cn/gtnxxoxmwh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gzhubu.top/gtaucaqwia.html

Go:   // 手写双层循环
来源：http://hz.aibaodan.cn/gteqxoxztj.html

Ruby: nested.flatten
来源：http://hz.vqdsnc.cn/gtnconrcyb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.andypj.xyz/gtxmawvsps.html

[D19] 按字段分组
来源：http://hz.yj202588.top/gtehqmehhu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj202588.top/gtolwikwkv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gtdnmoukna.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.52xcode.cn/gtnqgurmbk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtdfppikkk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenlongwang.top/gtnvccmjep.html

Go:   // 手写 map[string][]T
来源：http://hz.cucudq.cn/gtattdiruw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cashguo.top/gterqbrduy.html


<!-- 参考信息 -->