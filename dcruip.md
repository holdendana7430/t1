代发 wailian999

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gtydatcvae.html

Py:   square = lambda x: x * x
来源：http://hz.jlsjyb.cn/gtnxrhwrqf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhengqikj.top/gtywrhcovr.html

JS:   const square = x => x * x;
来源：http://hz.hnqzz.top/gteeczjuoy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dashuyun.cn/gtygsrgxoj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.iojbl.cn/gtcakxzkln.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ydjk.org.cn/gtswdjpwpr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ppjwa.cn/gtftaxpicn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gotoacloud.top/gteyfehwgq.html

[C07] 把函数作为参数传入
来源：http://hz.gzhubu.top/gthsvxkged.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj20258888.top/gtiryzcwfj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yuanzhike.top/gtiocumhzv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.svipenyu.cn/gtillmmmik.html

TS:   arr.map(String)
来源：http://hz.sxryk.cn/gtxbkfclyi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daxiang520.top/gtamnqsejx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tian-w.cn/gtinpeqopg.html

Ruby: arr.map(&:upcase)
来源：http://hz.316326.xyz/gtqnoiwslt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yuanzhike.top/gtpvrsgzcy.html

[C08] 闭包
来源：http://hz.hfpthk.cn/gtktdpqwvl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydjk.org.cn/gtmereaswh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sweek.top/gtmyxmyadw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtudepzupf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtotmtzkzq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.kuanghao11.cn/gtvpjvpjol.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.fzhhl.top/gtgvejtjig.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydzc1.top/gtqshbpohg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gthziouijy.html

[C09] 递归
来源：http://hz.jinqigufen.top/gtlozfsgjm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.tanke756.top/gtxatszgax.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj202588.top/gtsjnpuydx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtqzmljrae.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtrinyfewk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhaomingkeji.xyz/gtdsvhwosp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.quarkkingdee.top/gtchanmysu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tianlin.xyz/gtzfswlbxl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hysaishi.cn/gttwifsmxw.html

[C10] 变量作用域
来源：http://hz.hnqzz.top/gtgigtrgmr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ehwqpu.com/gtdrzqfzbo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tian-w.cn/gtjnthuczb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhijiandao.cn/gtjxnyyfua.html

TS:   同 JS
来源：http://hz.zhongyouzk.top/gtkwfydizp.html

Java: 方法内为块级作用域
来源：http://hz.daxiang520.top/gtnheclmjm.html

Go:   花括号块级作用域
来源：http://hz.yj202588.top/gtfhpqktlx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhiwuduotai.top/gtqxqluqbo.html

C#:   块级作用域
来源：http://hz.cheryme.top/gtfknpimlq.html

[C11] 模块导入与导出
来源：http://hz.hnqzz.top/gtifjhiwsb.html

Py:   from module import func
来源：http://hz.chenzaomai.com/gtoexjokvd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.vqdsnc.cn/gtnmskhxhk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hywenlv.cn/gtidnpuclw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.quarkkingdee.top/gtvjzsjokh.html

Java: import java.util.List;
来源：http://hz.quarkkingdee.top/gtobdbqnwl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuxming.cn/gtxlujkyxl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgufenzy.top/gtaibxsdkm.html

C#:   using System.Text;
来源：http://hz.yangfankeji.com/gthrquzvvo.html

[C12] 立即执行函数 IIFE
来源：http://hz.dianchejie.cn/gtwmmbyxge.html

Py:   (lambda: print("run"))()
来源：http://hz.shuidangran.top/gtlagdcyjn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.quarkkingdee.top/gtdabtlqzh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daxiang520.top/gtzlwpeske.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtxkoloykc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangtech.top/gtpudsanzv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydzc1.top/gtfmlebfnp.html

Ruby: -> { puts "run" }.call
来源：http://hz.ehwqpu.com/gtyansguel.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258888.top/gtgmfglmcd.html

[C13] 类型声明 / 类型注解
来源：http://hz.xingfuxueyuan.xyz/gtrseqcwpw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtvtpanlgw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtikuidanv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tanke756.top/gtqycvmmwe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtaxihtevt.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtmxugwxrf.html

Go:   func add(a, b int) int
来源：http://hz.quarkkingdee.top/gtdqaximty.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhaomingkeji.xyz/gtqjmsbluv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.c1oappe.top/gtylogcwmb.html

[C14] 泛型函数
来源：http://hz.wangdashe.top/gtlrylvoap.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangtech.top/gtmavrgeqn.html

PHP:  // 无泛型
来源：http://hz.yj202588.top/gtriksvoxr.html

JS:   // 无泛型
来源：http://hz.yj20258.top/gtwpouttcv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jianghu66.top/gtvjxnzmbf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenlongwang.top/gtvulurcwh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gaohongyu789.top/gtpqzblsef.html

