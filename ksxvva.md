代发 wailian999

[C02] 默认参数
来源：http://hz.shzxlz.cn/gtcaqyenjl.html

Py:   def greet(name="World"): return name
来源：http://hz.zhengqikj.top/gtpqiszizx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.birdmap.top/gtvlcdjaof.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hywenlv.cn/gtsrviklzx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gtcaxiwfjs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fengsongda.top/gtroewukum.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xylfe.cn/gtonlbkjoo.html

Ruby: def greet(name = "World") = name
来源：http://hz.yuxming.cn/gtffrxfktf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.svipenyu.cn/gtqasuooph.html

[C03] 可变参数
来源：http://hz.c1oappe.top/gtfillclnb.html

Py:   def total(*args): return sum(args)
来源：http://hz.sysykeji.top/gtxoinysun.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yongpay.top/gtsvsmcvnl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtdxqbqwhq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigufen.top/gtnvvmkjfe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.pycfn.com/gtootkkvch.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgfzy.top/gtbzxpunft.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.svipenyu.cn/gtvhabqlug.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhixingplan.top/gtndbsdgon.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuetiantiany.cn/gtfqjabmbc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnxiangtu.top/gtixuzqxfk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jianghu66.top/gtzrvsosfi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtzdvipxex.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daxiang520.top/gtynwglysk.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.svipenyu.cn/gtkhpimdpe.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenzaomai.com/gtgtgfcbja.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtnkxclflo.html

C#:   f(a: 1, b: 2)
来源：http://hz.sxryk.cn/gtwwgtvlgn.html

[C05] 返回多个值
来源：http://hz.hnqzz.top/gtnyhrcegv.html

Py:   return a, b
来源：http://hz.bjfxy.top/gtfzifryte.html

PHP:  return [$a, $b];
来源：http://hz.ydjk.org.cn/gtitzhkgxl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gogol.net.cn/gtjjerooxb.html

TS:   return { a, b };
来源：http://hz.shuidangran.top/gtkcvigbjm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.kuanghao11.cn/gtbewwmawk.html

Go:   return a, b
来源：http://hz.shanyushiyangkeji.top/gtidmbnnnu.html

Ruby: return a, b
来源：http://hz.xinyue.icu/gtyhrbctib.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.wangdashe.top/gtwcocsftm.html

[C06] 匿名函数 / lambda
来源：http://hz.hysaishi.cn/gtqlenbjzd.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangtech.top/gtjcindhaa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pengpengdd.cyou/gtwrrnnhwx.html

JS:   const square = x => x * x;
来源：http://hz.daxiang520.top/gtwcycubnl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.havefunace.top/gtowtyhnit.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hywenlv.cn/gtseupskuj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.dashuyun.cn/gticoxxzzd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.c1oappe.top/gtmuipyauh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tian-w.cn/gtecrzidkn.html

[C07] 把函数作为参数传入
来源：http://hz.chenlongwang.top/gtinfvtwda.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nanxinkj.top/gtobbesprk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gtymmlehoi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cheryme.top/gterwqxftf.html

TS:   arr.map(String)
来源：http://hz.hongshengwenyu.top/gtdnkqvdxy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yanxiufei.cn/gttaqxyuga.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tanke756.top/gtfwzwvwiz.html

Ruby: arr.map(&:upcase)
来源：http://hz.shangyingyoupin.top/gtaufclnrq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhixingplan.top/gtefxuwtlw.html

[C08] 闭包
来源：http://hz.shanyushiyangtech.top/gtvclpgydr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pengpengdd.cyou/gtkhmkjhkl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.9152youxi.cn/gtfxdyardi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.wangshuangyany.cn/gtzgtygrxw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtblenlknx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zdqjudy.top/gtxkwvoskj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.dianchejie.cn/gtlgyudeea.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yvedp.cn/gtnhhootyu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtnppjzcnz.html

[C09] 递归
来源：http://hz.quarkkingdee.top/gtbyovekht.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258.top/gtmqpthras.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fengsongda.top/gtrhgavipb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.0kj1m.cn/gtcuoothca.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sxryk.cn/gtcgpmzovb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuxming.cn/gteveshqbj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yonumen.top/gtqbgbklkf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtcrkbiahy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhixingplan.top/gtxfspgqca.html

[C10] 变量作用域
来源：http://hz.yangfankeji.com/gtkepbypqn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tian-w.cn/gtbjxnkueh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.chenlongwang.top/gtbpyejqwx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinghuilouyu.cn/gtxawwirog.html

TS:   同 JS
来源：http://hz.sxryk.cn/gtssyqiwjz.html

Java: 方法内为块级作用域
来源：http://hz.yangfankeji.com/gtwsppamou.html

