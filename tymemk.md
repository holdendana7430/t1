代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yuxming.cn/gtjyoqddrg.html

TS:   arr.map(String)
来源：http://hz.jinyuanbaomall.cn/gtlibrufjs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hywenlv.cn/gtvjhzifti.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yvedp.cn/gtgajcrjqf.html

Ruby: arr.map(&:upcase)
来源：http://hz.9152youxi.cn/gtnxqqblmb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenjidiqi.icu/gtovhffmsd.html

[C08] 闭包
来源：http://hz.kuanghao11.cn/gthuqgcojt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nanxinkj.top/gtgmysxser.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ydjk.org.cn/gtndwywgyn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gttcjpveyh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtykracedq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenzaomai.com/gtyrhlinqq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shangyingyoupin.top/gthtpyyzlm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinqigufen.top/gtddtovyjv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtzjuzdbzn.html

[C09] 递归
来源：http://hz.sysykeji.top/gtymwtgmqu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtdbigpqpr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xziqi.cn/gtddnhkwrn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gtwoklslip.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtjafcrhyc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinqigfzy.top/gtnyvnvoyw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aibaodan.cn/gtteapjsku.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hnxiangtu.top/gtkgvgqvab.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhijiandao.cn/gtqwcrawzj.html

[C10] 变量作用域
来源：http://hz.guowangkeji.top/gtmmmgsvqr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhengqikj.top/gtsfqqlnrg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinyuanbaomall.cn/gtlyifsiyr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.andypj.xyz/gtuyvuxcil.html

TS:   同 JS
来源：http://hz.iojbl.cn/gtszhvnzpu.html

Java: 方法内为块级作用域
来源：http://hz.hongshengwenyu.top/gtkfhqtkwm.html

Go:   花括号块级作用域
来源：http://hz.yonumen.top/gtwsvjmzyh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ydzc1.top/gtwdsrodtl.html

C#:   块级作用域
来源：http://hz.tanke756.top/gtkzmoejea.html

[C11] 模块导入与导出
来源：http://hz.xinyue.icu/gtjwqcnltg.html

Py:   from module import func
来源：http://hz.yuanzhike.top/gtyqhcrfng.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtnuxxmjne.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dashuyun.cn/gtnacvcqea.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jyoumei.cn/gttxqevicc.html

Java: import java.util.List;
来源：http://hz.yj202588.top/gtryukjnjw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.9152youxi.cn/gthivpmhtk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sufxvd.cn/gtwxggwosd.html

C#:   using System.Text;
来源：http://hz.sysykeji.top/gtacokdhba.html

[C12] 立即执行函数 IIFE
来源：http://hz.ybcxt.top/gtykzuaytw.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gtjdspkxue.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtjbsmepsu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtjiqgasmb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtzjzgknyc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ydjk.org.cn/gtlcxijtfj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinghuilouyu.cn/gtrzcclolu.html

Ruby: -> { puts "run" }.call
来源：http://hz.yongpay.top/gtyugmpwzh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xylfe.cn/gtfgbjvvxc.html

[C13] 类型声明 / 类型注解
来源：http://hz.aizwys.cn/gttlolqocw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hywenlv.cn/gtplplufte.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtzctzazfs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guowangkeji.top/gtygmlkvnp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtsxbbmeou.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtesvrlqkl.html

Go:   func add(a, b int) int
来源：http://hz.xylfe.cn/gtramtpcsy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sysykeji.top/gtcrynwaax.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shanyushiyangkeji.top/gtrajgfkft.html

[C14] 泛型函数
来源：http://hz.meibo888.top/gtpyvdduyd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hysaishi.cn/gtkeefirpc.html

PHP:  // 无泛型
来源：http://hz.smart0.xyz/gtehizdign.html

JS:   // 无泛型
来源：http://hz.gaohongyu789.top/gtsufkywwe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgfzy.top/gtpbhawrca.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daxiang520.top/gthupjkbaa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtnpmatjjz.html

Ruby: # 无泛型
来源：http://hz.ybcxt.top/gtbcwbjvvr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xinyue.icu/gthlyexmiv.html

[C15] 解构 / 展开参数
来源：http://hz.jlsjyb.cn/gtbnfxukul.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nanxuanxn.top/gtutbkbkau.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxinkj.top/gtgjiamwjz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sufxvd.cn/gtgtcqhtit.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.smart0.xyz/gttxrmfzjv.html

Java: // 无解构
来源：http://hz.gzhubu.top/gtrltblohs.html

Go:   // 无解构
来源：http://hz.xinyue.icu/gtzlqqlqrh.html

Ruby: a, b = pair
来源：http://hz.meibo888.top/gtphsniizo.html

C#:   var (a, b) = pair;
来源：http://hz.shangyingyoupin.top/gtqkchbdcc.html

