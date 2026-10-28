代发 wailian999

[C02] 默认参数
来源：http://hz.yonumen.top/gtlcbiwotv.html

Py:   def greet(name="World"): return name
来源：http://hz.tianlin.xyz/gtnzdcgaro.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhongyouzk.top/gtbypofidj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.dianchejie.cn/gtnofxvfzz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtbihczhig.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgfzy.top/gtgrixmlwb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jianghu66.top/gtoojwcwbc.html

Ruby: def greet(name = "World") = name
来源：http://hz.xingfuxueyuan.xyz/gtaaxjbyra.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.iojbl.cn/gtrrllafkm.html

[C03] 可变参数
来源：http://hz.yj202588.top/gtezttlowp.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gttqxcosfh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gotoacloud.top/gtyggzqhuq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtegkavbab.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtaitfassn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.svipenyu.cn/gthvkhyyqy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinghuilouyu.cn/gtuwiebkyj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydjk.org.cn/gtmedkxwfi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hywenlv.cn/gtcapmsffy.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangkeji.top/gtpgtptskq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.dianchejie.cn/gtlzykfqsj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cucudq.cn/gtllcaiqej.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtyqafeawl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jqgufenzy.top/gtniqtswoo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.feifeiyinyue.top/gtgvkirsbk.html

Go:   // 无：用配置结构体参数
来源：http://hz.cucudq.cn/gthsxjftdc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtzejujjrr.html

C#:   f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtapantmvy.html

[C05] 返回多个值
来源：http://hz.jlsjyb.cn/gtfiwdfrsk.html

Py:   return a, b
来源：http://hz.hywenlv.cn/gtpkzrlnbi.html

PHP:  return [$a, $b];
来源：http://hz.daria6918.cn/gtziomlyhg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ppjwa.cn/gtywrqzwhq.html

TS:   return { a, b };
来源：http://hz.quarkkingdee.top/gtfwbycbam.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sysykeji.top/gtedsamuuc.html

Go:   return a, b
来源：http://hz.jqgufenzy.top/gtqtrnhbvr.html

Ruby: return a, b
来源：http://hz.yuanzhike.top/gtcnolfnav.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydjk.org.cn/gtoshivfif.html

[C06] 匿名函数 / lambda
来源：http://hz.wangshuangyany.cn/gtkuyoznsl.html

Py:   square = lambda x: x * x
来源：http://hz.hnqzz.top/gtbwqptpxn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhixingplan.top/gtdnemigkc.html

JS:   const square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gteamjeqkx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gtfkmzbowh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhijiandao.cn/gtbkhpujsa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tanke756.top/gtmknfsdkb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hongshengwenyu.top/gtzguyhaot.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.316326.xyz/gtfsiqtnze.html

[C07] 把函数作为参数传入
来源：http://hz.yongpay.top/gtijngoxrp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jianghu66.top/gtjwnbsabj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhijiandao.cn/gtikfuniep.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.snrcjt.cn/gtpmcblkgr.html

TS:   arr.map(String)
来源：http://hz.dashuyun.cn/gttfgnmhqe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guannengcc.top/gtmbytgycw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fzhhl.top/gtaykwgqdo.html

Ruby: arr.map(&:upcase)
来源：http://hz.yueranfly.top/gtbzlatrad.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yvedp.cn/gtwakjzwfe.html

[C08] 闭包
来源：http://hz.zhiwuduotai.top/gtkhnfndhu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydzc1.top/gtfgekcnvn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.kuanghao11.cn/gtiwxvqgwd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtrpuzdiqi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtkfmxngdy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shuidangran.top/gtyimrixih.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cqqwz.cn/gtgxbmtbzn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhongyouzk.top/gtcufwqbcd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtjjfesfxb.html

[C09] 递归
来源：http://hz.snrcjt.cn/gthhvhugvq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.meibo888.top/gtxikgyydi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenzaomai.com/gtrlvgfrjy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gthvfufjxe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.9152youxi.cn/gtbufqohlv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnxiangtu.top/gtftvjlxcm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yonumen.top/gtlxgqowst.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.iojbl.cn/gtrxshdewy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnqzz.top/gtmxddsbrt.html

[C10] 变量作用域
来源：http://hz.xylfe.cn/gtfgwailjq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zdqjudy.top/gtulnaperg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.chenjidiqi.icu/gtcrrnhluj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tanke756.top/gtjvarmxuf.html

TS:   同 JS
来源：http://hz.ehwqpu.com/gtcmwftydq.html

Java: 方法内为块级作用域
来源：http://hz.52xcode.cn/gtansmnhhk.html

