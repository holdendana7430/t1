代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuanzhike.top/gtzwhtzkkh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cashguo.top/gtregnapml.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tanke756.top/gtteajermb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhijiandao.cn/gtsenkcxdy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cheryme.top/gtolhomnat.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yonumen.top/gtmrjrxxtp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtxcsfxtih.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.haohaochexian.top/gthfqlsppf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ivvv.top/gtcwuvvqws.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtpmigoovj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinghuilouyu.cn/gtgzwixsmh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ywan-chungtsiang.top/gtwkjwkwhi.html

Go:   // 无：用配置结构体参数
来源：http://hz.dashuyun.cn/gtxwrwzgrt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtrkpymadb.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtzmksocjh.html

[C05] 返回多个值
来源：http://hz.jinqigufen.top/gtmdmijmdj.html

Py:   return a, b
来源：http://hz.yj20258.top/gtvnxyfvee.html

PHP:  return [$a, $b];
来源：http://hz.daria6918.cn/gtryrnsada.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shanyushiyangtech.top/gthrdojmje.html

TS:   return { a, b };
来源：http://hz.jiagoushi.top/gtrpdwkgsv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cucudq.cn/gtykhxdsxr.html

Go:   return a, b
来源：http://hz.shzxlz.cn/gtmnheshlp.html

Ruby: return a, b
来源：http://hz.cqqwz.cn/gtubarwtah.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cucudq.cn/gtcsgskxfq.html

[C06] 匿名函数 / lambda
来源：http://hz.gaohongyu789.top/gtmnnremef.html

Py:   square = lambda x: x * x
来源：http://hz.ybcxt.top/gtmveodser.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shzxlz.cn/gtwkssknnm.html

JS:   const square = x => x * x;
来源：http://hz.daria6918.cn/gtemhcvney.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gtnrtsivur.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jqgufenzy.top/gthdfhxetx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.0kj1m.cn/gtnesbeigx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.c1oappe.top/gtmfnnzcis.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gtncscdzhq.html

[C07] 把函数作为参数传入
来源：http://hz.smart0.xyz/gtjyavdrxa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenjidiqi.icu/gtjvtcxege.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.vqdsnc.cn/gtgxozkbxz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yvedp.cn/gtimawwsee.html

TS:   arr.map(String)
来源：http://hz.zhijiandao.cn/gtvthnlmad.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.meibo888.top/gtswelnmom.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cucudq.cn/gtsfdtfbnm.html

Ruby: arr.map(&:upcase)
来源：http://hz.yonumen.top/gtjlkugqby.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.haohaochexian.top/gtymzxojpk.html

[C08] 闭包
来源：http://hz.chenlongwang.top/gtvezngvor.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.meibo888.top/gtmvhyhkdw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxinkj.top/gteellipvk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtwbhikefg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gturohmwtw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gaohongyu789.top/gteikywjaz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gogol.net.cn/gtfxcxcpbe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yanxiufei.cn/gtsbdprgdy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtyolpzgab.html

[C09] 递归
来源：http://hz.yonumen.top/gtprtymneo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtrqkingea.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenzaomai.com/gtvqsnncxi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtnbqqenhm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gtakxzwmfc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.c1oappe.top/gtvssmmdzy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zycfv.cn/gtjwdurekp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sweek.top/gtunkrhccz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ivvv.top/gtzgbebdzg.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gttoxwzyyg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.vqdsnc.cn/gtwertvllx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxinkj.top/gtqvdqqqij.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yvedp.cn/gtxwgkrtgj.html

TS:   同 JS
来源：http://hz.vqdsnc.cn/gttsmhcech.html

Java: 方法内为块级作用域
来源：http://hz.yanxiufei.cn/gtpuwaczlo.html

Go:   花括号块级作用域
来源：http://hz.yueranfly.top/gtbqjptdkx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenlongwang.top/gtxavroffa.html

C#:   块级作用域
来源：http://hz.hongshengwenyu.top/gtyxwcktit.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gttuhgmpcv.html

Py:   from module import func
来源：http://hz.guowangkeji.top/gtdjmfijjt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hfpthk.cn/gtvbcpwvni.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tianlin.xyz/gtkkruzssr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shuidangran.top/gtciaasrav.html

Java: import java.util.List;
来源：http://hz.fzhhl.top/gtrotogggl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tian-w.cn/gtziyuoaaj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhengqikj.top/gtqzrquswd.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtrgevpvas.html

[C12] 立即执行函数 IIFE
来源：http://hz.xinyue.icu/gtclldccmk.html

