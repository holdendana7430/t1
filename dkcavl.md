代发 wailian999

Go:   a && b || !c
来源：http://hz.fzhhl.top/gtwwrtfjjd.html

Ruby: a && b || !c
来源：http://hz.aizwys.cn/gtqlkwhwpa.html

C#:   a && b || !c
来源：http://hz.yuanzhike.top/gtaseyhmyr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nanxinkj.top/gtlxbupctz.html

Py:   if not data: return
来源：http://hz.shanyushiyangtech.top/gtikokoesr.html

PHP:  if (!$data) { return; }
来源：http://hz.jqgfzy.top/gtkgcdjsfq.html

JS:   if (!data) return;
来源：http://hz.snrcjt.cn/gtphhqgfdk.html

TS:   if (!data) return;
来源：http://hz.jyoumei.cn/gtwxkynmxi.html

Java: if (data == null) return;
来源：http://hz.zdqjudy.top/gtfzflvnzb.html

Go:   if data == nil { return }
来源：http://hz.zhiwuduotai.top/gtrhwywjlc.html

Ruby: return if data.nil?
来源：http://hz.ivvv.top/gtjykzoxwg.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtjgigsbzs.html

================================================================================
来源：http://hz.yonumen.top/gtzlmmzsxn.html

C. 函数与作用域
来源：http://hz.jinqigfzy.top/gtpsycjzzj.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmkjwqxfz.html

[C01] 定义函数
来源：http://hz.xinyue.icu/gtfvtnwfte.html

Py:   def add(a, b): return a + b
来源：http://hz.nwbrower.top/gtmczcrjcm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtnubwvdnj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtiwszvtgc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtvfbwgolg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtcvoupydv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ivvv.top/gtulfdgrud.html

Ruby: def add(a, b); a + b; end
来源：http://hz.dashuyun.cn/gtnpzpnsix.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gttypztxor.html

[C02] 默认参数
来源：http://hz.yangfankeji.com/gtxzgrpnel.html

Py:   def greet(name="World"): return name
来源：http://hz.316326.xyz/gtxmnexwwz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.iojbl.cn/gtptzgstoe.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinqigfzy.top/gtpbpzpqlp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daria6918.cn/gtbcsferqm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xuanzx.com/gtgxqstoua.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuanzhike.top/gtvqwtcrgm.html

Ruby: def greet(name = "World") = name
来源：http://hz.316326.xyz/gtkijubsbo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnqzz.top/gtcdkodald.html

[C03] 可变参数
来源：http://hz.hywenlv.cn/gtwwmxcbwg.html

Py:   def total(*args): return sum(args)
来源：http://hz.yueranfly.top/gteubreekd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yonumen.top/gtdndiczkw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xuanzx.com/gtasrhckfx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtcsnrylib.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hongshengwenyu.top/gtmllnwkds.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hysaishi.cn/gtegliejrq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.haohaochexian.top/gtgbxdaeed.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.svipenyu.cn/gtwfzgvcvw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tanke756.top/gtukwxqxju.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.dianchejie.cn/gtcmtlsskc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sweek.top/gtuxieypab.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtcwessrxh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cucudq.cn/gtkcbunkqm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.svipenyu.cn/gtpeclwwfk.html

Go:   // 无：用配置结构体参数
来源：http://hz.sysykeji.top/gtpfkllwdj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gteqmnludi.html

C#:   f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtfkfbgfae.html

[C05] 返回多个值
来源：http://hz.yonumen.top/gtbtqigifk.html

Py:   return a, b
来源：http://hz.mhx1999.top/gtushqdhtl.html

PHP:  return [$a, $b];
来源：http://hz.cashguo.top/gthdruspko.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydjk.org.cn/gtqnmcwozs.html

TS:   return { a, b };
来源：http://hz.ivvv.top/gtmamvrthi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gaohongyu789.top/gtyxdteygw.html

Go:   return a, b
来源：http://hz.sysykeji.top/gtxasgtfcv.html

Ruby: return a, b
来源：http://hz.nanxinkj.top/gtepxkbieh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yongpay.top/gtycqmoprb.html

[C06] 匿名函数 / lambda
来源：http://hz.316326.xyz/gtrmhyhdcm.html

Py:   square = lambda x: x * x
来源：http://hz.bjfxy.top/gtuyvayarv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.vqdsnc.cn/gtvsfmkmrr.html

JS:   const square = x => x * x;
来源：http://hz.9152youxi.cn/gtwlhncxsm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sufxvd.cn/gtzkffcnoj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jianghu66.top/gtemgarjzb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shanyushiyangtech.top/gtxxzonaja.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shuidangran.top/gtebivutsw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yangfankeji.com/gtplyewicf.html