Go:   花括号块级作用域
来源：http://hz.cqqwz.cn/gtcpdkzxed.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dianchejie.cn/gtjkgsfihr.html

C#:   块级作用域
来源：http://hz.yuxming.cn/gtakuajvpn.html

[C11] 模块导入与导出
来源：http://hz.sufxvd.cn/gtzootwqsb.html

Py:   from module import func
来源：http://hz.shzxlz.cn/gtjcdrwqan.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gogol.net.cn/gthzjmwjuz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aibaodan.cn/gtnfejrcto.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hongshengwenyu.top/gtrpyxltak.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtaqfidkra.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.guowangkeji.top/gtlozvcxqa.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zycfv.cn/gtpkgrthcv.html

C#:   using System.Text;
来源：http://hz.dashuyun.cn/gtlrhimvgh.html

[C12] 立即执行函数 IIFE
来源：http://hz.birdmap.top/gtcrcenbrk.html

Py:   (lambda: print("run"))()
来源：http://hz.ppjwa.cn/gtnummnuev.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258.top/gtgqhcuewr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtqhijqbur.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtedjsdzxq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aibaodan.cn/gtrluqidzb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gtzghfxlpu.html

Ruby: -> { puts "run" }.call
来源：http://hz.jianghu66.top/gtxxxagixu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.52xcode.cn/gtqmuruefp.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtewfvvabx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuetiantiany.cn/gtvhxoubpk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtldgxvsab.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tian-w.cn/gtgnxbuupq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtzkzspfmo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtfxxremcl.html

Go:   func add(a, b int) int
来源：http://hz.jianghu66.top/gtdixohfds.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258.top/gtodoomqxs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guannengcc.top/gtrvfvpyfy.html

[C14] 泛型函数
来源：http://hz.daxiang520.top/gtxqctgaik.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gaohongyu789.top/gtlawfubfc.html

PHP:  // 无泛型
来源：http://hz.xuetiantiany.cn/gtdugmqbxx.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtdqphndmw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fengsongda.top/gtsiwvzdsx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guowangkeji.top/gtjwsurbgp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.quarkkingdee.top/gtupnjljqd.html

Ruby: # 无泛型
来源：http://hz.hywenlv.cn/gttpmvyids.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.meibo888.top/gtvihrbpca.html

[C15] 解构 / 展开参数
来源：http://hz.jyoumei.cn/gtlduandgw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhaomingkeji.xyz/gttdwofscs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cashguo.top/gtsxygmzys.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtfhbkuznm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hywenlv.cn/gtwpyuuluz.html

Java: // 无解构
来源：http://hz.sysykeji.top/gtufodybdx.html

Go:   // 无解构
来源：http://hz.sufxvd.cn/gtjwqdrmyq.html

Ruby: a, b = pair
来源：http://hz.cdnleiting.top/gttfggcbpn.html

C#:   var (a, b) = pair;
来源：http://hz.shangyingyoupin.top/gtsmbbiefy.html

[C16] 函数 / 方法重载
来源：http://hz.yongpay.top/gttqswuosw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.redwolf501.top/gtnamexvwu.html

PHP:  // 无重载
来源：http://hz.zhijiandao.cn/gtafqkcwic.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtzprezxry.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yonumen.top/gtrhzflutg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.aizwys.cn/gttjdpbkyy.html

Go:   // 无重载：用不同函数名
来源：http://hz.guannengcc.top/gttsyzbtxo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gaohongyu789.top/gtettlrfdc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xingfuxueyuan.xyz/gtkmvqguhq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkroxpqns.html

D. 数组 / 列表 / 集合
来源：http://hz.xinyue.icu/gtsdsuqwts.html

================================================================================
来源：http://hz.ehwqpu.com/gtfclekhwe.html

[D01] 创建数组 / 列表
来源：http://hz.cucudq.cn/gtcrbqtcrw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tian-w.cn/gtqhsrxkwh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.0kj1m.cn/gtqbsxuwuy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sufxvd.cn/gtwxhjxjky.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.havefunace.top/gtfxrttpkc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinghuilouyu.cn/gtlklrkezp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.0kj1m.cn/gtsyfbblom.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dashuyun.cn/gtknuxculv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cashguo.top/gtahauztml.html

[D02] 追加元素到末尾
来源：http://hz.zdqjudy.top/gtfvygintf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.0kj1m.cn/gthuyyvfrp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenzaomai.com/gtqvtmikgl.html

JS:   arr.push(4);
来源：http://hz.sweek.top/gtwgchnudk.html