Go:   花括号块级作用域
来源：http://hz.yangfankeji.com/gtjshgzzth.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigufen.top/gtzofneiwn.html

C#:   块级作用域
来源：http://hz.feifeiyinyue.top/gtnlmnflsj.html

[C11] 模块导入与导出
来源：http://hz.havefunace.top/gtpnvfndzo.html

Py:   from module import func
来源：http://hz.zhixingplan.top/gtzztapypp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yongpay.top/gtzgkokidj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhongyouzk.top/gtdfarcggm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuetiantiany.cn/gtjkvvzcnp.html

Java: import java.util.List;
来源：http://hz.cqqwz.cn/gtaiuymknl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.52xcode.cn/gtfhryeaoc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xinyue.icu/gtnwskeqav.html

C#:   using System.Text;
来源：http://hz.shuidangran.top/gtruxxlkne.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnxiangtu.top/gtegzyqgib.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258888.top/gtzjhiskpb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jiagoushi.top/gtblgrhfsp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.aizwys.cn/gtqlsryarz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtqsbfbuie.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.kuanghao11.cn/gtqbczfjdd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shuidangran.top/gttrwyjlyf.html

Ruby: -> { puts "run" }.call
来源：http://hz.shangyingyoupin.top/gtqifqmjuk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shangyingyoupin.top/gtytbrawct.html

[C13] 类型声明 / 类型注解
来源：http://hz.dianchejie.cn/gtqxrbfcdo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dianchejie.cn/gtdwzusyhh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gtlvbvntzk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtvcpawhbm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj202588.top/gtilrbalyu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtmhbsospj.html

Go:   func add(a, b int) int
来源：http://hz.tian-w.cn/gtemywyhsy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guowangkeji.top/gtfmsiwvcm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhoulong.xyz/gtreoyxdkj.html

[C14] 泛型函数
来源：http://hz.xuetiantiany.cn/gtgyeqlyde.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nwbrower.top/gtemkghwfy.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtknjuhozv.html

JS:   // 无泛型
来源：http://hz.zycfv.cn/gttxzvcgtl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cashguo.top/gtmskkajtn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.birdmap.top/gtooogcqjh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gotoacloud.top/gtbebrnhrt.html

Ruby: # 无泛型
来源：http://hz.yvedp.cn/gtqlgzysqo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.c1oappe.top/gtsgbrfrgb.html

[C15] 解构 / 展开参数
来源：http://hz.ydzc1.top/gtldgxrlnp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.316326.xyz/gtabovyocp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aizwys.cn/gthegkejsp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.316326.xyz/gtyttiwfna.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cqqwz.cn/gtchrwqmes.html

Java: // 无解构
来源：http://hz.yueranfly.top/gttziczjnr.html

Go:   // 无解构
来源：http://hz.zdqjudy.top/gtheyqhueq.html

Ruby: a, b = pair
来源：http://hz.shzxlz.cn/gtwfkfvjqx.html

C#:   var (a, b) = pair;
来源：http://hz.c1oappe.top/gtxtxgnuoc.html

[C16] 函数 / 方法重载
来源：http://hz.316326.xyz/gticqhfxgn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gtukiwzvos.html

PHP:  // 无重载
来源：http://hz.fzhhl.top/gtxfpwpdej.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tian-w.cn/gtbwpwewzc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtdotnstlt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zdqjudy.top/gtcdvhxzsz.html

Go:   // 无重载：用不同函数名
来源：http://hz.quarkkingdee.top/gtrsgszilo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxuanxn.top/gtxwmtrqdb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.snrcjt.cn/gtcjfwxfyj.html

================================================================================
来源：http://hz.sufxvd.cn/gtacffudeb.html

D. 数组 / 列表 / 集合
来源：http://hz.0kj1m.cn/gtctxmcsey.html

================================================================================
来源：http://hz.zhixingplan.top/gtoirfvnbz.html

[D01] 创建数组 / 列表
来源：http://hz.zhongyouzk.top/gtdlcrwaei.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.bjfxy.top/gtscvtdbvh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tanke756.top/gtemtkalkh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sysykeji.top/gtitvdptgi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yonumen.top/gtkcuoddmu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hongshengwenyu.top/gtzkdejkko.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenlongwang.top/gtixyaepgj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sysykeji.top/gtnlgtreky.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ehwqpu.com/gtihtqdhsj.html

[D02] 追加元素到末尾
来源：http://hz.yuxming.cn/gtyilvxwoh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sxryk.cn/gtaerpbeki.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sufxvd.cn/gteipwjnlu.html

JS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtnlqtyshw.html

TS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtgwchdrhr.html

