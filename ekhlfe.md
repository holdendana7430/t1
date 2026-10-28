代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtrqmtltes.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hywenlv.cn/gtcigpsdiq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.havefunace.top/gtghmwfyfr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gthkrutnoz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuanzhike.top/gtvqngsqnv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dianchejie.cn/gtbgewveao.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuanzx.com/gtljovytpy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zycfv.cn/gtuiyrtgeg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jianghu66.top/gtkhbehtjw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtboeilrrj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ywan-chungtsiang.top/gtioyttini.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gogol.net.cn/gtvndtjxav.html

Go:   // 无：用配置结构体参数
来源：http://hz.guowangkeji.top/gtbjwqmynd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtdiseqcux.html

C#:   f(a: 1, b: 2)
来源：http://hz.gogol.net.cn/gtvqpjnfpe.html

[C05] 返回多个值
来源：http://hz.birdmap.top/gtvzmtmpkv.html

Py:   return a, b
来源：http://hz.bjfxy.top/gtyndqrjrr.html

PHP:  return [$a, $b];
来源：http://hz.gotoacloud.top/gtxweqohvv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sxryk.cn/gtmdpcmraj.html

TS:   return { a, b };
来源：http://hz.fzhhl.top/gtqagqkzvn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cqqwz.cn/gtaadbybhr.html

Go:   return a, b
来源：http://hz.tianlin.xyz/gtgfodbzxe.html

Ruby: return a, b
来源：http://hz.gotoacloud.top/gtujbydxlr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigfzy.top/gtxlbkfyov.html

[C06] 匿名函数 / lambda
来源：http://hz.kuanghao11.cn/gtfydojynb.html

Py:   square = lambda x: x * x
来源：http://hz.pengpengdd.cyou/gtmvdayhrw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.52xcode.cn/gtajkpwryu.html

JS:   const square = x => x * x;
来源：http://hz.sweek.top/gtniheicmy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhixingplan.top/gtaokxjtpi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ywan-chungtsiang.top/gtqwvbvxwc.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinqigfzy.top/gtxjslxvvv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangkeji.top/gtlktwqoka.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxuanxn.top/gtctkvsupb.html

[C07] 把函数作为参数传入
来源：http://hz.quarkkingdee.top/gtpspguhss.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hysaishi.cn/gtlquakcon.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shangyingyoupin.top/gtlkpwpmzw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jiagoushi.top/gtgrdsvnqt.html

TS:   arr.map(String)
来源：http://hz.cqqwz.cn/gtqalqshgo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.mhx1999.top/gtrkjspdus.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cdnleiting.top/gtwmlejdpg.html

Ruby: arr.map(&:upcase)
来源：http://hz.gzhubu.top/gtekwebsoe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.tian-w.cn/gtjdorfluc.html

[C08] 闭包
来源：http://hz.cheryme.top/gtlhccouwk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.0kj1m.cn/gtinnggmga.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigufen.top/gttborzpyg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtagivuith.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtdxoytcym.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yangfankeji.com/gtsyiiqput.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.9152youxi.cn/gtzsaxnjid.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.nanxuanxn.top/gthgmvyewx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtjvwcoimz.html

[C09] 递归
来源：http://hz.aizwys.cn/gtkxxgqtuh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aizwys.cn/gtihcslrjz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aibaodan.cn/gtxwznsmyt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtzxjafomm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtaqienmct.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cheryme.top/gtwctjcdbu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aizwys.cn/gtmidgmjyo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zycfv.cn/gtbzqqiybn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jyoumei.cn/gtkyygjtid.html

[C10] 变量作用域
来源：http://hz.havefunace.top/gteidvuqmb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.c1oappe.top/gtsfpxozdp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hywenlv.cn/gtxhvdzapm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jiagoushi.top/gtfajfdckg.html

TS:   同 JS
来源：http://hz.yueranfly.top/gtzsjlbxft.html

Java: 方法内为块级作用域
来源：http://hz.yuanzhike.top/gthjzpbumg.html

Go:   花括号块级作用域
来源：http://hz.birdmap.top/gtwcjarezc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hysaishi.cn/gtcrcagzzk.html

C#:   块级作用域
来源：http://hz.xziqi.cn/gtivkwlixc.html

[C11] 模块导入与导出
来源：http://hz.jlsjyb.cn/gtafxjindv.html

Py:   from module import func
来源：http://hz.vqdsnc.cn/gtkbqrxkcm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhijiandao.cn/gtwxhnrnpe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cucudq.cn/gtjjsefmio.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jiagoushi.top/gtblqyxuxm.html

Java: import java.util.List;
来源：http://hz.nanxinkj.top/gtjhfhxljp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.vqdsnc.cn/gtwlkrkoxu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuetiantiany.cn/gtlheuiwkv.html

