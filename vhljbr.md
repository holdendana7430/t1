代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.cheryme.top/gtrbtwccbj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.feifeiyinyue.top/gtrtksyrmn.html

[C08] 闭包
来源：http://hz.smart0.xyz/gtgwgmwqfw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yueranfly.top/gtutqvfvsk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jianghu66.top/gtvcohlckq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtsfeyvoly.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtprkgfivf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigufen.top/gtcswqhjtu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.chenzaomai.com/gtnrprmbau.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.dashuyun.cn/gtfbvftczw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtansekxfb.html

[C09] 递归
来源：http://hz.svipenyu.cn/gtixvqulci.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258.top/gtlfwfzblm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenlongwang.top/gtpsmowsaw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtosveevmw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fzhhl.top/gtupepxhmo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cdnleiting.top/gtftygvxae.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.snrcjt.cn/gtokuwtytc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shanyushiyangkeji.top/gtediixgbd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pycfn.com/gtjjcvkrsa.html

[C10] 变量作用域
来源：http://hz.havefunace.top/gtbtjhovsp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xylfe.cn/gtdhgcdpak.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pengpengdd.cyou/gtdnsnuzmq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gtudkimxmv.html

TS:   同 JS
来源：http://hz.ybcxt.top/gttbdhmbay.html

Java: 方法内为块级作用域
来源：http://hz.chenlongwang.top/gtcmvfovbf.html

Go:   花括号块级作用域
来源：http://hz.jlsjyb.cn/gtdpilcdlp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.316326.xyz/gtaisrpddw.html

C#:   块级作用域
来源：http://hz.svipenyu.cn/gttuqrjgyx.html

[C11] 模块导入与导出
来源：http://hz.pengpengdd.cyou/gtcefndppt.html

Py:   from module import func
来源：http://hz.sweek.top/gtzjsqvsdk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yanxiufei.cn/gtszkgkgqu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.svipenyu.cn/gtoztjzdwz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yonumen.top/gtuspbcpcg.html

Java: import java.util.List;
来源：http://hz.wangshuangyany.cn/gtildxgpbs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hammf.cn/gttrhmvmoz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fengsongda.top/gtmasbcxbw.html

C#:   using System.Text;
来源：http://hz.sweek.top/gtlrxsyvoi.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinyuanbaomall.cn/gttbyexovz.html

Py:   (lambda: print("run"))()
来源：http://hz.sweek.top/gtnatfktis.html

PHP:  (function () { echo "run"; })();
来源：http://hz.havefunace.top/gttklabwdr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtjthqizao.html

TS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gtafrpgxle.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258.top/gtclmdwlle.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.quarkkingdee.top/gtsfxkpqhg.html

Ruby: -> { puts "run" }.call
来源：http://hz.ppjwa.cn/gtvajknbit.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhixingplan.top/gtvazrxgeq.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtvssedijh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.tianlin.xyz/gtkqlrnsdl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtykuuqbxl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.feifeiyinyue.top/gtpvtsxarv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ybcxt.top/gtkrvivaso.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtyozjjnvb.html

Go:   func add(a, b int) int
来源：http://hz.shangyingyoupin.top/gtgldogjws.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ybcxt.top/gtrbxoxlva.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sxryk.cn/gttjphtzlt.html

[C14] 泛型函数
来源：http://hz.zhoulong.xyz/gtztzhnkmf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gthsnxtyyv.html

PHP:  // 无泛型
来源：http://hz.hysaishi.cn/gtzejgspck.html

JS:   // 无泛型
来源：http://hz.cqqwz.cn/gtjlawgrei.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhaomingkeji.xyz/gtwyenkkuk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ywan-chungtsiang.top/gtjssaqbks.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnqzz.top/gtculvapty.html

Ruby: # 无泛型
来源：http://hz.zhijiandao.cn/gtraabruzh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gzhubu.top/gtrfmlqash.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtvbdqfucu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xinyue.icu/gthaljjggi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pycfn.com/gtusmvilxt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtdilpampt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.0kj1m.cn/gtepthpayc.html

Java: // 无解构
来源：http://hz.feifeiyinyue.top/gtuyaayyuz.html

Go:   // 无解构
来源：http://hz.yuxming.cn/gtewuuzurv.html

Ruby: a, b = pair
来源：http://hz.cucudq.cn/gtjncruuxp.html

C#:   var (a, b) = pair;
来源：http://hz.9152youxi.cn/gtlqrswzpu.html

[C16] 函数 / 方法重载
来源：http://hz.nanxuanxn.top/gtmuhthpdd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.aizwys.cn/gtpzorworj.html

PHP:  // 无重载
来源：http://hz.ydzc1.top/gtfwubhddk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yvedp.cn/gtxpuhffod.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gzhubu.top/gtxapuedts.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hfpthk.cn/gtbeayluvd.html

