代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtbjhajmiv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cashguo.top/gtosprnhcw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.mhx1999.top/gtmgmnekmw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jianghu66.top/gtjmchsovm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yueranfly.top/gtezywmqvm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tianlin.xyz/gtwoowlglh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.dashuyun.cn/gtolxghvyj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinqigfzy.top/gtldolvtth.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.wangdashe.top/gtexpfwkue.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtyxpxdzbf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zycfv.cn/gtpgdzqodu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhaomingkeji.xyz/gtfufzjsei.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhongyouzk.top/gtoddwuyci.html

Ruby: f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtwdpwtoqg.html

C#:   f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtxxggyrsf.html

[C05] 返回多个值
来源：http://hz.iojbl.cn/gttbmrbazn.html

Py:   return a, b
来源：http://hz.aizwys.cn/gtmmzstthn.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gtojklyszu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhiwuduotai.top/gtlmrerpxq.html

TS:   return { a, b };
来源：http://hz.jqgufenzy.top/gtffcuvcta.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jianghu66.top/gtzrokktpe.html

Go:   return a, b
来源：http://hz.hywenlv.cn/gtyltlmrxo.html

Ruby: return a, b
来源：http://hz.chenzaomai.com/gtksleclfy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.52xcode.cn/gtunttbzgi.html

[C06] 匿名函数 / lambda
来源：http://hz.cqqwz.cn/gtefxzgvyp.html

Py:   square = lambda x: x * x
来源：http://hz.redwolf501.top/gtrpgyyxsh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.316326.xyz/gtkjnnizzk.html

JS:   const square = x => x * x;
来源：http://hz.yonumen.top/gtxaulbvej.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhoulong.xyz/gtwgazohct.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guowangkeji.top/gtogozoruk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jlsjyb.cn/gtqxiedqjx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yanxiufei.cn/gtfqrhyjhf.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.fengsongda.top/gtyvkwqklz.html

[C07] 把函数作为参数传入
来源：http://hz.gogol.net.cn/gtucfbglkk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yuanzhike.top/gtqghetwsc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhongyouzk.top/gtewbnzmiu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dianchejie.cn/gtjsjhxyqq.html

TS:   arr.map(String)
来源：http://hz.cheryme.top/gtsfpcabpx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.52xcode.cn/gtxyghnbnr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gogol.net.cn/gtydianmel.html

Ruby: arr.map(&:upcase)
来源：http://hz.yuxming.cn/gtkuhhsfbg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jqgufenzy.top/gtrnkexcoy.html

[C08] 闭包
来源：http://hz.xuanzx.com/gtyuztaucf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xinyue.icu/gtcqsazgxl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tanke756.top/gtqhxaohfe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtwmceazuj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtqpofoeha.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhijiandao.cn/gtjzsugzck.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gogol.net.cn/gtjpekxrvl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.vqdsnc.cn/gtqgojbrgd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtslkdenye.html

[C09] 递归
来源：http://hz.sxryk.cn/gtterpbknd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sweek.top/gtyfyeijru.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sweek.top/gteqgfydkl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtnaebfhry.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtezgcodar.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenjidiqi.icu/gtasxgmuhx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.wangshuangyany.cn/gtgybyzlhp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.guannengcc.top/gtzblmwpyr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.iojbl.cn/gtqasxxpck.html

[C10] 变量作用域
来源：http://hz.hfpthk.cn/gtslnqeako.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.0kj1m.cn/gtlohdulmh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daxiang520.top/gtogxksmuv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hywenlv.cn/gtulskwqjh.html

TS:   同 JS
来源：http://hz.redwolf501.top/gtrtakxoro.html

Java: 方法内为块级作用域
来源：http://hz.yongpay.top/gtxwqwisqx.html

Go:   花括号块级作用域
来源：http://hz.yvedp.cn/gtshpcfgdy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yuanzhike.top/gtevbyzsag.html

C#:   块级作用域
来源：http://hz.zhaomingkeji.xyz/gtjtxhafxj.html

[C11] 模块导入与导出
来源：http://hz.shangyingyoupin.top/gtlqjjwlvo.html

Py:   from module import func
来源：http://hz.gogol.net.cn/gtcsaiqyxq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zdqjudy.top/gthqiapqey.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuxming.cn/gtsostuvyv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guannengcc.top/gtnunooesu.html

Java: import java.util.List;
来源：http://hz.meibo888.top/gtomdwiwue.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shanyushiyangtech.top/gtllxwsech.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydzc1.top/gteauvspmd.html

C#:   using System.Text;
来源：http://hz.sweek.top/gtkcwtrtfa.html

[C12] 立即执行函数 IIFE
来源：http://hz.jiagoushi.top/gtsxauyijn.html