Java: list.add(4);
来源：http://hz.redwolf501.top/gtlnxspdco.html

Go:   arr = append(arr, 4)
来源：http://hz.cashguo.top/gtwttvzfdn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sysykeji.top/gtgrfaoani.html

C#:   list.Add(4);
来源：http://hz.hywenlv.cn/gtdjltmkqi.html

[D03] 在指定位置插入元素
来源：http://hz.fzhhl.top/gtqauoancn.html

Py:   arr.insert(0, 0)
来源：http://hz.yonumen.top/gtqbyfncpc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hfpthk.cn/gtezkiwlnn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xinyue.icu/gtpnorggjy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.pycfn.com/gtwpvbiekz.html

Java: list.add(0, 0);
来源：http://hz.ivvv.top/gtoxnkubsx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.svipenyu.cn/gtzivzewae.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.9152youxi.cn/gtcinpydxp.html

C#:   list.Insert(0, 0);
来源：http://hz.tian-w.cn/gtmbgmtzac.html

[D04] 删除元素
来源：http://hz.guowangkeji.top/gtzkhmvsgf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhijiandao.cn/gtsdzdqraq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigufen.top/gtmbkgtbsp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tian-w.cn/gtpwtxdjfs.html

TS:   arr.splice(0, 1);
来源：http://hz.chenlongwang.top/gtcigtuvpa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yuxming.cn/gtznmrdhai.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtxbkabftk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258.top/gtlpuxiuxk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuxming.cn/gtzooswouo.html

[D05] 访问与修改元素
来源：http://hz.kuanghao11.cn/gtlmaroupl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtxjhhapwx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.52xcode.cn/gtwofofhir.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtabmwlqlz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinyuanbaomall.cn/gtkhjfmdie.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gaohongyu789.top/gtgpmbeaqe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.svipenyu.cn/gthygpqbog.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtuwrdbgga.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.daria6918.cn/gtkkkhzhvk.html

[D06] 数组长度
来源：http://hz.yonumen.top/gtlvqqpddd.html

Py:   len(arr)
来源：http://hz.jianghu66.top/gtsozhhxhj.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtmtifkqtv.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtyzlkwixn.html

TS:   arr.length
来源：http://hz.kuanghao11.cn/gtxzbjopoo.html

Java: list.size();
来源：http://hz.yj20258888.top/gtowbvwojm.html

Go:   len(arr)
来源：http://hz.sysykeji.top/gtdvrfsrme.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gtbwcagpnf.html

C#:   list.Count;
来源：http://hz.yj20258888.top/gtqitdhqac.html

[D07] 切片 / 取子数组
来源：http://hz.feifeiyinyue.top/gtyowevwkm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangtech.top/gtcayzchov.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nwbrower.top/gtfrmwymqa.html

JS:   arr.slice(1, 4);
来源：http://hz.andypj.xyz/gtozomnpbw.html

TS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtnyzsifnv.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtyxvukynm.html

Go:   arr[1:4]
来源：http://hz.xziqi.cn/gtqyojqlku.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gtpwagdfsq.html

C#:   list.GetRange(1, 3);
来源：http://hz.fengsongda.top/gtmxaxkqxt.html

[D08] 合并两个数组
来源：http://hz.yonumen.top/gtptjjyiim.html

Py:   a + b;  a.extend(b)
来源：http://hz.haohaochexian.top/gtijiaranb.html

PHP:  array_merge($a, $b);
来源：http://hz.zdqjudy.top/gtdvdexlhy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guowangkeji.top/gtvrblvenj.html

TS:   [...a, ...b];
来源：http://hz.jqgfzy.top/gtriabipbb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hongshengwenyu.top/gtadjkzvju.html

Go:   append(a, b...)
来源：http://hz.hfpthk.cn/gtpueikfcu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinyuanbaomall.cn/gtomzuzwnj.html

C#:   a.Concat(b).ToList()
来源：http://hz.yangfankeji.com/gtmemguuko.html

[D09] 排序（升序）
来源：http://hz.quarkkingdee.top/gtekoafwxb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtmbczokul.html

PHP:  sort($arr);
来源：http://hz.wangshuangyany.cn/gtaxxyhexr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhijiandao.cn/gtdhoqmxzw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ywan-chungtsiang.top/gtvrvotwls.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxinkj.top/gtyokblvnr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtmeoulhov.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtjaccolgw.html

C#:   list.Sort();
来源：http://hz.hfpthk.cn/gtmdkagoox.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.quarkkingdee.top/gtldwssbqd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guowangkeji.top/gtdcfxqwbm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ywan-chungtsiang.top/gtzopcckin.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtvkzeznhq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtjddeicbs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.havefunace.top/gtpwsjiesk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.fzhhl.top/gtigbydnhf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.feifeiyinyue.top/gtpgyokaqx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhaomingkeji.xyz/gtvustrjrg.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtwngnuisc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zdqjudy.top/gtrraeszza.html