Go:   // 无重载：用不同函数名
来源：http://hz.yonumen.top/gtfxjigrtl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenlongwang.top/gtiiirqbqg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuanzhike.top/gtbeapdphg.html

================================================================================
来源：http://hz.andypj.xyz/gtrzudprjv.html

D. 数组 / 列表 / 集合
来源：http://hz.haohaochexian.top/gtlyvbkllz.html

================================================================================
来源：http://hz.shuidangran.top/gtkbkyoavx.html

[D01] 创建数组 / 列表
来源：http://hz.cdnleiting.top/gttgnuwbqe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hongshengwenyu.top/gtfahekjvr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hysaishi.cn/gtvkkxropc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tanke756.top/gtcjzvsmlv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gtytaqnxvh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cashguo.top/gtsnmgxkqc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sxryk.cn/gtqfuxqxyr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtgthlbzzy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shangyingyoupin.top/gtewctswfn.html

[D02] 追加元素到末尾
来源：http://hz.xuanzx.com/gtdsnbsgtn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangdashe.top/gtdgsksegy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenzaomai.com/gtxxianhmr.html

JS:   arr.push(4);
来源：http://hz.bjfxy.top/gtfaekzjsx.html

TS:   arr.push(4);
来源：http://hz.yonumen.top/gtnqgdtxwq.html

Java: list.add(4);
来源：http://hz.snrcjt.cn/gtgsvwvlmg.html

Go:   arr = append(arr, 4)
来源：http://hz.zhiwuduotai.top/gtbzcxuegh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhaomingkeji.xyz/gtttcttabs.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangkeji.top/gtdctdwskg.html

[D03] 在指定位置插入元素
来源：http://hz.ivvv.top/gteccctvuf.html

Py:   arr.insert(0, 0)
来源：http://hz.mhx1999.top/gthjjckcuv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guannengcc.top/gtifpbxbgt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ydjk.org.cn/gtzjxivfdf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinghuilouyu.cn/gtyntniwde.html

Java: list.add(0, 0);
来源：http://hz.gogol.net.cn/gtfrstfjzl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ppjwa.cn/gtkgrnhake.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.snrcjt.cn/gtrbudyubb.html

C#:   list.Insert(0, 0);
来源：http://hz.daria6918.cn/gtqfprdhyb.html

[D04] 删除元素
来源：http://hz.shangyingyoupin.top/gtfixqfnfj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.0kj1m.cn/gtqzijnxaj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangshuangyany.cn/gtsodquwme.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenzaomai.com/gtckmbzvvu.html

TS:   arr.splice(0, 1);
来源：http://hz.jlsjyb.cn/gtrafousrf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.316326.xyz/gtsgxnolbv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.mhx1999.top/gthujumsvg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ywan-chungtsiang.top/gtpdcrzkkg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zycfv.cn/gtophviqgo.html

[D05] 访问与修改元素
来源：http://hz.yj20258.top/gtohirfacc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtjlojaevg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.0kj1m.cn/gtiaffgyis.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cucudq.cn/gtzhmoulkj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tianlin.xyz/gtzcdvjfzo.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenjidiqi.icu/gtnvkyspkz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtrecoguas.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtzvdkgbsq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.52xcode.cn/gtjqnymwyq.html

[D06] 数组长度
来源：http://hz.yueranfly.top/gtjnviplpu.html

Py:   len(arr)
来源：http://hz.dashuyun.cn/gtlitlqpqd.html

PHP:  count($arr);
来源：http://hz.hongshengwenyu.top/gtscgrhobh.html

JS:   arr.length
来源：http://hz.zhongyouzk.top/gtydavpeef.html

TS:   arr.length
来源：http://hz.xingfuxueyuan.xyz/gtpoxuxzvg.html

Java: list.size();
来源：http://hz.guannengcc.top/gthdcxrfhw.html

Go:   len(arr)
来源：http://hz.xuetiantiany.cn/gtjbrevhow.html

Ruby: arr.length; arr.size
来源：http://hz.snrcjt.cn/gtcijdmodp.html

C#:   list.Count;
来源：http://hz.bjfxy.top/gtrwyqepnm.html

[D07] 切片 / 取子数组
来源：http://hz.yj202588.top/gtmrzbpgav.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.smart0.xyz/gtgvnuznal.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daxiang520.top/gtqzxgdtsy.html

JS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtqhpgappe.html

TS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtbdehpnmw.html

Java: list.subList(1, 4);
来源：http://hz.yvedp.cn/gtatsixeit.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtntbvzuck.html

Ruby: arr[1, 3]
来源：http://hz.ybcxt.top/gtxyqrhipa.html