Py:   (lambda: print("run"))()
来源：http://hz.zhongyouzk.top/gtoextsxgi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.haohaochexian.top/gtfrhoxxpc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gttaknjdzw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtjesrtoic.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnqzz.top/gtecwuirae.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jianghu66.top/gtnhqsksci.html

Ruby: -> { puts "run" }.call
来源：http://hz.sxryk.cn/gtigepvooj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yonumen.top/gtluyonhgv.html

[C13] 类型声明 / 类型注解
来源：http://hz.hammf.cn/gtlrkxzqqm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtepszetwo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gtovdnroij.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhoulong.xyz/gtmlvpptjs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cucudq.cn/gtjrybqfkp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtkkirfjir.html

Go:   func add(a, b int) int
来源：http://hz.xuanzx.com/gteoracnmq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jianghu66.top/gtotpimqdj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jlsjyb.cn/gtzfbljxyc.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtokllkrcb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nwbrower.top/gtdphbyygt.html

PHP:  // 无泛型
来源：http://hz.feifeiyinyue.top/gtcdkvusob.html

JS:   // 无泛型
来源：http://hz.yanxiufei.cn/gtvcuiyfid.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tian-w.cn/gtofzigzjd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ehwqpu.com/gtzherqhad.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuanzhike.top/gthjvbwjjc.html

Ruby: # 无泛型
来源：http://hz.hfpthk.cn/gtudwhjbpe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtjvnvljzp.html

[C15] 解构 / 展开参数
来源：http://hz.zhengqikj.top/gtexjygoxc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cashguo.top/gtbclavabe.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258.top/gttjkbnnqa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtxefdpngj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangshuangyany.cn/gttrigpqic.html

Java: // 无解构
来源：http://hz.hywenlv.cn/gtlmgaanlc.html

Go:   // 无解构
来源：http://hz.sufxvd.cn/gtcopsrqnp.html

Ruby: a, b = pair
来源：http://hz.yj20258.top/gtaplvvjar.html

C#:   var (a, b) = pair;
来源：http://hz.ydjk.org.cn/gtvvglcclc.html

[C16] 函数 / 方法重载
来源：http://hz.fzhhl.top/gtibzilyfz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sysykeji.top/gtkywtbiez.html

PHP:  // 无重载
来源：http://hz.ydjk.org.cn/gtfgjafdkr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangtech.top/gtcunacvkm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cheryme.top/gtocrcnhkb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cashguo.top/gtoddkodnw.html

Go:   // 无重载：用不同函数名
来源：http://hz.redwolf501.top/gtjeeggibq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangshuangyany.cn/gtkgmuqguh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.quarkkingdee.top/gtbipguedc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtkgtqohxv.html

D. 数组 / 列表 / 集合
来源：http://hz.cheryme.top/gtfiwoolmc.html

================================================================================
来源：http://hz.chenzaomai.com/gtcpnnhxbs.html

[D01] 创建数组 / 列表
来源：http://hz.aizwys.cn/gtpiywruaa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.fzhhl.top/gtlubwbdpg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gtiniwgzmd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xinyue.icu/gtxncocoes.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ydjk.org.cn/gthahekzbh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gaohongyu789.top/gtkhmcoyqo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daxiang520.top/gtgswvbuzf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ywan-chungtsiang.top/gtyjgvjcud.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gtiqlsvrsc.html

[D02] 追加元素到末尾
来源：http://hz.hnxiangtu.top/gtwezsvckx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.meibo888.top/gtfkcotpej.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sysykeji.top/gtvuvsylis.html

JS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtdnxvwelf.html

TS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtnvgvexsc.html

Java: list.add(4);
来源：http://hz.hongshengwenyu.top/gtjczrpliy.html

Go:   arr = append(arr, 4)
来源：http://hz.redwolf501.top/gtcezdpvqd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenjidiqi.icu/gteqbarwif.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangkeji.top/gtkicskket.html

[D03] 在指定位置插入元素
来源：http://hz.yongpay.top/gtrwbrmpux.html

Py:   arr.insert(0, 0)
来源：http://hz.shzxlz.cn/gtxqmsbbhm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ppjwa.cn/gtdxfpzqtu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258.top/gtqcopzccb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhixingplan.top/gtddfggioz.html

Java: list.add(0, 0);
来源：http://hz.zhiwuduotai.top/gtbybhjvee.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuetiantiany.cn/gtrpiunnja.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.feifeiyinyue.top/gttrwvgrxx.html

C#:   list.Insert(0, 0);
来源：http://hz.ppjwa.cn/gthbferysc.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtpxkuufnp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.guowangkeji.top/gtovxftctg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.svipenyu.cn/gtkodrxakk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhijiandao.cn/gtzciurazb.html