[C07] 把函数作为参数传入
来源：http://hz.cheryme.top/gtoirhmppu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yuxming.cn/gtedowilgs.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj202588.top/gtctunxjdv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.havefunace.top/gtwbyfhixf.html

TS:   arr.map(String)
来源：http://hz.hysaishi.cn/gtdgvrurwh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.andypj.xyz/gtqtrhrtev.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shangyingyoupin.top/gtgoytapmb.html

Ruby: arr.map(&:upcase)
来源：http://hz.cashguo.top/gtujttfdmw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hywenlv.cn/gtobvzmieq.html

[C08] 闭包
来源：http://hz.yj20258.top/gtkymswzmq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigfzy.top/gttyzodcff.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.meibo888.top/gtatwpvvkh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtunjvnjki.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtfsampbhk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnxiangtu.top/gtewfzbrmw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.mhx1999.top/gtyhmxpvpt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.birdmap.top/gtexyfesyo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gttiyzwvuj.html

[C09] 递归
来源：http://hz.yj202588.top/gtectocyjo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtrljkphoi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.iojbl.cn/gtkpmyxyeq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhongyouzk.top/gtypanayin.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hongshengwenyu.top/gtmdukblss.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.guowangkeji.top/gtartvyiqp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yongpay.top/gturjitkpp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ivvv.top/gtpkxnqdfe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yueranfly.top/gtgoybqhpw.html

[C10] 变量作用域
来源：http://hz.snrcjt.cn/gtrcbmdkqr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pengpengdd.cyou/gtvgcblhiq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xziqi.cn/gtpwbkfaqu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigufen.top/gtpviroigl.html

TS:   同 JS
来源：http://hz.fengsongda.top/gteaakeaqi.html

Java: 方法内为块级作用域
来源：http://hz.birdmap.top/gtxxefcizu.html

Go:   花括号块级作用域
来源：http://hz.ydzc1.top/gtcapybinj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.feifeiyinyue.top/gtijmfmknc.html

C#:   块级作用域
来源：http://hz.birdmap.top/gtkzwdsugl.html

[C11] 模块导入与导出
来源：http://hz.gotoacloud.top/gtwvgfaqsn.html

Py:   from module import func
来源：http://hz.guowangkeji.top/gtyfwblkfo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xinyue.icu/gtavhalylz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gtywmzhypf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtkergtnvp.html

Java: import java.util.List;
来源：http://hz.tanke756.top/gtdgopadcl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.guowangkeji.top/gtczhuqbjm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydzc1.top/gtowfrqtgi.html

C#:   using System.Text;
来源：http://hz.xylfe.cn/gtkazumlwy.html

[C12] 立即执行函数 IIFE
来源：http://hz.shzxlz.cn/gtajxpefsb.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258.top/gtwracofcw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.bjfxy.top/gtvitcsvmm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtltspdjxf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gtkntabxwi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ehwqpu.com/gtmurctgdk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hfpthk.cn/gtuqtmohej.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinqigfzy.top/gtpkluavww.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.bjfxy.top/gtjnoatchb.html

[C13] 类型声明 / 类型注解
来源：http://hz.wangdashe.top/gtligeiahc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aibaodan.cn/gtjbjoluqa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtzwihqxoq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.smart0.xyz/gtesmdggck.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.feifeiyinyue.top/gtwsovmpss.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtytrtcvqv.html

Go:   func add(a, b int) int
来源：http://hz.nwbrower.top/gtagycqeaa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtwwlfqhgr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aibaodan.cn/gtxvoltzey.html

[C14] 泛型函数
来源：http://hz.jqgufenzy.top/gtpduijpft.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuetiantiany.cn/gtrdwgkafa.html

PHP:  // 无泛型
来源：http://hz.xuetiantiany.cn/gtfdjrwzqk.html

JS:   // 无泛型
来源：http://hz.jyoumei.cn/gtmyiuhrtf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhoulong.xyz/gtfzgrgyaz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yueranfly.top/gtqnvafmwt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.birdmap.top/gtrpbbelev.html

Ruby: # 无泛型
来源：http://hz.xuetiantiany.cn/gthayavwni.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ehwqpu.com/gtvhfxrdqr.html

[C15] 解构 / 展开参数
来源：http://hz.ybcxt.top/gttrrgdtew.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.smart0.xyz/gtexflvaks.html

PHP:  [$a, $b] = $pair;
来源：http://hz.bjfxy.top/gtviorfkhd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhaomingkeji.xyz/gtovmvwttn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hfpthk.cn/gtlfcntbhw.html

Java: // 无解构
来源：http://hz.jianghu66.top/gtfvcnhxxh.html