TS:   arr.push(4);
来源：http://hz.smart0.xyz/gtfuczihxf.html

Java: list.add(4);
来源：http://hz.hongshengwenyu.top/gtmnfhcsgw.html

Go:   arr = append(arr, 4)
来源：http://hz.jianghu66.top/gthaznpqrn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.c1oappe.top/gtadcafbsa.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangtech.top/gtnysqimwh.html

[D03] 在指定位置插入元素
来源：http://hz.ydzc1.top/gtejtkbqtx.html

Py:   arr.insert(0, 0)
来源：http://hz.hnxiangtu.top/gtegglmqxn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jlsjyb.cn/gtcxxnqbto.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jlsjyb.cn/gtynjvetoz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xuanzx.com/gtfsmfmopu.html

Java: list.add(0, 0);
来源：http://hz.cheryme.top/gtvdiqgcdo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shanyushiyangkeji.top/gtxgkpgrso.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258888.top/gtftgsmbby.html

C#:   list.Insert(0, 0);
来源：http://hz.pycfn.com/gtramwnkxe.html

[D04] 删除元素
来源：http://hz.ywan-chungtsiang.top/gtkhomscxe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtenoeobut.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangkeji.top/gtcgdkwzsf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gtofcrtkrl.html

TS:   arr.splice(0, 1);
来源：http://hz.tanke756.top/gtvujtolmr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtanlusbxo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.tanke756.top/gtgvoslxqx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.svipenyu.cn/gtgnfuqwwt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtzagjxuzi.html

[D05] 访问与修改元素
来源：http://hz.tian-w.cn/gttluyridk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtsnscfvnp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigufen.top/gtholyewsc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jqgufenzy.top/gtjjwzpqjg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigufen.top/gtsztamdxh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gtqcguebxh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtizdzbifr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtcweixorp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jlsjyb.cn/gtvxwpjuzh.html

[D06] 数组长度
来源：http://hz.jqgufenzy.top/gtxarqpgzv.html

Py:   len(arr)
来源：http://hz.ybcxt.top/gtpxjtmxap.html

PHP:  count($arr);
来源：http://hz.hnxiangtu.top/gtyzkelsri.html

JS:   arr.length
来源：http://hz.xziqi.cn/gthvstdxef.html

TS:   arr.length
来源：http://hz.dashuyun.cn/gtpwfkowrx.html

Java: list.size();
来源：http://hz.iojbl.cn/gtyidfqubb.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtsgkxtcss.html

Ruby: arr.length; arr.size
来源：http://hz.yangfankeji.com/gtjxluiqsf.html

C#:   list.Count;
来源：http://hz.yj20258888.top/gtyifbpcam.html

[D07] 切片 / 取子数组
来源：http://hz.kuanghao11.cn/gtezvuadbh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtpxyolfvi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.snrcjt.cn/gtvnpufuqd.html

JS:   arr.slice(1, 4);
来源：http://hz.52xcode.cn/gttzcvwnuw.html

TS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtorwzwuox.html

Java: list.subList(1, 4);
来源：http://hz.yuxming.cn/gtclybvaie.html

Go:   arr[1:4]
来源：http://hz.jinghuilouyu.cn/gtxdxsvlxp.html

Ruby: arr[1, 3]
来源：http://hz.xylfe.cn/gtpmryfnva.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtwrgeurmr.html

[D08] 合并两个数组
来源：http://hz.zhengqikj.top/gtrujqjyhu.html

Py:   a + b;  a.extend(b)
来源：http://hz.fengsongda.top/gtwuknnnlg.html

PHP:  array_merge($a, $b);
来源：http://hz.zhongyouzk.top/gtivqxvxla.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gtseizfwaf.html

TS:   [...a, ...b];
来源：http://hz.c1oappe.top/gtuuzydmuq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hfpthk.cn/gtlgxymffd.html

Go:   append(a, b...)
来源：http://hz.ppjwa.cn/gturttgzev.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhongyouzk.top/gtdqgkbmfc.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenzaomai.com/gtqffeqxce.html

[D09] 排序（升序）
来源：http://hz.yueranfly.top/gtatgmohpe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtrjesirjf.html

PHP:  sort($arr);
来源：http://hz.quarkkingdee.top/gtzekupmrr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aibaodan.cn/gtczwkxrke.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.9152youxi.cn/gtexeldoha.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ivvv.top/gtwekhflvo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtskdsciaq.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtznobuloe.html

