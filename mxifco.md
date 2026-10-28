代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yanxiufei.cn/gtylzxenhr.html

[C07] 把函数作为参数传入
来源：http://hz.jqgufenzy.top/gtmzouxymz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fengsongda.top/gtdxueeton.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dianchejie.cn/gtsbytqceg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.birdmap.top/gtdpbuuryr.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangkeji.top/gtzyjrjfoj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangtech.top/gtqllncssq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtvupakhxo.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtmuwosslx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhengqikj.top/gtprtzcwmg.html

[C08] 闭包
来源：http://hz.hfpthk.cn/gtwuilxjgz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hnxiangtu.top/gteocalwmj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.0kj1m.cn/gtnujngzzr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtwiuuekws.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtwwqwichn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.dashuyun.cn/gtjgptipwj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gtcytmyczb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenzaomai.com/gttazojzfh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gthozprvxx.html

[C09] 递归
来源：http://hz.cashguo.top/gtvadixpye.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtsderensk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cheryme.top/gtaswrxdux.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.andypj.xyz/gtdbriwjdq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtgagdewzv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgufenzy.top/gtfpvsunuk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yvedp.cn/gtykffukkl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xinyue.icu/gtqjlsazmq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhijiandao.cn/gtvxkkzqsa.html

[C10] 变量作用域
来源：http://hz.nanxuanxn.top/gtbbozoywy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shuidangran.top/gtlqpbrslf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhongyouzk.top/gtvfxcbvic.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtyzutevna.html

TS:   同 JS
来源：http://hz.guannengcc.top/gtvfekuwlv.html

Java: 方法内为块级作用域
来源：http://hz.c1oappe.top/gtcsdkkpzv.html

Go:   花括号块级作用域
来源：http://hz.yanxiufei.cn/gtxifxgjeh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.andypj.xyz/gthjfjvpbk.html

C#:   块级作用域
来源：http://hz.yangfankeji.com/gtmxafudps.html

[C11] 模块导入与导出
来源：http://hz.dashuyun.cn/gtsibofjgy.html

Py:   from module import func
来源：http://hz.hammf.cn/gtslnhjnjs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xingfuxueyuan.xyz/gtxyobppdc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pycfn.com/gtzzkdfnzr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yonumen.top/gtrdxxyzbj.html

Java: import java.util.List;
来源：http://hz.birdmap.top/gttbsmjksx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jyoumei.cn/gtpnaaztam.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.meibo888.top/gtnfcplnrk.html

C#:   using System.Text;
来源：http://hz.shanyushiyangkeji.top/gtxadsdnsg.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuetiantiany.cn/gtopqhbfrj.html

Py:   (lambda: print("run"))()
来源：http://hz.yuanzhike.top/gtixblladu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhixingplan.top/gtosjyrugo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gthlyobopd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtnkmcvath.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daria6918.cn/gttqwzuzic.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hammf.cn/gtcqwitiuo.html

Ruby: -> { puts "run" }.call
来源：http://hz.gaohongyu789.top/gtplfscyjp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenjidiqi.icu/gtnjchjdeh.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhaomingkeji.xyz/gtujhrapkj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cucudq.cn/gtoamnclfq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtvzytgosc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zycfv.cn/gtgawkydqh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jianghu66.top/gtvudwfqyz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtbfxbsaxw.html

Go:   func add(a, b int) int
来源：http://hz.nwbrower.top/gtxkvlzxbz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.feifeiyinyue.top/gtnhfvebeu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ywan-chungtsiang.top/gthuoairvc.html

[C14] 泛型函数
来源：http://hz.redwolf501.top/gtceladzvs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ehwqpu.com/gtalybfpnk.html

PHP:  // 无泛型
来源：http://hz.feifeiyinyue.top/gtwdmovxoa.html

JS:   // 无泛型
来源：http://hz.zhongyouzk.top/gtjpimnrwh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dashuyun.cn/gtmaapohpa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.iojbl.cn/gthsmdlcqc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gogol.net.cn/gtxjhewczr.html

Ruby: # 无泛型
来源：http://hz.zhixingplan.top/gtdeunqnlu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangdashe.top/gtxtemswpt.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtzlaycqfj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.svipenyu.cn/gtgdqhzjdj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhiwuduotai.top/gtvzxgjauf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gthuihurqq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zdqjudy.top/gtkosptfmc.html

Java: // 无解构
来源：http://hz.mhx1999.top/gtrvhtsoso.html

Go:   // 无解构
来源：http://hz.yongpay.top/gtvnajpall.html

Ruby: a, b = pair
来源：http://hz.ydzc1.top/gtodzatbmm.html