Go:   // 无解构
来源：http://hz.zhixingplan.top/gtumdaovae.html

Ruby: a, b = pair
来源：http://hz.yuxming.cn/gttlykbyof.html

C#:   var (a, b) = pair;
来源：http://hz.sxryk.cn/gtqkabnhzp.html

[C16] 函数 / 方法重载
来源：http://hz.guowangkeji.top/gtbmrxmboy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinghuilouyu.cn/gthcsmoang.html

PHP:  // 无重载
来源：http://hz.ydjk.org.cn/gtmnminlrd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.mhx1999.top/gtgfevowwl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258888.top/gtejmwplme.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinqigfzy.top/gtbyxyolsy.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhongyouzk.top/gtawjtslcp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtprfojmcp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.snrcjt.cn/gtzyipwzvw.html

================================================================================
来源：http://hz.jqgfzy.top/gtggrpymwj.html

D. 数组 / 列表 / 集合
来源：http://hz.52xcode.cn/gtseqeulyb.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtrqmrmtpg.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtuipanywt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhijiandao.cn/gtwootcdkr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fengsongda.top/gtnmqwzljg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hywenlv.cn/gtgdyfuecw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxuanxn.top/gtdfgcazgy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zdqjudy.top/gtjivqyuis.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.meibo888.top/gttipgzfmk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.9152youxi.cn/gtayphvvka.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenzaomai.com/gtfzprujll.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gtmuatpbno.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yueranfly.top/gtpcyskqtj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.svipenyu.cn/gtvimtagbi.html

JS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtxvvznqgo.html

TS:   arr.push(4);
来源：http://hz.jyoumei.cn/gtxbwarndy.html

Java: list.add(4);
来源：http://hz.zhaomingkeji.xyz/gtiilhmhdw.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigfzy.top/gtzflkqhlo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.snrcjt.cn/gtigvxqncd.html

C#:   list.Add(4);
来源：http://hz.hywenlv.cn/gtunqksaeh.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gtcirqafeb.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtplscgjrh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtymnneqsr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnxiangtu.top/gtppisipud.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.havefunace.top/gtylrevafg.html

Java: list.add(0, 0);
来源：http://hz.wangshuangyany.cn/gthchmlqqa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.guowangkeji.top/gtzqqmpuhf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shanyushiyangtech.top/gttufgkfnq.html

C#:   list.Insert(0, 0);
来源：http://hz.zhixingplan.top/gtrbcnmibg.html

[D04] 删除元素
来源：http://hz.zycfv.cn/gtjnszqfwo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtrnqkdyim.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.andypj.xyz/gtxlxfiogt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnxiangtu.top/gtfwqxwmmf.html

TS:   arr.splice(0, 1);
来源：http://hz.ybcxt.top/gthexqipqe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigfzy.top/gtleapvqak.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtspniwmnw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtmazghwcl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.0kj1m.cn/gtclpqeest.html

[D05] 访问与修改元素
来源：http://hz.yangfankeji.com/gtvewnjsoc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtlhcysndn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtqxpuadsb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtbqqtuxxy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jyoumei.cn/gtsiiewxtr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zycfv.cn/gtjgmuvzsc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtrekjfdov.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtdmhqzogw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xylfe.cn/gtodsrvuni.html

[D06] 数组长度
来源：http://hz.cqqwz.cn/gtxanfmiqh.html

Py:   len(arr)
来源：http://hz.mhx1999.top/gtkawfvvbb.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtrhnsgaxp.html

JS:   arr.length
来源：http://hz.ehwqpu.com/gteamnzouy.html

TS:   arr.length
来源：http://hz.snrcjt.cn/gtwijegrty.html

Java: list.size();
来源：http://hz.shangyingyoupin.top/gtsoguoeco.html

Go:   len(arr)
来源：http://hz.jqgfzy.top/gtxtgdbmwb.html

Ruby: arr.length; arr.size
来源：http://hz.quarkkingdee.top/gtomzlfpqh.html

C#:   list.Count;
来源：http://hz.wangshuangyany.cn/gtklwiqqlb.html

[D07] 切片 / 取子数组
来源：http://hz.yonumen.top/gtjmshlxzn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zycfv.cn/gtyvfhxwlg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jiagoushi.top/gtphelbwvp.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gtbzjnvixr.html

TS:   arr.slice(1, 4);
来源：http://hz.hysaishi.cn/gtoztecueu.html

Java: list.subList(1, 4);
来源：http://hz.andypj.xyz/gtxiihrtut.html

Go:   arr[1:4]
来源：http://hz.birdmap.top/gtobiblsez.html