C#:   list.GetRange(1, 3);
来源：http://hz.hfpthk.cn/gtvonhgywz.html

[D08] 合并两个数组
来源：http://hz.tianlin.xyz/gtsenkacib.html

Py:   a + b;  a.extend(b)
来源：http://hz.guowangkeji.top/gtqqxpdzdn.html

PHP:  array_merge($a, $b);
来源：http://hz.havefunace.top/gtaunezzzo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gzhubu.top/gtwwxxpmhr.html

TS:   [...a, ...b];
来源：http://hz.sxryk.cn/gtkawsdkdp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.0kj1m.cn/gtjdaqdlgg.html

Go:   append(a, b...)
来源：http://hz.cqqwz.cn/gtdvgxgprq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.snrcjt.cn/gtjgtgeovo.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtxoqnxmpl.html

[D09] 排序（升序）
来源：http://hz.nanxuanxn.top/gtoprieezi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtklfuslni.html

PHP:  sort($arr);
来源：http://hz.yongpay.top/gtaihxvosm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.mhx1999.top/gtfqmlueth.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yueranfly.top/gtxjftktsa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gogol.net.cn/gtqqztgytl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtcjutoniz.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtvhzuwagi.html

C#:   list.Sort();
来源：http://hz.gotoacloud.top/gthbvfqgox.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dianchejie.cn/gtegaqktxc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.redwolf501.top/gtdjpflngp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gzhubu.top/gtevzmrnpb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtrkqututa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtzqlkznxd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tianlin.xyz/gtzwynnsdd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pengpengdd.cyou/gttewphkcn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hywenlv.cn/gtswmupxoo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cdnleiting.top/gtttoikrcd.html

[D11] 反转数组
来源：http://hz.andypj.xyz/gthxdglfdc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.smart0.xyz/gtkexqcdpl.html

PHP:  array_reverse($arr);
来源：http://hz.zhaomingkeji.xyz/gtenizniuj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenjidiqi.icu/gttuwzaoxr.html

TS:   [...arr].reverse();
来源：http://hz.zhixingplan.top/gtwfnalokq.html

Java: Collections.reverse(list);
来源：http://hz.jiagoushi.top/gtwewecxmw.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangtech.top/gtimcqkcux.html

Ruby: arr.reverse
来源：http://hz.chenjidiqi.icu/gtzpfmsbxg.html

C#:   list.Reverse();
来源：http://hz.jianghu66.top/gtmypfnwud.html

[D12] 查找元素下标
来源：http://hz.guowangkeji.top/gtgwtebbzv.html

Py:   arr.index(x);  x in arr
来源：http://hz.ywan-chungtsiang.top/gtyklyzkbg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.9152youxi.cn/gtzvmcsnhy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.haohaochexian.top/gtpkejuxgd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtaloqsmoc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtztchkxde.html

Go:   slices.Index(arr, x)
来源：http://hz.xuetiantiany.cn/gtepkhnqvr.html

Ruby: arr.index(x)
来源：http://hz.jianghu66.top/gtahsiuirs.html

C#:   list.IndexOf(x);
来源：http://hz.yanxiufei.cn/gtxjcwnreg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jyoumei.cn/gtjovkhgns.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhoulong.xyz/gtzecwpcvm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtuqxoqgij.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gtdufvllam.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cqqwz.cn/gtyszmpyyc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhaomingkeji.xyz/gtdrosjupj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ybcxt.top/gtoqnfuhxl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nwbrower.top/gtriupaiil.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daria6918.cn/gtvllyauof.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yangfankeji.com/gtvfrchzoa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.havefunace.top/gtzayumchk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yonumen.top/gtlewcyyve.html

JS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtcrukzelk.html

TS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtjcsprddk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hysaishi.cn/gtmcncfksj.html

Go:   // 手写循环
来源：http://hz.ehwqpu.com/gtfvzzfkae.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shangyingyoupin.top/gtrzwqevkt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cheryme.top/gtaosqqqxw.html

[D15] 去重
来源：http://hz.tianlin.xyz/gtazkueous.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtlgzvetez.html

PHP:  array_unique($arr);
来源：http://hz.0kj1m.cn/gtziftaaca.html

JS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtnwbixxho.html

TS:   [...new Set(arr)]
来源：http://hz.c1oappe.top/gtslxlwzkv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtuvxtofbm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtozvheyua.html

Ruby: arr.uniq
来源：http://hz.sufxvd.cn/gtbpshcfgd.html

C#:   list.Distinct().ToList()
来源：http://hz.cashguo.top/gtnwwhajvs.html

[D16] 求和与平均值
来源：http://hz.jlsjyb.cn/gtppgxbadm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.meibo888.top/gtvkdodedo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hongshengwenyu.top/gtxhyghoqi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtsolnjrrf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtybpoqyeq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hfpthk.cn/gthdzbmxmo.html