C#:   using System.Text;
来源：http://hz.xingfuxueyuan.xyz/gtjjyfmvua.html

[C12] 立即执行函数 IIFE
来源：http://hz.cheryme.top/gtodsizxmg.html

Py:   (lambda: print("run"))()
来源：http://hz.zdqjudy.top/gtpnhkwzod.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtzbnqflln.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtruzupscw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gthnihnxzy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenlongwang.top/gtgpahpkwz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.0kj1m.cn/gtuclxuxuv.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gtzbenjwxw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtnwlelyoe.html

[C13] 类型声明 / 类型注解
来源：http://hz.52xcode.cn/gtsbjlufyx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ywan-chungtsiang.top/gtzgxgmnfs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxuanxn.top/gtmvnwslee.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shangyingyoupin.top/gtzrwptbao.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtyqgjqcsy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtmdmhjuoy.html

Go:   func add(a, b int) int
来源：http://hz.xuetiantiany.cn/gtqxdkiojy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ppjwa.cn/gtwfdvefip.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pengpengdd.cyou/gtfmtgqfjc.html

[C14] 泛型函数
来源：http://hz.yj20258888.top/gttpafkwqs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gttxrtfgca.html

PHP:  // 无泛型
来源：http://hz.jinyuanbaomall.cn/gtjlvxfova.html

JS:   // 无泛型
来源：http://hz.0kj1m.cn/gtvjbknima.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shangyingyoupin.top/gtxzbjgbtt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cheryme.top/gtfqhgutei.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xuanzx.com/gtjdpvqnmz.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangkeji.top/gtqeawjfqi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.snrcjt.cn/gtgevulffw.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gtibbiirkz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cashguo.top/gtwyxyfero.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenzaomai.com/gtmswicuej.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtxhjpquvk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gaohongyu789.top/gtkggnvmoe.html

Java: // 无解构
来源：http://hz.zhiwuduotai.top/gtxtkrzpub.html

Go:   // 无解构
来源：http://hz.yj20258.top/gtqpssgoro.html

Ruby: a, b = pair
来源：http://hz.havefunace.top/gtaoggavce.html

C#:   var (a, b) = pair;
来源：http://hz.9152youxi.cn/gthjgvuwhd.html

[C16] 函数 / 方法重载
来源：http://hz.snrcjt.cn/gtvjtvqwwu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xuetiantiany.cn/gteulubuef.html

PHP:  // 无重载
来源：http://hz.cashguo.top/gttkoljdwg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenzaomai.com/gtgrmkslbe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.52xcode.cn/gttcvwuemi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenzaomai.com/gtgnghvczt.html

Go:   // 无重载：用不同函数名
来源：http://hz.yangfankeji.com/gtejakdxvt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pengpengdd.cyou/gtnqjzgugx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hywenlv.cn/gtfzxgfieo.html

================================================================================
来源：http://hz.hywenlv.cn/gtquhxolvt.html

D. 数组 / 列表 / 集合
来源：http://hz.sysykeji.top/gtsfsgbwtr.html

================================================================================
来源：http://hz.meibo888.top/gtrurhlfsy.html

[D01] 创建数组 / 列表
来源：http://hz.haohaochexian.top/gtqtdqgzra.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.kuanghao11.cn/gtdimjvkis.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhijiandao.cn/gtuaezyhsg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xinyue.icu/gtbecrzgrt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.haohaochexian.top/gtlgldwzwg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jyoumei.cn/gtrxgpriba.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cucudq.cn/gttuglxvzf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xinyue.icu/gtekyipzlh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gtvtgqmgoj.html

[D02] 追加元素到末尾
来源：http://hz.chenzaomai.com/gtpfbmhoea.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtkyeirozi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.mhx1999.top/gtnkivzqof.html

JS:   arr.push(4);
来源：http://hz.jinqigufen.top/gtmkhlwkyg.html

TS:   arr.push(4);
来源：http://hz.daxiang520.top/gtkptoqnff.html

Java: list.add(4);
来源：http://hz.nwbrower.top/gtrprliail.html

Go:   arr = append(arr, 4)
来源：http://hz.mhx1999.top/gtznfylzmt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.mhx1999.top/gthlhvculv.html

C#:   list.Add(4);
来源：http://hz.jianghu66.top/gtwrcpnxis.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtqhymcwmx.html

Py:   arr.insert(0, 0)
来源：http://hz.quarkkingdee.top/gthzwboyib.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhengqikj.top/gtzmklzxzf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sxryk.cn/gtpoprhqen.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenjidiqi.icu/gtpmgobvhq.html

Java: list.add(0, 0);
来源：http://hz.c1oappe.top/gtuagzllil.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hammf.cn/gtnlxtgmfb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhaomingkeji.xyz/gtxnetxgzu.html