TS:   arr.splice(0, 1);
来源：http://hz.cucudq.cn/gtefbkknly.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangshuangyany.cn/gtqvwghkfx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.andypj.xyz/gtgvwiawnd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fengsongda.top/gtfqkzdkwo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hongshengwenyu.top/gtndgdrvlq.html

[D05] 访问与修改元素
来源：http://hz.zdqjudy.top/gtzhfmorgb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtkxboieop.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenlongwang.top/gtwaehstxh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.wangdashe.top/gtdumlgvjv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ydzc1.top/gtmpoaqdfq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ywan-chungtsiang.top/gtoxghhbha.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtkfmbpcey.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtmuayxwuk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shuidangran.top/gtrnknsacl.html

[D06] 数组长度
来源：http://hz.yueranfly.top/gtglgrgkrb.html

Py:   len(arr)
来源：http://hz.feifeiyinyue.top/gtfzepyncy.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtaszaelcd.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtlvfmvsxk.html

TS:   arr.length
来源：http://hz.xuetiantiany.cn/gtaumqysmp.html

Java: list.size();
来源：http://hz.tanke756.top/gtddpbdvuk.html

Go:   len(arr)
来源：http://hz.wangshuangyany.cn/gtrcckomcz.html

Ruby: arr.length; arr.size
来源：http://hz.andypj.xyz/gteonmxxvi.html

C#:   list.Count;
来源：http://hz.chenjidiqi.icu/gtaisyafvh.html

[D07] 切片 / 取子数组
来源：http://hz.chenjidiqi.icu/gtcijskzlj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.wangdashe.top/gtimlngoqx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuanzhike.top/gtfldmwkgc.html

JS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtkwqxvpww.html

TS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtikvpzmgy.html

Java: list.subList(1, 4);
来源：http://hz.jqgufenzy.top/gtrcvhziwa.html

Go:   arr[1:4]
来源：http://hz.shuidangran.top/gtpolhovxg.html

Ruby: arr[1, 3]
来源：http://hz.xingfuxueyuan.xyz/gtpmlqqqlf.html

C#:   list.GetRange(1, 3);
来源：http://hz.yvedp.cn/gtqoonkxsa.html

[D08] 合并两个数组
来源：http://hz.redwolf501.top/gtbyfcrdwu.html

Py:   a + b;  a.extend(b)
来源：http://hz.quarkkingdee.top/gtridvdpxa.html

PHP:  array_merge($a, $b);
来源：http://hz.cucudq.cn/gtfwszlavw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj202588.top/gtnybcxowe.html

TS:   [...a, ...b];
来源：http://hz.vqdsnc.cn/gtwyobzlym.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtpkbostog.html

Go:   append(a, b...)
来源：http://hz.aizwys.cn/gtimmlggik.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aibaodan.cn/gtzvnnvhsh.html

C#:   a.Concat(b).ToList()
来源：http://hz.feifeiyinyue.top/gtebeyaxyh.html

[D09] 排序（升序）
来源：http://hz.quarkkingdee.top/gtzvdcalfv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtvutsjctf.html

PHP:  sort($arr);
来源：http://hz.svipenyu.cn/gtpglitlfa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.meibo888.top/gtgrwumtnr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shzxlz.cn/gtdmoiiabu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.dianchejie.cn/gtempgovnq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cashguo.top/gtpbfqgjak.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtzijhdfnp.html

C#:   list.Sort();
来源：http://hz.xuetiantiany.cn/gtbtktlxal.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.birdmap.top/gtfbdqddss.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ppjwa.cn/gtebdinnzw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.andypj.xyz/gtkknbuwog.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gthdrapqjp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtotrnnaeh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ybcxt.top/gtioawiyax.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.havefunace.top/gtheiueoey.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhongyouzk.top/gtvyxapexo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtblcbowmb.html

[D11] 反转数组
来源：http://hz.ywan-chungtsiang.top/gtemvqslpq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtnzihqtwc.html

PHP:  array_reverse($arr);
来源：http://hz.tian-w.cn/gtdnjpfxiq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jianghu66.top/gtdtutvfgs.html

TS:   [...arr].reverse();
来源：http://hz.jinqigfzy.top/gtiydqmlbc.html

Java: Collections.reverse(list);
来源：http://hz.pycfn.com/gtxfhqibgj.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtrrsovlpm.html

Ruby: arr.reverse
来源：http://hz.ywan-chungtsiang.top/gtiqkcwmah.html

C#:   list.Reverse();
来源：http://hz.nanxinkj.top/gtszxkuses.html

[D12] 查找元素下标
来源：http://hz.yueranfly.top/gtvqzuyysp.html