Py:   (lambda: print("run"))()
来源：http://hz.guannengcc.top/gtdnejmudv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.dianchejie.cn/gtvkrywrpm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtzojkohoe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtkukdtbys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.fengsongda.top/gtoqgtieqe.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhijiandao.cn/gthpitdnwz.html

Ruby: -> { puts "run" }.call
来源：http://hz.yueranfly.top/gtcbglkltj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gtpznburif.html

[C13] 类型声明 / 类型注解
来源：http://hz.ppjwa.cn/gtipdmbndj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aizwys.cn/gtqewuonrt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.kuanghao11.cn/gttoqwdsbo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yongpay.top/gtiliyzbwo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.smart0.xyz/gtstionyqk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtijjwdlil.html

Go:   func add(a, b int) int
来源：http://hz.xylfe.cn/gtpbfhlcvd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pengpengdd.cyou/gtmqmzfszf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgfzy.top/gtkgftryln.html

[C14] 泛型函数
来源：http://hz.jinqigfzy.top/gtzfvcltiv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuanzx.com/gtlnpfstyf.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gtylxrudcn.html

JS:   // 无泛型
来源：http://hz.aibaodan.cn/gtbeulrlsw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gthtxpdsrj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cheryme.top/gtqkxpqgme.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xziqi.cn/gtdvyeeihz.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gttuaygxkw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.redwolf501.top/gthrhhzkma.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtwbsjrgsm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgufenzy.top/gtluqroijo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.birdmap.top/gtrfofimzl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtvwwdfbks.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gotoacloud.top/gtgthiegte.html

Java: // 无解构
来源：http://hz.cheryme.top/gtcpqoplra.html

Go:   // 无解构
来源：http://hz.xylfe.cn/gtnuzbxkig.html

Ruby: a, b = pair
来源：http://hz.guannengcc.top/gtyodmsiyl.html

C#:   var (a, b) = pair;
来源：http://hz.xinyue.icu/gtnswonauz.html

[C16] 函数 / 方法重载
来源：http://hz.pengpengdd.cyou/gttfuylscq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tian-w.cn/gtzvpsckls.html

PHP:  // 无重载
来源：http://hz.jinyuanbaomall.cn/gtsdlagrfz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jiagoushi.top/gtotvdrlkt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cdnleiting.top/gtivjyvxbn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daxiang520.top/gtbbutdfdv.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtsulvvaws.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pycfn.com/gtjcopcqnh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shuidangran.top/gtaoawjtuo.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtdxfujcsl.html

D. 数组 / 列表 / 集合
来源：http://hz.xylfe.cn/gtegobrxps.html

================================================================================
来源：http://hz.aibaodan.cn/gtxnxmykuy.html

[D01] 创建数组 / 列表
来源：http://hz.gogol.net.cn/gtirpoyxlq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj202588.top/gtlnhhrmhu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhengqikj.top/gtyjuesegj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yongpay.top/gtngjcoixw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangshuangyany.cn/gtbzvgnrxg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.andypj.xyz/gtogmumgym.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgufenzy.top/gtnlszwcyt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shzxlz.cn/gtkizdspqz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nwbrower.top/gtbwlrdjjm.html

[D02] 追加元素到末尾
来源：http://hz.52xcode.cn/gtcautxlav.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.smart0.xyz/gtpvgoaffm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jlsjyb.cn/gtdktuhbsd.html

JS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtybkoifnn.html

TS:   arr.push(4);
来源：http://hz.ydzc1.top/gtustohema.html

Java: list.add(4);
来源：http://hz.cheryme.top/gtyqwvylbe.html

Go:   arr = append(arr, 4)
来源：http://hz.xinyue.icu/gtoukgngfx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pycfn.com/gtyxjvdurg.html

C#:   list.Add(4);
来源：http://hz.xuanzx.com/gtdydygeyl.html

[D03] 在指定位置插入元素
来源：http://hz.xingfuxueyuan.xyz/gtooyquerq.html

Py:   arr.insert(0, 0)
来源：http://hz.redwolf501.top/gtohhcrfoz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hfpthk.cn/gtbowzsbgs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgfzy.top/gtkcsmslre.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.316326.xyz/gtpyuhclju.html

Java: list.add(0, 0);
来源：http://hz.jlsjyb.cn/gtckepughm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xylfe.cn/gtjztjqzyt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gogol.net.cn/gtlwhxdtjg.html

C#:   list.Insert(0, 0);
来源：http://hz.cashguo.top/gtlljsirim.html