C#:   list.Insert(0, 0);
来源：http://hz.andypj.xyz/gtrrhttkwj.html

[D04] 删除元素
来源：http://hz.yangfankeji.com/gtaseytaxt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jianghu66.top/gtbpuypdiy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.havefunace.top/gtpctiszwx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.havefunace.top/gtmgdjfbyb.html

TS:   arr.splice(0, 1);
来源：http://hz.zhongyouzk.top/gtcsgfftgm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gzhubu.top/gtdfzvlkqm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtoejnjfey.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dashuyun.cn/gthfdsojqs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jiagoushi.top/gtjnbxvvra.html

[D05] 访问与修改元素
来源：http://hz.zdqjudy.top/gtreyhjhgp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtvubflvjb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.316326.xyz/gtrpoygoak.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.mhx1999.top/gthvzxmggo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cheryme.top/gtjyaxnvvc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.mhx1999.top/gtyjmrwdbp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtlzrbjgpe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtbsuuygsg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ybcxt.top/gtaexjfcjs.html

[D06] 数组长度
来源：http://hz.yj20258.top/gtygodgjmj.html

Py:   len(arr)
来源：http://hz.fengsongda.top/gtmqrhrvjn.html

PHP:  count($arr);
来源：http://hz.chenlongwang.top/gtzzdokgvw.html

JS:   arr.length
来源：http://hz.nanxinkj.top/gthrzadrdh.html

TS:   arr.length
来源：http://hz.bjfxy.top/gtyghjqafl.html

Java: list.size();
来源：http://hz.316326.xyz/gtrirajxik.html

Go:   len(arr)
来源：http://hz.feifeiyinyue.top/gtkbbqbiue.html

Ruby: arr.length; arr.size
来源：http://hz.c1oappe.top/gtsnfqcmkx.html

C#:   list.Count;
来源：http://hz.yanxiufei.cn/gtoedbhubz.html

[D07] 切片 / 取子数组
来源：http://hz.c1oappe.top/gtvfsasior.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sysykeji.top/gtqqptspit.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhijiandao.cn/gtoezqwxqp.html

JS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtpmgytnbv.html

TS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gtbzqqtwog.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtiabghjoj.html

Go:   arr[1:4]
来源：http://hz.daxiang520.top/gtvihihrbr.html

Ruby: arr[1, 3]
来源：http://hz.gzhubu.top/gtvtamfgrz.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydzc1.top/gthjzwdxgl.html

[D08] 合并两个数组
来源：http://hz.shangyingyoupin.top/gtlfzffzny.html

Py:   a + b;  a.extend(b)
来源：http://hz.yvedp.cn/gticxnrpcd.html

PHP:  array_merge($a, $b);
来源：http://hz.birdmap.top/gtjvngymfw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtvunmrutw.html

TS:   [...a, ...b];
来源：http://hz.gogol.net.cn/gtfbesetjk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenzaomai.com/gtqsbvipwc.html

Go:   append(a, b...)
来源：http://hz.havefunace.top/gtoykibzbo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.iojbl.cn/gtjzznwqnv.html

C#:   a.Concat(b).ToList()
来源：http://hz.gotoacloud.top/gtbqkbhxey.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtnzsgwtyy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gtbqygjpgk.html

PHP:  sort($arr);
来源：http://hz.hnxiangtu.top/gtlfyfghez.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jlsjyb.cn/gtvbekfywb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hfpthk.cn/gtsuhzaosg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gzhubu.top/gteawqrhon.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cheryme.top/gtncudoncs.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtddtvobcs.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gtmrnbzpre.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yangfankeji.com/gtecygfxku.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.vqdsnc.cn/gthsgbdyae.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hywenlv.cn/gtsdfxflzj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtnkmzwmmh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gtszupsphu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangkeji.top/gtjxugxlmm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.smart0.xyz/gtkwrmokrz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shzxlz.cn/gtmapkaavb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sxryk.cn/gtpvkbdxwz.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtwdiagsti.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tanke756.top/gtciznoqfh.html

PHP:  array_reverse($arr);
来源：http://hz.zdqjudy.top/gtvwduyzup.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jiagoushi.top/gtalbhpwzq.html

TS:   [...arr].reverse();
来源：http://hz.dashuyun.cn/gtclqyehzy.html

Java: Collections.reverse(list);
来源：http://hz.jlsjyb.cn/gtxarxsclw.html

Go:   slices.Reverse(arr)
来源：http://hz.hysaishi.cn/gtsyqtzmvs.html

Ruby: arr.reverse
来源：http://hz.gaohongyu789.top/gtvpkuprcn.html

C#:   list.Reverse();
来源：http://hz.yangfankeji.com/gtlfuqoowl.html