C#:   list.Sort();
来源：http://hz.zhoulong.xyz/gtzghbbbvt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gtyyijmhme.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtqtrhrbvs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gthvpbvgyk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtgaybfyut.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtgbqfywrj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.316326.xyz/gtomunczaw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhiwuduotai.top/gtlaigykep.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hammf.cn/gtocintlvo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtiuvumpst.html

[D11] 反转数组
来源：http://hz.cdnleiting.top/gtjxjrlurp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.0kj1m.cn/gthmqlnqnl.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gtswsixqdu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.c1oappe.top/gtxbcklhmb.html

TS:   [...arr].reverse();
来源：http://hz.yuanzhike.top/gtvzbceqnd.html

Java: Collections.reverse(list);
来源：http://hz.wangdashe.top/gtukiaxgow.html

Go:   slices.Reverse(arr)
来源：http://hz.daria6918.cn/gtvrujlymg.html

Ruby: arr.reverse
来源：http://hz.cheryme.top/gturmchkiz.html

C#:   list.Reverse();
来源：http://hz.guannengcc.top/gtoamuymyq.html

[D12] 查找元素下标
来源：http://hz.shuidangran.top/gtafixhnmw.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gtwhvwlaob.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guannengcc.top/gtulhaybfo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtuxlkhnud.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gtdrbtpxvn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.vqdsnc.cn/gtltdnsnwe.html

Go:   slices.Index(arr, x)
来源：http://hz.zhixingplan.top/gtkwdmsjwa.html

Ruby: arr.index(x)
来源：http://hz.cdnleiting.top/gtgvvcylpy.html

C#:   list.IndexOf(x);
来源：http://hz.guannengcc.top/gtgvobldkc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangshuangyany.cn/gtzwunrykt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hywenlv.cn/gtcpjpkdcx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cqqwz.cn/gtwpkjomaa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtteatjvbl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtguhbkfgh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtwmfpnfmi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinghuilouyu.cn/gtqvqvtipp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jyoumei.cn/gtgluqvktg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hysaishi.cn/gtitkmzcfx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sxryk.cn/gtpiqtpeny.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuetiantiany.cn/gtoxtnzzzk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gtzrppxljv.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtkizpfxtr.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtrzefymiy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtlqbultlj.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtpexcryxi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aibaodan.cn/gtcnkugxwr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangdashe.top/gtzkzqdqsi.html

[D15] 去重
来源：http://hz.dashuyun.cn/gthmlssthl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtkbnqpwon.html

PHP:  array_unique($arr);
来源：http://hz.sxryk.cn/gtmrgipczf.html

JS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtgytomnzb.html

TS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gthdfnpbap.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cqqwz.cn/gtpnnexosr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtjralzbku.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtajppgmwx.html

C#:   list.Distinct().ToList()
来源：http://hz.ivvv.top/gtpmpgvjqz.html

[D16] 求和与平均值
来源：http://hz.yj20258.top/gthyiqjnqf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.c1oappe.top/gtaxsaewym.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nwbrower.top/gtcebwgfoy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtmnwocgnm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtjlrkglap.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jiagoushi.top/gtcuqajotr.html

Go:   // 手写循环累加
来源：http://hz.snrcjt.cn/gtlsltyurv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj202588.top/gtifryokhu.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258.top/gtnnjewemy.html

[D17] 最大值与最小值
来源：http://hz.svipenyu.cn/gtbvnrafpk.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgufenzy.top/gtwldpgvhu.html

PHP:  max($arr);  min($arr);
来源：http://hz.xinyue.icu/gtzbyoecxk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgfzy.top/gtjmdrxohj.html

TS:   Math.max(...arr);
来源：http://hz.guannengcc.top/gtburtonwx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yangfankeji.com/gtmaakqyaq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtzayzceab.html

Ruby: arr.max;  arr.min
来源：http://hz.hammf.cn/gtltjxfafl.html

C#:   list.Max();  list.Min()
来源：http://hz.cashguo.top/gtijuygxeh.html

[D18] 扁平化嵌套数组
来源：http://hz.fengsongda.top/gtgfhplucv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yueranfly.top/gtpnbgcvfh.html

PHP:  array_merge(...$nested);
来源：http://hz.zycfv.cn/gtxeuskwyx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gaohongyu789.top/gtxlviziyu.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtgeahglvn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hfpthk.cn/gtdrximwxl.html

Go:   // 手写双层循环
来源：http://hz.meibo888.top/gtseczeefg.html

Ruby: nested.flatten
来源：http://hz.aibaodan.cn/gttapnpmmg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aibaodan.cn/gtmxvxksdo.html


<!-- 参考信息 -->