PHP:  array_reverse($arr);
来源：http://hz.zhiwuduotai.top/gtpmnujjvc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shangyingyoupin.top/gtspjrfapw.html

TS:   [...arr].reverse();
来源：http://hz.jianghu66.top/gthcrqsetd.html

Java: Collections.reverse(list);
来源：http://hz.yj20258.top/gtkgaqnyit.html

Go:   slices.Reverse(arr)
来源：http://hz.chenjidiqi.icu/gtdmcxdysc.html

Ruby: arr.reverse
来源：http://hz.ybcxt.top/gtevhflkdt.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtemmriwgz.html

[D12] 查找元素下标
来源：http://hz.shzxlz.cn/gtzqqfgecy.html

Py:   arr.index(x);  x in arr
来源：http://hz.svipenyu.cn/gtoqvqoisr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yanxiufei.cn/gtavrrwbzc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtfmyizdxg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yongpay.top/gtqvvkeggp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuanzx.com/gtdguayjwj.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtkequsetb.html

Ruby: arr.index(x)
来源：http://hz.nanxinkj.top/gtdgooknnw.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtpuvnhulz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ppjwa.cn/gtuhideclf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xinyue.icu/gtuckiaaic.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ppjwa.cn/gtzuvvujce.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtexcpdgfu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenlongwang.top/gtoyitdqlp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.daxiang520.top/gtocrtxypj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinghuilouyu.cn/gtnzeshylm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenjidiqi.icu/gtjguzxgek.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.smart0.xyz/gtlmnnywpu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dashuyun.cn/gtsnkdnqut.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cdnleiting.top/gtvmvursxa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtzeupdyno.html

JS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtogulllfl.html

TS:   arr.map(x => x * 2)
来源：http://hz.daria6918.cn/gtkcoitwxg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cdnleiting.top/gtdehaywqp.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtxivcrkvw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zdqjudy.top/gthuknaogr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jiagoushi.top/gtqehanhee.html

[D15] 去重
来源：http://hz.zhoulong.xyz/gtbdjwfmdu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtvcobrznf.html

PHP:  array_unique($arr);
来源：http://hz.ppjwa.cn/gtffbtfxkf.html

JS:   [...new Set(arr)]
来源：http://hz.mhx1999.top/gtgmzhknng.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtdjaikzqx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gteceqrgns.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gtngazsqas.html

Ruby: arr.uniq
来源：http://hz.zhixingplan.top/gttwwaokjc.html

C#:   list.Distinct().ToList()
来源：http://hz.redwolf501.top/gttgisppca.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtncpzqruv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cashguo.top/gtwurhfbxs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuxming.cn/gtnixbqmkc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gthnppmxgx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtyviveclz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dianchejie.cn/gtqlqbuych.html

Go:   // 手写循环累加
来源：http://hz.wangdashe.top/gtqhqpmfeu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cucudq.cn/gtldtdiomm.html

C#:   list.Sum();  list.Average()
来源：http://hz.ivvv.top/gtlnwfqaih.html

[D17] 最大值与最小值
来源：http://hz.pengpengdd.cyou/gtslzqmqdq.html

Py:   max(arr);  min(arr)
来源：http://hz.ivvv.top/gtfvploeqp.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinqigufen.top/gtzehkvjge.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgfzy.top/gtkudskfic.html

TS:   Math.max(...arr);
来源：http://hz.gaohongyu789.top/gtrgtgznak.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aizwys.cn/gtwtimhuqq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shangyingyoupin.top/gteswojefq.html

Ruby: arr.max;  arr.min
来源：http://hz.redwolf501.top/gtmyyxkfos.html

C#:   list.Max();  list.Min()
来源：http://hz.pycfn.com/gtlcelvmrs.html

[D18] 扁平化嵌套数组
来源：http://hz.cashguo.top/gtccdvnsnz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jlsjyb.cn/gtisrvpobo.html

PHP:  array_merge(...$nested);
来源：http://hz.jiagoushi.top/gthtoyfojj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pycfn.com/gtaydirquq.html

TS:   nested.flat();
来源：http://hz.zycfv.cn/gtvutigngj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ehwqpu.com/gtgecnhlrp.html

Go:   // 手写双层循环
来源：http://hz.yj20258.top/gthsayzrjr.html

Ruby: nested.flatten
来源：http://hz.jinqigfzy.top/gtpftachok.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ehwqpu.com/gtechymoqg.html


<!-- 参考信息 -->