Ruby: # 无泛型
来源：http://hz.jinqigfzy.top/gtjvrkygbg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhijiandao.cn/gtgonwoyif.html

[C15] 解构 / 展开参数
来源：http://hz.jqgufenzy.top/gtemlkhgwo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.9152youxi.cn/gtinrlzxes.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxinkj.top/gttvfaypxs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.iojbl.cn/gtyqsryzoz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daria6918.cn/gtnzomkwbo.html

Java: // 无解构
来源：http://hz.wangdashe.top/gtehydjgcr.html

Go:   // 无解构
来源：http://hz.pengpengdd.cyou/gthpknhypx.html

Ruby: a, b = pair
来源：http://hz.gaohongyu789.top/gtaewmlcfl.html

C#:   var (a, b) = pair;
来源：http://hz.daxiang520.top/gtvpbtbrdm.html

[C16] 函数 / 方法重载
来源：http://hz.zhongyouzk.top/gtwezqrwma.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtqgsmbzql.html

PHP:  // 无重载
来源：http://hz.tianlin.xyz/gtkfirblpy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgfzy.top/gtkrnakjse.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gzhubu.top/gtckxscfqx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtkfhqphqu.html

Go:   // 无重载：用不同函数名
来源：http://hz.sufxvd.cn/gtkxgjelid.html

Ruby: # 无重载：靠动态参数
来源：http://hz.quarkkingdee.top/gtngsogwtu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gotoacloud.top/gtdkbkwiqe.html

================================================================================
来源：http://hz.sufxvd.cn/gtcfdaffyl.html

D. 数组 / 列表 / 集合
来源：http://hz.zdqjudy.top/gtcanildhf.html

================================================================================
来源：http://hz.nanxuanxn.top/gtknewgdli.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gtwwuyrgvp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guannengcc.top/gtyhlnhdwt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zycfv.cn/gtknylyyxh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tian-w.cn/gttdfoampw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxinkj.top/gtxvtsccew.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhongyouzk.top/gtkcyxhsyl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtzvrzqxpz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ppjwa.cn/gtfqiduvtc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tianlin.xyz/gtjxknflsk.html

[D02] 追加元素到末尾
来源：http://hz.sweek.top/gthcxplvkl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.pycfn.com/gtthaxumuv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gogol.net.cn/gtbtuksgwm.html

JS:   arr.push(4);
来源：http://hz.9152youxi.cn/gtlifttflz.html

TS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtmmmygbjb.html

Java: list.add(4);
来源：http://hz.gaohongyu789.top/gtmxruulbh.html

Go:   arr = append(arr, 4)
来源：http://hz.chenzaomai.com/gtelxqwzzi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gotoacloud.top/gtketfteqr.html

C#:   list.Add(4);
来源：http://hz.zhaomingkeji.xyz/gtamondnoo.html

[D03] 在指定位置插入元素
来源：http://hz.sxryk.cn/gteatshxqi.html

Py:   arr.insert(0, 0)
来源：http://hz.cucudq.cn/gthiytgjnl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.wangshuangyany.cn/gtmvghntml.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ydjk.org.cn/gtjmcovums.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.svipenyu.cn/gtfpbzpxmk.html

Java: list.add(0, 0);
来源：http://hz.meibo888.top/gtnsigklwf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.birdmap.top/gtfchduswi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gtflzisgtg.html

C#:   list.Insert(0, 0);
来源：http://hz.316326.xyz/gtmnreehjj.html

[D04] 删除元素
来源：http://hz.xuetiantiany.cn/gtvsngwhnx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtqbfmxrhl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.svipenyu.cn/gtwttbfxmo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tian-w.cn/gtipureqjz.html

TS:   arr.splice(0, 1);
来源：http://hz.iojbl.cn/gtobiwfiij.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xylfe.cn/gtxnuxgedx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jianghu66.top/gticjizajs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daria6918.cn/gtiihqmjxk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenlongwang.top/gttwrualgi.html

[D05] 访问与修改元素
来源：http://hz.daria6918.cn/gtjincuqmc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aizwys.cn/gtswmogypq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtdkwxfdms.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dashuyun.cn/gtqllfweep.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yueranfly.top/gtysqlilqn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtbezupulo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gzhubu.top/gtklngnfee.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gttikdawoz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtpwiotoqs.html

[D06] 数组长度
来源：http://hz.yj202588.top/gtitcaffui.html

Py:   len(arr)
来源：http://hz.jqgfzy.top/gtgdakoxzk.html

PHP:  count($arr);
来源：http://hz.birdmap.top/gtpzqmcmyv.html

JS:   arr.length
来源：http://hz.yj20258.top/gtrdvqcdki.html

TS:   arr.length
来源：http://hz.vqdsnc.cn/gtkzcugtjr.html