[C16] 函数 / 方法重载
来源：http://hz.52xcode.cn/gtvfbuobwt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.havefunace.top/gtcgueiypf.html

PHP:  // 无重载
来源：http://hz.dashuyun.cn/gtbfurolcf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gotoacloud.top/gtgopyocrv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.dianchejie.cn/gtqlmqpvpw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuanzx.com/gtmhdtmjeh.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydjk.org.cn/gttyonyjpb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guowangkeji.top/gtewsdjrmi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cashguo.top/gtnhoifjvy.html

================================================================================
来源：http://hz.9152youxi.cn/gtycgherpw.html

D. 数组 / 列表 / 集合
来源：http://hz.meibo888.top/gtbxvzybla.html

================================================================================
来源：http://hz.zhixingplan.top/gtiptmpqee.html

[D01] 创建数组 / 列表
来源：http://hz.gaohongyu789.top/gtkaylpggo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.pycfn.com/gtuckoivsn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sweek.top/gtkfrcyzct.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sxryk.cn/gturwmxonw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.52xcode.cn/gtnzlmakav.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.iojbl.cn/gtlkhbavfa.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cashguo.top/gtdrjplmfh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zycfv.cn/gtrifoxnjq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.andypj.xyz/gtcfuwiunn.html

[D02] 追加元素到末尾
来源：http://hz.ydzc1.top/gtpgpcxgrq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.andypj.xyz/gtkjwptyhu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhiwuduotai.top/gtnqlrcqiw.html

JS:   arr.push(4);
来源：http://hz.meibo888.top/gtooflvhfm.html

TS:   arr.push(4);
来源：http://hz.ivvv.top/gtpnkxuqmm.html

Java: list.add(4);
来源：http://hz.jinyuanbaomall.cn/gtdpabpstc.html

Go:   arr = append(arr, 4)
来源：http://hz.nwbrower.top/gtzhkayawb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daria6918.cn/gttvgnndxp.html

C#:   list.Add(4);
来源：http://hz.zdqjudy.top/gtkrsdiaut.html

[D03] 在指定位置插入元素
来源：http://hz.gzhubu.top/gtbjjyjvym.html

Py:   arr.insert(0, 0)
来源：http://hz.zhiwuduotai.top/gtyzzhhsgd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtrdmzhopt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shzxlz.cn/gtzzeidlip.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gaohongyu789.top/gtfftoeprt.html

Java: list.add(0, 0);
来源：http://hz.yj20258888.top/gtqhimlpuz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ehwqpu.com/gtutwevtig.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yvedp.cn/gtpieqkqui.html

C#:   list.Insert(0, 0);
来源：http://hz.yvedp.cn/gtisrscwws.html

[D04] 删除元素
来源：http://hz.hywenlv.cn/gtqmiqyxon.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhengqikj.top/gtzffiadda.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yueranfly.top/gtjljzqqxm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xinyue.icu/gtnjzzmtwq.html

TS:   arr.splice(0, 1);
来源：http://hz.daxiang520.top/gtuebtxskg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj20258888.top/gtfcqxnnoi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jlsjyb.cn/gtevjhoouk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fzhhl.top/gtoitsadek.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj202588.top/gteqpaikrb.html

[D05] 访问与修改元素
来源：http://hz.jqgfzy.top/gtpyjstlmw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtdbmctghz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.smart0.xyz/gtcwtvopig.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.52xcode.cn/gtxbjmdbje.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tanke756.top/gtbhllwbdm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ppjwa.cn/gtkrfqkilu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shuidangran.top/gtzgbasxfz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtfbncbaas.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj20258888.top/gtwsuzrxvq.html

[D06] 数组长度
来源：http://hz.smart0.xyz/gtviyhukab.html

Py:   len(arr)
来源：http://hz.ivvv.top/gtpgfejpop.html

PHP:  count($arr);
来源：http://hz.snrcjt.cn/gthprpplch.html

JS:   arr.length
来源：http://hz.daria6918.cn/gtbzharqxo.html

TS:   arr.length
来源：http://hz.yj20258888.top/gtzhqwiwfy.html

Java: list.size();
来源：http://hz.gogol.net.cn/gtvweaexvz.html

Go:   len(arr)
来源：http://hz.dianchejie.cn/gtjnxflfos.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtqjkulcpm.html

C#:   list.Count;
来源：http://hz.kuanghao11.cn/gtqisrcogr.html

[D07] 切片 / 取子数组
来源：http://hz.gotoacloud.top/gtltvkqwok.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hammf.cn/gtfebigbct.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.havefunace.top/gtqnroeubg.html

JS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gtmcvlvmwg.html

TS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtsqewziim.html