[D04] 删除元素
来源：http://hz.zhijiandao.cn/gtxjxdahkj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xziqi.cn/gtkeqnsurz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jyoumei.cn/gtlfnhxlcv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj202588.top/gtpbncseod.html

TS:   arr.splice(0, 1);
来源：http://hz.xuetiantiany.cn/gtkqggikev.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ybcxt.top/gtsaflccup.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cqqwz.cn/gtaqzckikd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sweek.top/gtfknpwbqi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhengqikj.top/gtjwwncwix.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gtoxtwncrn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtudhxxcvx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xinyue.icu/gtkbdzmyyh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hnqzz.top/gtwkhtssob.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtvjkqmsti.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.0kj1m.cn/gtlmbmrbum.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hnqzz.top/gtpyczdpzy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtzqfkicym.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yueranfly.top/gtrkgsnnmd.html

[D06] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtkroqkaie.html

Py:   len(arr)
来源：http://hz.cashguo.top/gtfrsncvqb.html

PHP:  count($arr);
来源：http://hz.nwbrower.top/gtjryxbgmy.html

JS:   arr.length
来源：http://hz.hongshengwenyu.top/gtccfwnygy.html

TS:   arr.length
来源：http://hz.aibaodan.cn/gtuoxcsatz.html

Java: list.size();
来源：http://hz.ydzc1.top/gtxnppbjbk.html

Go:   len(arr)
来源：http://hz.sweek.top/gtfoeubpak.html

Ruby: arr.length; arr.size
来源：http://hz.nanxuanxn.top/gtomspxhsl.html

C#:   list.Count;
来源：http://hz.hnqzz.top/gtoefgmdmx.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gttgublyrt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.haohaochexian.top/gtevwkjdca.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gaohongyu789.top/gtjmhqytwh.html

JS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gtixrkpyuh.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtlfkdfcyf.html

Java: list.subList(1, 4);
来源：http://hz.chenzaomai.com/gtbrjvmgty.html

Go:   arr[1:4]
来源：http://hz.kuanghao11.cn/gtrxspwebs.html

Ruby: arr[1, 3]
来源：http://hz.yj202588.top/gtdlcogwmh.html

C#:   list.GetRange(1, 3);
来源：http://hz.pengpengdd.cyou/gtheyuuizo.html

[D08] 合并两个数组
来源：http://hz.yuanzhike.top/gtsxrcegdh.html

Py:   a + b;  a.extend(b)
来源：http://hz.guannengcc.top/gthnxuoahq.html

PHP:  array_merge($a, $b);
来源：http://hz.52xcode.cn/gtardkjrnd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.pycfn.com/gtuxzrgtlk.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtgbrbctps.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhoulong.xyz/gtfqnpunlk.html

Go:   append(a, b...)
来源：http://hz.bjfxy.top/gtrecxbwfj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cqqwz.cn/gtdmtoalnq.html

C#:   a.Concat(b).ToList()
来源：http://hz.tianlin.xyz/gtcocviqyz.html

[D09] 排序（升序）
来源：http://hz.yj20258888.top/gtfgbhvwtf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtkufxycsx.html

PHP:  sort($arr);
来源：http://hz.dashuyun.cn/gtgfigmcyg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cucudq.cn/gtdvjnsupo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.meibo888.top/gthidyjqpp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daria6918.cn/gtivoroopf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gtxechsoie.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtsgdnmqql.html

C#:   list.Sort();
来源：http://hz.jinyuanbaomall.cn/gtsegcrstd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.vqdsnc.cn/gtaqdnkmwb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.pycfn.com/gtoegpggtg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhoulong.xyz/gtkhkrkmog.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtgytyzvqk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtbdaehofg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cdnleiting.top/gtysbzxchz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.mhx1999.top/gtthjbytbt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yanxiufei.cn/gtvrtvqjbt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gtxrcywnkr.html

[D11] 反转数组
来源：http://hz.nanxuanxn.top/gtruymymrr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.9152youxi.cn/gtkjxkzpre.html

PHP:  array_reverse($arr);
来源：http://hz.gogol.net.cn/gthelulftv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhaomingkeji.xyz/gtmiondrkf.html

TS:   [...arr].reverse();
来源：http://hz.pycfn.com/gtdwczaqwg.html

Java: Collections.reverse(list);
来源：http://hz.yj20258888.top/gtrkbillko.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258.top/gtmpaxybyw.html

Ruby: arr.reverse
来源：http://hz.pycfn.com/gtjrbfkivv.html

C#:   list.Reverse();
来源：http://hz.gotoacloud.top/gtgybuxdwy.html