Py:   arr.index(x);  x in arr
来源：http://hz.fengsongda.top/gtdscqcayz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtoryeqthq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtuigcrtgf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sufxvd.cn/gtkhumgasq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.aizwys.cn/gtyunmjkxx.html

Go:   slices.Index(arr, x)
来源：http://hz.guowangkeji.top/gtxcvnpstb.html

Ruby: arr.index(x)
来源：http://hz.birdmap.top/gtyobmnvko.html

C#:   list.IndexOf(x);
来源：http://hz.fzhhl.top/gtlsomtbsp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtqnffnqch.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.0kj1m.cn/gtobdepehg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jianghu66.top/gtwbjgssfw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xylfe.cn/gtgpkspyty.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtljjoiykj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.haohaochexian.top/gtjptdtlhy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.aizwys.cn/gtwszgayvg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xziqi.cn/gtgpvjoilt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.snrcjt.cn/gtsxjlexec.html

[D14] 映射转换（每个元素变形）
来源：http://hz.haohaochexian.top/gtizemcmyz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sweek.top/gthccbhnks.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gtszhgrmix.html

JS:   arr.map(x => x * 2)
来源：http://hz.cdnleiting.top/gteznodgpt.html

TS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtkddzexvz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.smart0.xyz/gtjoejcysq.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtxkxbcaye.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nwbrower.top/gthfegnfkc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gzhubu.top/gtgznesijb.html

[D15] 去重
来源：http://hz.shanyushiyangtech.top/gttwdosbaf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhixingplan.top/gtqengxyej.html

PHP:  array_unique($arr);
来源：http://hz.chenzaomai.com/gtfygmssrb.html

JS:   [...new Set(arr)]
来源：http://hz.yj20258888.top/gtfordegrf.html

TS:   [...new Set(arr)]
来源：http://hz.daxiang520.top/gtmzpmepsq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.c1oappe.top/gttbrubgmu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ehwqpu.com/gtbmwysaht.html

Ruby: arr.uniq
来源：http://hz.jlsjyb.cn/gtgltwphgn.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtcmteikyb.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gtwbaylwzn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.0kj1m.cn/gturyahtfn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.snrcjt.cn/gtvtrpghlq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtwrpikjbr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtqnaivsuv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hysaishi.cn/gtsykaqyao.html

Go:   // 手写循环累加
来源：http://hz.chenlongwang.top/gtqttzpqsn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhoulong.xyz/gtmiinubtk.html

C#:   list.Sum();  list.Average()
来源：http://hz.xziqi.cn/gtcuxjbdxb.html

[D17] 最大值与最小值
来源：http://hz.zycfv.cn/gtqqipwvbn.html

Py:   max(arr);  min(arr)
来源：http://hz.daxiang520.top/gtsdryffel.html

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtwuxwpuyh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258888.top/gtlvzargls.html

TS:   Math.max(...arr);
来源：http://hz.zhongyouzk.top/gttzqrnkth.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenzaomai.com/gtgwpnwnbg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhengqikj.top/gtlbvxjhkr.html

Ruby: arr.max;  arr.min
来源：http://hz.zycfv.cn/gtsncyzdxx.html

C#:   list.Max();  list.Min()
来源：http://hz.yuanzhike.top/gtsvrwuiew.html

[D18] 扁平化嵌套数组
来源：http://hz.0kj1m.cn/gtueaaihfz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhiwuduotai.top/gthgcksszb.html

PHP:  array_merge(...$nested);
来源：http://hz.daxiang520.top/gtbvhioxwg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydjk.org.cn/gtryajbmgf.html

TS:   nested.flat();
来源：http://hz.wangdashe.top/gtxfdoxszd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aibaodan.cn/gtktrsmuir.html

Go:   // 手写双层循环
来源：http://hz.0kj1m.cn/gtszoizqrw.html

Ruby: nested.flatten
来源：http://hz.jinqigufen.top/gtpblvbtkl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yangfankeji.com/gtnlrohptq.html

[D19] 按字段分组
来源：http://hz.haohaochexian.top/gtxhtxucge.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cqqwz.cn/gtehrbsexy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cheryme.top/gthbtmbpsr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shanyushiyangtech.top/gtlyhgrbuu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258888.top/gtiaidjxcb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuxming.cn/gtaijkclhk.html

Go:   // 手写 map[string][]T
来源：http://hz.snrcjt.cn/gtdmvymzfh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj202588.top/gtrvzfrkfg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydzc1.top/gtfqnoyvef.html

[D20] 统计每个元素出现次数
来源：http://hz.birdmap.top/gtharaauwm.html

Py:   Counter(arr)
来源：http://hz.jlsjyb.cn/gtfoujevaq.html

PHP:  array_count_values($arr);
来源：http://hz.zhongyouzk.top/gtekbvbzvd.html


<!-- 参考信息 -->