C#:   var (a, b) = pair;
来源：http://hz.yj20258888.top/gtxafztejt.html

[C16] 函数 / 方法重载
来源：http://hz.andypj.xyz/gtascmehjo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinyuanbaomall.cn/gtteqvrnfz.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gtxwmiixeb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cheryme.top/gttjidazsk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cheryme.top/gtnctnnwdh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shangyingyoupin.top/gtvlkafdap.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgfzy.top/gtmilswozp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sxryk.cn/gtrhwujete.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangkeji.top/gtqpltnpht.html

================================================================================
来源：http://hz.daxiang520.top/gtflofhcka.html

D. 数组 / 列表 / 集合
来源：http://hz.hysaishi.cn/gtcxljbrdk.html

================================================================================
来源：http://hz.xylfe.cn/gtwrykhtgi.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtlfentlrc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.kuanghao11.cn/gtqoujmguq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hywenlv.cn/gtejwyzqur.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhixingplan.top/gtpaigjkon.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ydzc1.top/gtdmnglkki.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigufen.top/gtzwawowgc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinyuanbaomall.cn/gtwzuieduz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.c1oappe.top/gtpstzcrhe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xingfuxueyuan.xyz/gtvgjukyyz.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtgagiyfnk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigfzy.top/gtwtyveuax.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xziqi.cn/gtsbgzowlu.html

JS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtaxadgmqx.html

TS:   arr.push(4);
来源：http://hz.xziqi.cn/gttbyzcgaz.html

Java: list.add(4);
来源：http://hz.jqgufenzy.top/gtffyudlpi.html

Go:   arr = append(arr, 4)
来源：http://hz.yangfankeji.com/gtcffosrsu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ydjk.org.cn/gtzjdvbiid.html

C#:   list.Add(4);
来源：http://hz.ydjk.org.cn/gtnggugcaj.html

[D03] 在指定位置插入元素
来源：http://hz.xziqi.cn/gtrhgxmfav.html

Py:   arr.insert(0, 0)
来源：http://hz.tian-w.cn/gtrfozwfhz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gaohongyu789.top/gtbbxcpdal.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yonumen.top/gtpdusqzwc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hfpthk.cn/gtjzokgdvs.html

Java: list.add(0, 0);
来源：http://hz.xuanzx.com/gthbsbfuvu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yueranfly.top/gtaffeqtsu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zycfv.cn/gtnkrbcpxf.html

C#:   list.Insert(0, 0);
来源：http://hz.hysaishi.cn/gtlfmaoxoh.html

[D04] 删除元素
来源：http://hz.smart0.xyz/gtwchgrnht.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydjk.org.cn/gtpmcehalh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.9152youxi.cn/gtafllmzdv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.0kj1m.cn/gtdklfnckx.html

TS:   arr.splice(0, 1);
来源：http://hz.guannengcc.top/gtnsxaxryd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nwbrower.top/gtnotcgzrd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cucudq.cn/gtikavrkdj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aibaodan.cn/gtcakkjcvg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.c1oappe.top/gtswggukss.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gtewwndhdy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtmcthhnir.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.smart0.xyz/gtkheudwvz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.mhx1999.top/gtnjzlyloi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hysaishi.cn/gtraqrkvre.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtefkcmuab.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.316326.xyz/gtsefsodxj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtgcgsyizl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtbogresmd.html

[D06] 数组长度
来源：http://hz.xylfe.cn/gtpfvairhk.html

Py:   len(arr)
来源：http://hz.sweek.top/gtxhtlmtir.html

PHP:  count($arr);
来源：http://hz.zhixingplan.top/gtojyztpmd.html

JS:   arr.length
来源：http://hz.chenzaomai.com/gtljmiecwd.html

TS:   arr.length
来源：http://hz.gzhubu.top/gtocowdwbz.html

Java: list.size();
来源：http://hz.jyoumei.cn/gtgjkldpne.html

Go:   len(arr)
来源：http://hz.jqgufenzy.top/gtfoangwkp.html

Ruby: arr.length; arr.size
来源：http://hz.gogol.net.cn/gtrzayuksr.html

C#:   list.Count;
来源：http://hz.jqgfzy.top/gtlidakaqs.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gtasmyreob.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yanxiufei.cn/gtdedsfcnw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ybcxt.top/gtgsggccvd.html

JS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtduukrwik.html

TS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtckhortoq.html

Java: list.subList(1, 4);
来源：http://hz.ivvv.top/gtvbdkawma.html

Go:   arr[1:4]
来源：http://hz.jinghuilouyu.cn/gtzqpooirr.html