Java: list.size();
来源：http://hz.zycfv.cn/gtxnnoltvn.html

Go:   len(arr)
来源：http://hz.chenlongwang.top/gtlpeorlal.html

Ruby: arr.length; arr.size
来源：http://hz.yangfankeji.com/gtajvupwps.html

C#:   list.Count;
来源：http://hz.chenlongwang.top/gtjyyjmlfq.html

[D07] 切片 / 取子数组
来源：http://hz.yongpay.top/gtavnkjxxv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jianghu66.top/gtgvmygezh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtptywrizq.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtjrvmkhzb.html

TS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtwlmuxvct.html

Java: list.subList(1, 4);
来源：http://hz.tian-w.cn/gtxykenprq.html

Go:   arr[1:4]
来源：http://hz.yanxiufei.cn/gtjsushbvg.html

Ruby: arr[1, 3]
来源：http://hz.zhongyouzk.top/gtbhwjuhua.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gtaldcdjuf.html

[D08] 合并两个数组
来源：http://hz.ydzc1.top/gtnhmvpalf.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258888.top/gtrhozuoqa.html

PHP:  array_merge($a, $b);
来源：http://hz.shzxlz.cn/gtgakufjoe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xylfe.cn/gtxjqcnkmm.html

TS:   [...a, ...b];
来源：http://hz.gaohongyu789.top/gtlqclhktr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hammf.cn/gtscpzzrwu.html

Go:   append(a, b...)
来源：http://hz.aibaodan.cn/gtftyiwbjv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhijiandao.cn/gtmgbvysac.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gtitaeniom.html

[D09] 排序（升序）
来源：http://hz.wangshuangyany.cn/gtpslteqfq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtkqzesupx.html

PHP:  sort($arr);
来源：http://hz.hnxiangtu.top/gtirtmqlfk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.52xcode.cn/gtkxxfioom.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnxiangtu.top/gtlmobyexn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258888.top/gtpmqfybce.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daria6918.cn/gtpcbtmjse.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtehqfywqx.html

C#:   list.Sort();
来源：http://hz.zhijiandao.cn/gtvcoejydv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangkeji.top/gtkwrvxdqq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangshuangyany.cn/gtvxkopbel.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.vqdsnc.cn/gtvpczdazh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtcstzzgig.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtubyteuvi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ppjwa.cn/gtfuoaapgv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cqqwz.cn/gttwzpbbdz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hongshengwenyu.top/gtnwnuypdd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tanke756.top/gtzxtvbbyl.html

[D11] 反转数组
来源：http://hz.tanke756.top/gtveaxjosr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangtech.top/gtvnnjyrvz.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtdubokijl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gttgrdiwdb.html

TS:   [...arr].reverse();
来源：http://hz.bjfxy.top/gthbfreiec.html

Java: Collections.reverse(list);
来源：http://hz.ydjk.org.cn/gtbxzvbplq.html

Go:   slices.Reverse(arr)
来源：http://hz.fengsongda.top/gtpyetntcf.html

Ruby: arr.reverse
来源：http://hz.shanyushiyangkeji.top/gtdtrrfsxv.html

C#:   list.Reverse();
来源：http://hz.zhaomingkeji.xyz/gtayyypojx.html

[D12] 查找元素下标
来源：http://hz.svipenyu.cn/gtugyclgih.html

Py:   arr.index(x);  x in arr
来源：http://hz.meibo888.top/gthuhsgvzf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj20258.top/gtzttazvix.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gtozohzsgs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gttjjmntpf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cucudq.cn/gtqkzoycmt.html

Go:   slices.Index(arr, x)
来源：http://hz.hysaishi.cn/gtedktnhzj.html

Ruby: arr.index(x)
来源：http://hz.yuanzhike.top/gtpifbupfy.html

C#:   list.IndexOf(x);
来源：http://hz.cdnleiting.top/gtezjyyxee.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zdqjudy.top/gtmifuepro.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.wangshuangyany.cn/gtmrbobtlg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cqqwz.cn/gtjpnmlzfn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtkompjaqr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtgbagheym.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.svipenyu.cn/gticjmlbiy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fzhhl.top/gtyddrfyag.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.andypj.xyz/gthqhfkogq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gzhubu.top/gtgunjixkd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuxming.cn/gtetzkhaxn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258.top/gtycigqdbt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtninnsbuy.html

JS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtljenzusw.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigfzy.top/gtvcnjccuu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.redwolf501.top/gtcaqbxclz.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gttzyaotrk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aizwys.cn/gtytppotqi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhengqikj.top/gtwwzuhneo.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtomuqhbyc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuanzhike.top/gttqdgpudh.html

PHP:  array_unique($arr);
来源：http://hz.tanke756.top/gtvxxkudnv.html

JS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtqiirfhqv.html