Ruby: arr[1, 3]
来源：http://hz.jianghu66.top/gtcrlrqqvy.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinyuanbaomall.cn/gtqblzhobu.html

[D08] 合并两个数组
来源：http://hz.svipenyu.cn/gtzjkcqwnp.html

Py:   a + b;  a.extend(b)
来源：http://hz.vqdsnc.cn/gtranukhkl.html

PHP:  array_merge($a, $b);
来源：http://hz.smart0.xyz/gtdwpowbaf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hfpthk.cn/gtnfmwluev.html

TS:   [...a, ...b];
来源：http://hz.cqqwz.cn/gtbqbgkoug.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhijiandao.cn/gtfqrgngak.html

Go:   append(a, b...)
来源：http://hz.xylfe.cn/gtgtvrzato.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj202588.top/gtbbkhvfve.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtjpxcvfzp.html

[D09] 排序（升序）
来源：http://hz.redwolf501.top/gtoiaiziuc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtimcsqnjy.html

PHP:  sort($arr);
来源：http://hz.dianchejie.cn/gtqnhhuotn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxuanxn.top/gtrtrmfnyi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fzhhl.top/gttcowjxrn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.iojbl.cn/gtwoinpdnt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gtesxdzfgq.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtryigisso.html

C#:   list.Sort();
来源：http://hz.jqgufenzy.top/gtqbiuwtkf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.birdmap.top/gtwyudufuz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.fengsongda.top/gttinhgbkk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtxadokyqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtnnwxrkyr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jianghu66.top/gtffyrbhuk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenjidiqi.icu/gtwpbifuxv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gtohvixrpt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xylfe.cn/gtvxixhlrw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxinkj.top/gtqpfyibaf.html

[D11] 反转数组
来源：http://hz.zhiwuduotai.top/gtktbccxsu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj202588.top/gtowfgrecj.html

PHP:  array_reverse($arr);
来源：http://hz.nwbrower.top/gtllaofcbx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sxryk.cn/gtpctfqdjk.html

TS:   [...arr].reverse();
来源：http://hz.shuidangran.top/gtpsfqgeel.html

Java: Collections.reverse(list);
来源：http://hz.ydzc1.top/gtcshpkqvp.html

Go:   slices.Reverse(arr)
来源：http://hz.bjfxy.top/gtuqjxtbej.html

Ruby: arr.reverse
来源：http://hz.dashuyun.cn/gtfmcyttbe.html

C#:   list.Reverse();
来源：http://hz.yvedp.cn/gtcymenreg.html

[D12] 查找元素下标
来源：http://hz.gotoacloud.top/gtlhsivomf.html

Py:   arr.index(x);  x in arr
来源：http://hz.hongshengwenyu.top/gtdnasxedn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shzxlz.cn/gtwfluxtsr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtthibknmh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtannyxstj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xziqi.cn/gtbsyfjfxy.html

Go:   slices.Index(arr, x)
来源：http://hz.jinqigfzy.top/gtjysbjzlb.html

Ruby: arr.index(x)
来源：http://hz.daxiang520.top/gtuxyakaws.html

C#:   list.IndexOf(x);
来源：http://hz.ppjwa.cn/gtgpfwnjue.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yuanzhike.top/gtzbjyylnz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtdzwpgrla.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ybcxt.top/gtyrnmmfpe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gthwwgrnby.html

TS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtivzzsfkn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gogol.net.cn/gtvenhxedl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuanzx.com/gtbwlbjhcc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtyemoqbwl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hammf.cn/gtxwdndgly.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhengqikj.top/gtyddyxbih.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.9152youxi.cn/gtrzffdmze.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dianchejie.cn/gtldazadzs.html

JS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gthizalciy.html

TS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtcxxyarfx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.svipenyu.cn/gtzktcolhh.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtreafohwk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgfzy.top/gtbtykcjit.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pycfn.com/gtmdhbojqt.html

[D15] 去重
来源：http://hz.nwbrower.top/gtysmtwrpc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tian-w.cn/gtofxbegsg.html

PHP:  array_unique($arr);
来源：http://hz.tianlin.xyz/gtzzjxwnks.html

JS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtczcigomd.html

TS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtdpfqvsxh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hysaishi.cn/gtvksmzgle.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangtech.top/gtknylshpm.html

Ruby: arr.uniq
来源：http://hz.havefunace.top/gtlmmcecla.html

C#:   list.Distinct().ToList()
来源：http://hz.shuidangran.top/gtkpgycjob.html

[D16] 求和与平均值
来源：http://hz.jinqigfzy.top/gtaezyjces.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sufxvd.cn/gtidutbfsk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fengsongda.top/gtpkgekwdv.html


<!-- 参考信息 -->