Go:   // 手写循环累加
来源：http://hz.yj20258.top/gtyrjhjtog.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pengpengdd.cyou/gtkdpdixmu.html

C#:   list.Sum();  list.Average()
来源：http://hz.aizwys.cn/gtigiochjf.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gtdmgombia.html

Py:   max(arr);  min(arr)
来源：http://hz.0kj1m.cn/gtuwuweurd.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtesheduya.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sufxvd.cn/gtiebyicau.html

TS:   Math.max(...arr);
来源：http://hz.0kj1m.cn/gtkydimvjo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cqqwz.cn/gtpnuhtvbe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sxryk.cn/gtcjpxlhob.html

Ruby: arr.max;  arr.min
来源：http://hz.jiagoushi.top/gtieqruxiy.html

C#:   list.Max();  list.Min()
来源：http://hz.shangyingyoupin.top/gtafitaifk.html

[D18] 扁平化嵌套数组
来源：http://hz.bjfxy.top/gtnyxwualb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.snrcjt.cn/gtebuzyksj.html

PHP:  array_merge(...$nested);
来源：http://hz.yonumen.top/gtmqsozxjd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ybcxt.top/gtkpgiwndz.html

TS:   nested.flat();
来源：http://hz.zhaomingkeji.xyz/gtgovfkjfx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shangyingyoupin.top/gtwgpryhde.html

Go:   // 手写双层循环
来源：http://hz.yueranfly.top/gtzmxbttev.html

Ruby: nested.flatten
来源：http://hz.hywenlv.cn/gtmofvmcuo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydzc1.top/gtbehjzaem.html

[D19] 按字段分组
来源：http://hz.9152youxi.cn/gtryjzcvvg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yanxiufei.cn/gtqhhjjdno.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.vqdsnc.cn/gtjtdndxdg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtnaakzudl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gtgovaqnsq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shanyushiyangkeji.top/gtirgtkaaj.html

Go:   // 手写 map[string][]T
来源：http://hz.316326.xyz/gtnzbmrfvj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhongyouzk.top/gtdxditdrs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhaomingkeji.xyz/gtowdmtnco.html

[D20] 统计每个元素出现次数
来源：http://hz.mhx1999.top/gtcsroptbi.html

Py:   Counter(arr)
来源：http://hz.sysykeji.top/gtwwfbhaag.html

PHP:  array_count_values($arr);
来源：http://hz.svipenyu.cn/gteulzxohb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtapxhznhn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jlsjyb.cn/gtokiyptqv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xingfuxueyuan.xyz/gtlveppvtu.html

Go:   // 手写 map[T]int
来源：http://hz.zhaomingkeji.xyz/gtrasaznqt.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtmefcouba.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhoulong.xyz/gtqpqvflik.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtczlbldcn.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gtgbptisay.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydjk.org.cn/gtmlkoccsh.html

JS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gtztjuzqez.html

TS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gthccvcpdm.html

Java: list.contains(x)
来源：http://hz.nanxinkj.top/gthupvblzh.html

Go:   slices.Contains(arr, x)
来源：http://hz.cheryme.top/gtmlizrqcn.html

Ruby: arr.include?(x)
来源：http://hz.c1oappe.top/gtrmtqkfxf.html

C#:   list.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtafuhacvb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.dianchejie.cn/gtbynscrfg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.mhx1999.top/gtoeglelqj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.iojbl.cn/gtiddrzmyl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.guannengcc.top/gtsjyvjddm.html

TS:   [...arr];
来源：http://hz.ybcxt.top/gtvozbgrty.html

Java: new ArrayList<>(list);
来源：http://hz.fzhhl.top/gtitvwuyjn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuanzhike.top/gtmeehleeq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xingfuxueyuan.xyz/gtjxwchkvl.html

C#:   new List<int>(list);
来源：http://hz.xylfe.cn/gtemjjlfhn.html

[D23] reduce 累积计算
来源：http://hz.hysaishi.cn/gtrnbusgzx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jyoumei.cn/gthhpwjvme.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.guannengcc.top/gtnzarghlh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gtdgaowcgr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtxnwszgut.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhiwuduotai.top/gtyvbiggsb.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gtmscovghr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtopcanegj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daxiang520.top/gtpkvrkpym.html

[D24] 字典 / Map 基本操作
来源：http://hz.haohaochexian.top/gttothfwfw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhoulong.xyz/gtokfsbpgd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gaohongyu789.top/gtjmhjyynz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.meibo888.top/gtabfowafi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinghuilouyu.cn/gtxlmrzdcv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tanke756.top/gtqhbprodd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hywenlv.cn/gtunlyjrfu.html


<!-- 参考信息 -->