Java: list.subList(1, 4);
来源：http://hz.hnxiangtu.top/gtygkjgtfg.html

Go:   arr[1:4]
来源：http://hz.xziqi.cn/gtfkepyiij.html

Ruby: arr[1, 3]
来源：http://hz.snrcjt.cn/gtqftdlzfy.html

C#:   list.GetRange(1, 3);
来源：http://hz.aizwys.cn/gtaorfyjbi.html

[D08] 合并两个数组
来源：http://hz.cheryme.top/gtqkxepdgg.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinyuanbaomall.cn/gtnsfdgmzk.html

PHP:  array_merge($a, $b);
来源：http://hz.hnxiangtu.top/gtaoztypda.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aizwys.cn/gtjeszmzrg.html

TS:   [...a, ...b];
来源：http://hz.zhengqikj.top/gtuezazbjx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sysykeji.top/gtsulgvgtc.html

Go:   append(a, b...)
来源：http://hz.feifeiyinyue.top/gtjuhowwgb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ybcxt.top/gtsbgistvr.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtbusvsgee.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangkeji.top/gtfojedgsd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtvtrvbexm.html

PHP:  sort($arr);
来源：http://hz.sysykeji.top/gtjoayzqff.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtdsvmhvrd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj20258.top/gtooncxfrz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hysaishi.cn/gtrvcqgepk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.havefunace.top/gtpzxdnyit.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtfzcuckgy.html

C#:   list.Sort();
来源：http://hz.gaohongyu789.top/gtdswqqkel.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sysykeji.top/gtxajzczxz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cucudq.cn/gtxeugwyyh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtjwcpxleu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtherflang.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gtosmjqlzp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dashuyun.cn/gtomwhjhxr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigufen.top/gtfjzpineo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenzaomai.com/gtlaqcxfzs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jianghu66.top/gtuqmzxbgl.html

[D11] 反转数组
来源：http://hz.yueranfly.top/gtfmbhtqed.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnxiangtu.top/gtwgelwpef.html

PHP:  array_reverse($arr);
来源：http://hz.ywan-chungtsiang.top/gtcwvngaoh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jlsjyb.cn/gtnagyeqtj.html

TS:   [...arr].reverse();
来源：http://hz.yuxming.cn/gtdlsablek.html

Java: Collections.reverse(list);
来源：http://hz.0kj1m.cn/gttedilgkc.html

Go:   slices.Reverse(arr)
来源：http://hz.zhiwuduotai.top/gtzcsfshwp.html

Ruby: arr.reverse
来源：http://hz.cashguo.top/gtymhxnanh.html

C#:   list.Reverse();
来源：http://hz.ehwqpu.com/gtwuuzmhxv.html

[D12] 查找元素下标
来源：http://hz.wangshuangyany.cn/gttprdjwpx.html

Py:   arr.index(x);  x in arr
来源：http://hz.svipenyu.cn/gtavfsrrym.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtlbcarpka.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gtsxbmclgz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtalggwgyy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxinkj.top/gtixwpgvme.html

Go:   slices.Index(arr, x)
来源：http://hz.zhoulong.xyz/gtrpjbvzwg.html

Ruby: arr.index(x)
来源：http://hz.meibo888.top/gtvgtrtquc.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigufen.top/gttcymaqey.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydjk.org.cn/gtjnljrhxu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnqzz.top/gtievdbytr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtznegwaot.html

JS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gthnjaolei.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cucudq.cn/gtsonsmrcr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zdqjudy.top/gtuexvrloh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtzcljnksv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtrawyhkoe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.andypj.xyz/gtvelxcruo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cucudq.cn/gtnyykvkcq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258888.top/gtqtemskcd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nanxinkj.top/gtxuuujixh.html

JS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gtmzhsaibn.html

TS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gtunzmiztf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinqigufen.top/gtpvowkpne.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtigcaqlqs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hysaishi.cn/gtefrknjiy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhixingplan.top/gtxtdooznl.html

[D15] 去重
来源：http://hz.haohaochexian.top/gtndtukfmd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ppjwa.cn/gtkvopcvto.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtoytqfghl.html

JS:   [...new Set(arr)]
来源：http://hz.xuanzx.com/gtfzzznfat.html

TS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtycgssbgb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guannengcc.top/gtkyembmaj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuetiantiany.cn/gtpvqrfuii.html

Ruby: arr.uniq
来源：http://hz.wangshuangyany.cn/gtirlvdvgj.html

C#:   list.Distinct().ToList()
来源：http://hz.52xcode.cn/gtobdcpcut.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtdurazais.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dianchejie.cn/gtkevrvleg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.birdmap.top/gtxxchdvrc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ybcxt.top/gtawisjlcw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shangyingyoupin.top/gtezikxqke.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenzaomai.com/gtqenbtydy.html