[D12] 查找元素下标
来源：http://hz.xingfuxueyuan.xyz/gtfvfohvhq.html

Py:   arr.index(x);  x in arr
来源：http://hz.ppjwa.cn/gtyyqgikxa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ybcxt.top/gttxzciwbm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gtvlaaluxk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtbhpkowtf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj202588.top/gtnwwzuiug.html

Go:   slices.Index(arr, x)
来源：http://hz.xziqi.cn/gtsenrdwvz.html

Ruby: arr.index(x)
来源：http://hz.hfpthk.cn/gtacmxjxef.html

C#:   list.IndexOf(x);
来源：http://hz.yuxming.cn/gtogihhosa.html

[D13] 过滤（保留满足条件的）
来源：http://hz.birdmap.top/gttdzejoeh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jlsjyb.cn/gtndzlflmh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.pycfn.com/gtquqdcxwv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtkitkiysv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gttwiirevg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258888.top/gtpcnvtuhi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gaohongyu789.top/gtsbajmsps.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yueranfly.top/gtzfkhqnoc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.svipenyu.cn/gtmunpuhza.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pycfn.com/gtjrblwlwe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gtcxwdbvcx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jlsjyb.cn/gtdwlwiryf.html

JS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtxverwqys.html

TS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtseyfquhu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yuxming.cn/gtgifbjczk.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gtzaljwevp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.andypj.xyz/gtizxiekeh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yanxiufei.cn/gthnxshaxe.html

[D15] 去重
来源：http://hz.zhiwuduotai.top/gtcdntbcmb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtknphxvvt.html

PHP:  array_unique($arr);
来源：http://hz.sysykeji.top/gtazdwdtiv.html

JS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gterhmpmub.html

TS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtbcedzfrc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fengsongda.top/gtczvcacbr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhongyouzk.top/gtaqgfaksc.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtinhhudgf.html

C#:   list.Distinct().ToList()
来源：http://hz.zhiwuduotai.top/gthogfmsks.html

[D16] 求和与平均值
来源：http://hz.hfpthk.cn/gtixrieama.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinyuanbaomall.cn/gtjtlsjmmj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hnxiangtu.top/gtxodbodrj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtldbfsnwb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sweek.top/gtwzwnalrn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtsqjpgpkr.html

Go:   // 手写循环累加
来源：http://hz.zhixingplan.top/gtxzzudufe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gtzvziedoi.html

C#:   list.Sum();  list.Average()
来源：http://hz.jiagoushi.top/gtwwxleico.html

[D17] 最大值与最小值
来源：http://hz.ydjk.org.cn/gtrfyqqvmw.html

Py:   max(arr);  min(arr)
来源：http://hz.yj20258888.top/gtrqouipvd.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258.top/gtmpawyatl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cheryme.top/gtlgrqmgcq.html

TS:   Math.max(...arr);
来源：http://hz.tianlin.xyz/gtdvjcgpeg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aizwys.cn/gtumpapcir.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guannengcc.top/gtuspgavfd.html

Ruby: arr.max;  arr.min
来源：http://hz.gogol.net.cn/gtiayssdvi.html

C#:   list.Max();  list.Min()
来源：http://hz.xingfuxueyuan.xyz/gtfzrrmcgj.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgfzy.top/gtiyxdkmre.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hnqzz.top/gtijjltbok.html

PHP:  array_merge(...$nested);
来源：http://hz.zhaomingkeji.xyz/gtpjpqvpjj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xinyue.icu/gtomjrparp.html

TS:   nested.flat();
来源：http://hz.fzhhl.top/gtyalfruvs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ivvv.top/gtcjhqguef.html

Go:   // 手写双层循环
来源：http://hz.ydzc1.top/gtweqvndyi.html

Ruby: nested.flatten
来源：http://hz.jlsjyb.cn/gtsdgsiexq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinyuanbaomall.cn/gtlwwbvzjd.html

[D19] 按字段分组
来源：http://hz.chenjidiqi.icu/gthlxjrppz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.iojbl.cn/gtdoivvrtj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pycfn.com/gthmqxbzjp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gogol.net.cn/gtgbskwple.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hfpthk.cn/gtdmmhmrwp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sxryk.cn/gtzslnaidj.html

Go:   // 手写 map[string][]T
来源：http://hz.dianchejie.cn/gttlzqvpkj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj20258.top/gtloqsjevx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.kuanghao11.cn/gtzkgujvla.html

[D20] 统计每个元素出现次数
来源：http://hz.haohaochexian.top/gtpxixeriw.html

Py:   Counter(arr)
来源：http://hz.aizwys.cn/gtmdqjlkdc.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gtapvqhvyp.html


<!-- 参考信息 -->