Ruby: arr[1, 3]
来源：http://hz.wangshuangyany.cn/gtltxomcjo.html

C#:   list.GetRange(1, 3);
来源：http://hz.sxryk.cn/gtvlzbqrkl.html

[D08] 合并两个数组
来源：http://hz.ppjwa.cn/gttpdpqvst.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuxming.cn/gtdletcsnc.html

PHP:  array_merge($a, $b);
来源：http://hz.9152youxi.cn/gttncwixkz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhengqikj.top/gtkhqeudzu.html

TS:   [...a, ...b];
来源：http://hz.yangfankeji.com/gtmpitqeec.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.feifeiyinyue.top/gtxzyivlpt.html

Go:   append(a, b...)
来源：http://hz.9152youxi.cn/gtqlwxfkdw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.smart0.xyz/gttsohemhm.html

C#:   a.Concat(b).ToList()
来源：http://hz.cheryme.top/gtlulosgfy.html

[D09] 排序（升序）
来源：http://hz.guannengcc.top/gtozsbbgyn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtpntixeym.html

PHP:  sort($arr);
来源：http://hz.dashuyun.cn/gtieprmdil.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gotoacloud.top/gtfeferkik.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.0kj1m.cn/gtxppojrtf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.feifeiyinyue.top/gtyvpqqpqk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtuqnopdvf.html

Ruby: arr.sort
来源：http://hz.havefunace.top/gtfuwpuefm.html

C#:   list.Sort();
来源：http://hz.ppjwa.cn/gthnlkuepp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.mhx1999.top/gtvkmjjuen.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guannengcc.top/gtgkflxklm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtojabodrz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.svipenyu.cn/gtncpxbvnd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xinyue.icu/gtuswooizk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fengsongda.top/gtkvzktlva.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yangfankeji.com/gtdfashvyz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gteltipwst.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ybcxt.top/gtelffznod.html

[D11] 反转数组
来源：http://hz.nanxinkj.top/gtksgukbft.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.mhx1999.top/gtlpuirrzz.html

PHP:  array_reverse($arr);
来源：http://hz.hnqzz.top/gtilfmvzog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.wangdashe.top/gttecdkaxn.html

TS:   [...arr].reverse();
来源：http://hz.jinyuanbaomall.cn/gtoxwlyeeb.html

Java: Collections.reverse(list);
来源：http://hz.ehwqpu.com/gtjhmvbytv.html

Go:   slices.Reverse(arr)
来源：http://hz.daria6918.cn/gtfftdgtna.html

Ruby: arr.reverse
来源：http://hz.jinghuilouyu.cn/gtylyrfanr.html

C#:   list.Reverse();
来源：http://hz.mhx1999.top/gtdgfzlavx.html

[D12] 查找元素下标
来源：http://hz.yanxiufei.cn/gtahpaeimr.html

Py:   arr.index(x);  x in arr
来源：http://hz.0kj1m.cn/gtlwjlvjae.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dashuyun.cn/gttkapeauv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtieutuhkl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtbgmkrako.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pycfn.com/gtrdfvxyje.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gtqdnouojj.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtjwzouixa.html

C#:   list.IndexOf(x);
来源：http://hz.c1oappe.top/gtjntixgmc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tianlin.xyz/gtbcrcdaec.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.snrcjt.cn/gtqauxxokr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuxming.cn/gthwgozpxj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtzpkgtctw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtekhbzbkd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aizwys.cn/gtvvbhoilf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhengqikj.top/gthnibmlkp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.birdmap.top/gtogjdckos.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jianghu66.top/gtzhrtonny.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhongyouzk.top/gtnkrzkqnf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258888.top/gtprafwzhg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.andypj.xyz/gtczebrtwk.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtrlolpzzh.html

TS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtlonuzvms.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shzxlz.cn/gtokervwgr.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtxvzwlfye.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hysaishi.cn/gtdqsuzhjq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yueranfly.top/gtwshlatbc.html

[D15] 去重
来源：http://hz.cheryme.top/gtkikqewdf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtgqnnpssh.html

PHP:  array_unique($arr);
来源：http://hz.snrcjt.cn/gtrxjymscs.html

JS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtpczoqdox.html

TS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtzttjksjz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gtpssqayif.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangshuangyany.cn/gtcndkfuqa.html

Ruby: arr.uniq
来源：http://hz.yangfankeji.com/gtrzmqrsaj.html

C#:   list.Distinct().ToList()
来源：http://hz.haohaochexian.top/gtzwkjcpqv.html