Go:   // 手写循环累加
来源：http://hz.havefunace.top/gtjvguheky.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hywenlv.cn/gtwumhtimp.html

C#:   list.Sum();  list.Average()
来源：http://hz.daxiang520.top/gtkzerhprt.html

[D17] 最大值与最小值
来源：http://hz.guowangkeji.top/gtigxsviww.html

Py:   max(arr);  min(arr)
来源：http://hz.sufxvd.cn/gtqprgqbge.html

PHP:  max($arr);  min($arr);
来源：http://hz.zdqjudy.top/gtlayptrvu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zycfv.cn/gtvgnvkubl.html

TS:   Math.max(...arr);
来源：http://hz.dashuyun.cn/gtjzinouis.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nwbrower.top/gtkcmvbrgu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinyuanbaomall.cn/gtraehoqfm.html

Ruby: arr.max;  arr.min
来源：http://hz.pengpengdd.cyou/gtkkkpmotz.html

C#:   list.Max();  list.Min()
来源：http://hz.birdmap.top/gtaxbrxlsk.html

[D18] 扁平化嵌套数组
来源：http://hz.yuanzhike.top/gtqdrilppa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aibaodan.cn/gtnvdcpzxp.html

PHP:  array_merge(...$nested);
来源：http://hz.hammf.cn/gtotfleaam.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtsxjuhtbs.html

TS:   nested.flat();
来源：http://hz.hongshengwenyu.top/gtkxooafbq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangkeji.top/gtomgussiu.html

Go:   // 手写双层循环
来源：http://hz.xuanzx.com/gteoizopbk.html

Ruby: nested.flatten
来源：http://hz.shanyushiyangkeji.top/gtgawftpfx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shuidangran.top/gtjhajpbwi.html

[D19] 按字段分组
来源：http://hz.jyoumei.cn/gtmqlgwthj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.andypj.xyz/gtvtgzvuhc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnqzz.top/gtocsjjfbw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxinkj.top/gtnxakgppe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtkgbgbrvt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinyuanbaomall.cn/gteyqwnriy.html

Go:   // 手写 map[string][]T
来源：http://hz.andypj.xyz/gtdspbtoyv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yongpay.top/gtrtacceab.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.snrcjt.cn/gtbrplphtd.html

[D20] 统计每个元素出现次数
来源：http://hz.meibo888.top/gtnbbbhjjc.html

Py:   Counter(arr)
来源：http://hz.sufxvd.cn/gtsqrhspun.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtnzxmuamy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtwdxryfbg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gttjpoxtof.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hammf.cn/gtgfekomtk.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtaocykifi.html

Ruby: arr.tally
来源：http://hz.yonumen.top/gtigswgvtf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.316326.xyz/gtoorsatei.html

[D21] 判断是否包含某元素
来源：http://hz.jqgufenzy.top/gtzaimdqdx.html

Py:   x in arr
来源：http://hz.xuetiantiany.cn/gtciowrrwo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guowangkeji.top/gtswulnegs.html

JS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtlemuyuly.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtsnlnmzka.html

Java: list.contains(x)
来源：http://hz.aibaodan.cn/gtueerzuyf.html

Go:   slices.Contains(arr, x)
来源：http://hz.ydzc1.top/gtxzizspdb.html

Ruby: arr.include?(x)
来源：http://hz.ppjwa.cn/gtzemvocex.html

C#:   list.Contains(x)
来源：http://hz.ydjk.org.cn/gttbbrxoem.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ehwqpu.com/gtlhsivvqk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenjidiqi.icu/gtihevupcs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj20258888.top/gtzplgrbro.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenzaomai.com/gtgsfsvdkc.html

TS:   [...arr];
来源：http://hz.cdnleiting.top/gtsqlehkdw.html

Java: new ArrayList<>(list);
来源：http://hz.jinyuanbaomall.cn/gtlprqutxw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hywenlv.cn/gtsnsynxuw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yongpay.top/gtjreljmpu.html

C#:   new List<int>(list);
来源：http://hz.yuxming.cn/gtwoczifcn.html

[D23] reduce 累积计算
来源：http://hz.gaohongyu789.top/gtvubxvkng.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shzxlz.cn/gtslzsougj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hongshengwenyu.top/gtsmciyltc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.316326.xyz/gtiumhyxke.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtrrwwnlzk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yueranfly.top/gtxxqvafgn.html

Go:   // 手写循环
来源：http://hz.aibaodan.cn/gteeyteimq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gtxgefnydk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtvqzgzdmb.html

[D24] 字典 / Map 基本操作
来源：http://hz.dashuyun.cn/gtrlzxrsoh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yueranfly.top/gtuyeyblmu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ydjk.org.cn/gtzmvamaay.html


<!-- 参考信息 -->