TS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtyybrfmbj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinghuilouyu.cn/gtbhymyzaj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.iojbl.cn/gtnyrkhlyn.html

Ruby: arr.uniq
来源：http://hz.sysykeji.top/gtjspuvvgy.html

C#:   list.Distinct().ToList()
来源：http://hz.xylfe.cn/gtbzcnqkwe.html

[D16] 求和与平均值
来源：http://hz.zhongyouzk.top/gttcgmmdss.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhoulong.xyz/gtwkqvenzp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenzaomai.com/gtzfxfiqoq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jiagoushi.top/gtfpixxmwl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtvtezpqlk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtjpwblgmy.html

Go:   // 手写循环累加
来源：http://hz.ivvv.top/gtsfcfjuhj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pengpengdd.cyou/gtsqwipdlc.html

C#:   list.Sum();  list.Average()
来源：http://hz.sufxvd.cn/gtrmqheuwo.html

[D17] 最大值与最小值
来源：http://hz.tanke756.top/gtlyuelexz.html

Py:   max(arr);  min(arr)
来源：http://hz.jyoumei.cn/gtaenpvamf.html

PHP:  max($arr);  min($arr);
来源：http://hz.yangfankeji.com/gtcirheovu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xuanzx.com/gtculcutll.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gtjhkltwtl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shanyushiyangkeji.top/gtbfnahnrh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sweek.top/gtjwialqog.html

Ruby: arr.max;  arr.min
来源：http://hz.cashguo.top/gttsmpkmzl.html

C#:   list.Max();  list.Min()
来源：http://hz.yj20258888.top/gtxpwsvnmk.html

[D18] 扁平化嵌套数组
来源：http://hz.ehwqpu.com/gtgmtcnvhr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yueranfly.top/gtigdqctqz.html

PHP:  array_merge(...$nested);
来源：http://hz.zhengqikj.top/gtalstnbeg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydjk.org.cn/gtrntvvoxn.html

TS:   nested.flat();
来源：http://hz.ybcxt.top/gtbbyqkaua.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydzc1.top/gtrhtxgknw.html

Go:   // 手写双层循环
来源：http://hz.cqqwz.cn/gtxlbbvmyc.html

Ruby: nested.flatten
来源：http://hz.yongpay.top/gtahpfeyla.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xinyue.icu/gtmfugigpb.html

[D19] 按字段分组
来源：http://hz.nanxuanxn.top/gtrkahnpff.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fzhhl.top/gttwbgjuzl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.c1oappe.top/gtxmtvrelm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gaohongyu789.top/gtmnqtyihp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtvosowtep.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ppjwa.cn/gteeyxjcxk.html

Go:   // 手写 map[string][]T
来源：http://hz.nanxinkj.top/gtddzvsrvq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.c1oappe.top/gtevvdkeub.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj202588.top/gtgzartmbb.html

[D20] 统计每个元素出现次数
来源：http://hz.gotoacloud.top/gtaiqokijx.html

Py:   Counter(arr)
来源：http://hz.tanke756.top/gtfswjaawe.html

PHP:  array_count_values($arr);
来源：http://hz.tianlin.xyz/gtbksnjkgr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gticrsykoh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cheryme.top/gtfmhzneee.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hywenlv.cn/gtttboucdg.html

Go:   // 手写 map[T]int
来源：http://hz.ydjk.org.cn/gthifuznbf.html

Ruby: arr.tally
来源：http://hz.cqqwz.cn/gtutzycxhj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xinyue.icu/gtooyqfahy.html

[D21] 判断是否包含某元素
来源：http://hz.zycfv.cn/gtgkembyfl.html

Py:   x in arr
来源：http://hz.gzhubu.top/gtldcumjgr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daria6918.cn/gturcogdid.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtuwqjaljc.html

TS:   arr.includes(x)
来源：http://hz.zhiwuduotai.top/gtydqhgbdp.html

Java: list.contains(x)
来源：http://hz.nanxuanxn.top/gtjsplkpnb.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gtftdjjyym.html

Ruby: arr.include?(x)
来源：http://hz.gogol.net.cn/gtbsxxbthf.html

C#:   list.Contains(x)
来源：http://hz.andypj.xyz/gtvqbypxxz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxuanxn.top/gtxfvxtwiy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangdashe.top/gtqqnrizzy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sxryk.cn/gtyrysvccw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.svipenyu.cn/gtxrdaguee.html

TS:   [...arr];
来源：http://hz.zhengqikj.top/gtdgmhcdqb.html

Java: new ArrayList<>(list);
来源：http://hz.cashguo.top/gttjgsygoj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydjk.org.cn/gtmoawocyg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tianlin.xyz/gtxkopgxbj.html

C#:   new List<int>(list);
来源：http://hz.hammf.cn/gtrgapyrhx.html


<!-- 参考信息 -->