[D16] 求和与平均值
来源：http://hz.gogol.net.cn/gthnufgush.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.snrcjt.cn/gtznimsinh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhiwuduotai.top/gtuotczydl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtfowcaezj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtxyxvbjlf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtvoglelaq.html

Go:   // 手写循环累加
来源：http://hz.gogol.net.cn/gtzszlqaxf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jlsjyb.cn/gtlobkqoeh.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258888.top/gtfwruqvto.html

[D17] 最大值与最小值
来源：http://hz.jqgufenzy.top/gtytzlwsxk.html

Py:   max(arr);  min(arr)
来源：http://hz.guannengcc.top/gttauqbhst.html

PHP:  max($arr);  min($arr);
来源：http://hz.xziqi.cn/gtfkzcqfks.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zdqjudy.top/gtkkrpreug.html

TS:   Math.max(...arr);
来源：http://hz.quarkkingdee.top/gtxpwrflhh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gttsauzquz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.meibo888.top/gtkaqcbwjr.html

Ruby: arr.max;  arr.min
来源：http://hz.yj202588.top/gtzzgnzyzk.html

C#:   list.Max();  list.Min()
来源：http://hz.zhoulong.xyz/gtxxqrgagj.html

[D18] 扁平化嵌套数组
来源：http://hz.daria6918.cn/gtuzjmljrg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenzaomai.com/gtfdpcfgva.html

PHP:  array_merge(...$nested);
来源：http://hz.jinyuanbaomall.cn/gtkdrudvtl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuanzhike.top/gtokejkkrd.html

TS:   nested.flat();
来源：http://hz.sufxvd.cn/gtlfdffgda.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenlongwang.top/gtwsdbcjlr.html

Go:   // 手写双层循环
来源：http://hz.ivvv.top/gtcxylnhto.html

Ruby: nested.flatten
来源：http://hz.wangdashe.top/gtzakyvbpa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.havefunace.top/gtcxntqdtw.html

[D19] 按字段分组
来源：http://hz.jlsjyb.cn/gttigrfbcg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yueranfly.top/gtjozuttmv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.kuanghao11.cn/gtzzfkejym.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gtvxwqimam.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gtpdgneixo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj202588.top/gtdtowtwck.html

Go:   // 手写 map[string][]T
来源：http://hz.yanxiufei.cn/gtypmtapan.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xylfe.cn/gtbzspfhyi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gtpboyxsqv.html

[D20] 统计每个元素出现次数
来源：http://hz.ywan-chungtsiang.top/gtfenunpwt.html

Py:   Counter(arr)
来源：http://hz.yongpay.top/gtlltnesgf.html

PHP:  array_count_values($arr);
来源：http://hz.zhengqikj.top/gtoiesdvmh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gthkcfoynk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtzbbofsae.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hammf.cn/gtccjjltvq.html

Go:   // 手写 map[T]int
来源：http://hz.ywan-chungtsiang.top/gtujszfepd.html

Ruby: arr.tally
来源：http://hz.yueranfly.top/gtuvahbpvt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ydjk.org.cn/gtgeabggwb.html

[D21] 判断是否包含某元素
来源：http://hz.haohaochexian.top/gtajjrxxdd.html

Py:   x in arr
来源：http://hz.sysykeji.top/gtdkblsfkc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hammf.cn/gtjykljjgw.html

JS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtktnkqndn.html

TS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gttxuxjebm.html

Java: list.contains(x)
来源：http://hz.daxiang520.top/gtyvqxhhxz.html

Go:   slices.Contains(arr, x)
来源：http://hz.yonumen.top/gtzmslfxhq.html

Ruby: arr.include?(x)
来源：http://hz.zhaomingkeji.xyz/gtmfzeceoh.html

C#:   list.Contains(x)
来源：http://hz.nwbrower.top/gtksblmdhy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xinyue.icu/gtsaftotah.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenzaomai.com/gtigtveknz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hammf.cn/gtdgbrdcqx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.0kj1m.cn/gtzjouwvan.html

TS:   [...arr];
来源：http://hz.bjfxy.top/gtesedqtpx.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtztfwojtm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.iojbl.cn/gtwpfkrovt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fzhhl.top/gttbnqbbtj.html

C#:   new List<int>(list);
来源：http://hz.sysykeji.top/gtqbxtasaj.html

[D23] reduce 累积计算
来源：http://hz.yuanzhike.top/gtcilkapsq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtmgdezslr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhijiandao.cn/gtainspuep.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gtndbjgwfx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtsppzdehf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtjhqjyayr.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtuqjvskie.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.andypj.xyz/gtpagoaewc.html


<!-- 参考信息 -->