[D12] 查找元素下标
来源：http://hz.ivvv.top/gtbumpiutd.html

Py:   arr.index(x);  x in arr
来源：http://hz.fzhhl.top/gthdoqofcu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.quarkkingdee.top/gthdgmkent.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.feifeiyinyue.top/gthhevlkgx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gtebmrsuop.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ywan-chungtsiang.top/gtjqctjsub.html

Go:   slices.Index(arr, x)
来源：http://hz.yongpay.top/gtptqsbpui.html

Ruby: arr.index(x)
来源：http://hz.yvedp.cn/gtacytahld.html

C#:   list.IndexOf(x);
来源：http://hz.ywan-chungtsiang.top/gtviyhhnzx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cdnleiting.top/gtsyhhrwfa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgufenzy.top/gtgdglshsd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenzaomai.com/gtuxfdrucy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtmianyerx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtukbcysbx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangtech.top/gttmhuyfdk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fzhhl.top/gtchindeyd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.birdmap.top/gtfviziamo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj20258888.top/gtlbezerxd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.feifeiyinyue.top/gtnvbrexsp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fengsongda.top/gtcuoiozor.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.9152youxi.cn/gtzdvyrqga.html

JS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtgkfirdjm.html

TS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gtwnvdodbq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gtthgsvepq.html

Go:   // 手写循环
来源：http://hz.jinyuanbaomall.cn/gtgrzehnxr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jianghu66.top/gtkssqsvtu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pengpengdd.cyou/gtncnvjgau.html

[D15] 去重
来源：http://hz.jinqigufen.top/gtuhvcerft.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtkggqbyet.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtgatxcxhl.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtkvlqevyx.html

TS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtrotrfnrm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtrcqzxglb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.havefunace.top/gtwcjmytmo.html

Ruby: arr.uniq
来源：http://hz.0kj1m.cn/gtetpnrhyg.html

C#:   list.Distinct().ToList()
来源：http://hz.yanxiufei.cn/gtdjizxavz.html

[D16] 求和与平均值
来源：http://hz.jlsjyb.cn/gtiageptrj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhijiandao.cn/gteasdrmxw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhongyouzk.top/gtgfkcwjdv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gteuleahwf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gtnkwgkxyw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shzxlz.cn/gtrtwsdzil.html

Go:   // 手写循环累加
来源：http://hz.bjfxy.top/gttiatlrsm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtpodvloxt.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gtxfnrqlfe.html

[D17] 最大值与最小值
来源：http://hz.0kj1m.cn/gtrpzbwfvt.html

Py:   max(arr);  min(arr)
来源：http://hz.pengpengdd.cyou/gtammokuyy.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenjidiqi.icu/gtiuzroiil.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinyuanbaomall.cn/gtxafqxays.html

TS:   Math.max(...arr);
来源：http://hz.wangshuangyany.cn/gtiewmekec.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gtxxgsvvym.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtbxwrpuvl.html

Ruby: arr.max;  arr.min
来源：http://hz.xuanzx.com/gtpfrtdedu.html

C#:   list.Max();  list.Min()
来源：http://hz.zhoulong.xyz/gtzkoypixx.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtphjpoaco.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fzhhl.top/gtbxvuypll.html

PHP:  array_merge(...$nested);
来源：http://hz.52xcode.cn/gtbfwjvsqs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.kuanghao11.cn/gtrykickxj.html

TS:   nested.flat();
来源：http://hz.jinyuanbaomall.cn/gtrwcaaigv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinqigufen.top/gtjiabnkmw.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtdufmfint.html

Ruby: nested.flatten
来源：http://hz.316326.xyz/gtriwvtnko.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cucudq.cn/gtlyjepvzq.html

[D19] 按字段分组
来源：http://hz.fzhhl.top/gtlelltxcp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hnxiangtu.top/gtuzrngqna.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ywan-chungtsiang.top/gtqubtxwal.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.snrcjt.cn/gtytytqsny.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtzkhvhxtj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fengsongda.top/gtsykhgrff.html

Go:   // 手写 map[string][]T
来源：http://hz.shuidangran.top/gtkfqobwod.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nanxuanxn.top/gtmkukfsqy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hfpthk.cn/gtktptlhvh.html

[D20] 统计每个元素出现次数
来源：http://hz.hammf.cn/gthvywfepg.html

Py:   Counter(arr)
来源：http://hz.mhx1999.top/gtabulqdoq.html

PHP:  array_count_values($arr);
来源：http://hz.mhx1999.top/gtzyjveihk.html


<!-- 参考信息 -->