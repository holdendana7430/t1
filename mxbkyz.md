代发 wailian999

C#:   块级作用域
来源：http://hz.hfpthk.cn/gtslyypugz.html

[C11] 模块导入与导出
来源：http://hz.guannengcc.top/gtmrecoqzx.html

Py:   from module import func
来源：http://hz.gzhubu.top/gthdmkqnbm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cqqwz.cn/gtwckgkwhm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinqigfzy.top/gtpztlrprk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.meibo888.top/gtfibkkttg.html

Java: import java.util.List;
来源：http://hz.yueranfly.top/gttskpqlkt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhongyouzk.top/gtbwuarjeu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tian-w.cn/gtoefrmicx.html

C#:   using System.Text;
来源：http://hz.yangfankeji.com/gtikrkodcq.html

[C12] 立即执行函数 IIFE
来源：http://hz.cdnleiting.top/gtyipnapnp.html

Py:   (lambda: print("run"))()
来源：http://hz.gaohongyu789.top/gtjhjkpbtr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ybcxt.top/gtnvifksmw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gtqrqytzcf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtjykzites.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sysykeji.top/gtrfvkxxgr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenjidiqi.icu/gtxidfukel.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhongyouzk.top/gtdqpdtmlw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yangfankeji.com/gtpfjwauqh.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuanzx.com/gtgfmluqky.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zdqjudy.top/gtrkttqljr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtxjyqtoik.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shuidangran.top/gtyngimrgo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ppjwa.cn/gtqmkojirk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtteluqlgn.html

Go:   func add(a, b int) int
来源：http://hz.xuetiantiany.cn/gtndptvdmo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gtywobjhml.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinyuanbaomall.cn/gtplklerut.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtlenjbopi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yonumen.top/gtksdjhgze.html

PHP:  // 无泛型
来源：http://hz.jqgfzy.top/gtyibcwsvu.html

JS:   // 无泛型
来源：http://hz.tanke756.top/gtpndascfx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.quarkkingdee.top/gtvviintuj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.quarkkingdee.top/gtkibdzyvf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dashuyun.cn/gttnkzogwl.html

Ruby: # 无泛型
来源：http://hz.xuetiantiany.cn/gtpjbhvgeu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gotoacloud.top/gtmgdjdeny.html

[C15] 解构 / 展开参数
来源：http://hz.yueranfly.top/gtiusfjotq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xylfe.cn/gtpeglymvz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pycfn.com/gtqpchmohp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gtpigdjdvl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guannengcc.top/gtsrqyzbrg.html

Java: // 无解构
来源：http://hz.guowangkeji.top/gtqdxtucoe.html

Go:   // 无解构
来源：http://hz.wangdashe.top/gtwsxcpxte.html

Ruby: a, b = pair
来源：http://hz.iojbl.cn/gtlsmlibyy.html

C#:   var (a, b) = pair;
来源：http://hz.tianlin.xyz/gtbwghyooi.html

[C16] 函数 / 方法重载
来源：http://hz.gotoacloud.top/gtesrhlrce.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guannengcc.top/gtrvztgwgz.html

PHP:  // 无重载
来源：http://hz.hnqzz.top/gtwigduune.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cashguo.top/gtyuwsrmbe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cashguo.top/gtmssrhptc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinqigfzy.top/gtgpeynfkm.html

Go:   // 无重载：用不同函数名
来源：http://hz.0kj1m.cn/gtfckkfmjq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuxming.cn/gtssutiuld.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ybcxt.top/gtjoodlhrm.html

================================================================================
来源：http://hz.tian-w.cn/gtkewswgnv.html

D. 数组 / 列表 / 集合
来源：http://hz.zhiwuduotai.top/gtcdrfnamt.html

================================================================================
来源：http://hz.mhx1999.top/gtoftlxirj.html

[D01] 创建数组 / 列表
来源：http://hz.ybcxt.top/gtkyiyjnpq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nwbrower.top/gtxinxbgts.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gogol.net.cn/gtwkpikzkw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtrueyetzs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dashuyun.cn/gtqfrfacuj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xziqi.cn/gtyoisjqvn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jianghu66.top/gtzuremkpx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gtfnuqwvnc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gotoacloud.top/gtodjfmgnt.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gteenteidc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hnxiangtu.top/gtlrhzaqwr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xziqi.cn/gtyqvlpxcr.html

JS:   arr.push(4);
来源：http://hz.tian-w.cn/gtbfwieroy.html

TS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtzflgnkrg.html

Java: list.add(4);
来源：http://hz.hongshengwenyu.top/gtoevrjsld.html

Go:   arr = append(arr, 4)
来源：http://hz.smart0.xyz/gtvtnhetwj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.svipenyu.cn/gtzqdzoqka.html

C#:   list.Add(4);
来源：http://hz.sxryk.cn/gtddpnveul.html

[D03] 在指定位置插入元素
来源：http://hz.jlsjyb.cn/gtbrzajuse.html

Py:   arr.insert(0, 0)
来源：http://hz.zhengqikj.top/gtsixbbuzi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hywenlv.cn/gtkbngsobi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.quarkkingdee.top/gtpkltrilk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yvedp.cn/gtqgvsfspj.html

Java: list.add(0, 0);
来源：http://hz.mhx1999.top/gtelfavjzd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shuidangran.top/gtecmkkosq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yueranfly.top/gtaxinfwft.html

C#:   list.Insert(0, 0);
来源：http://hz.shzxlz.cn/gtwwhylshl.html

[D04] 删除元素
来源：http://hz.sysykeji.top/gtfhpmpcwi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fengsongda.top/gtgryiqpkm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aibaodan.cn/gtwaevuokn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenjidiqi.icu/gtbeelfeni.html

TS:   arr.splice(0, 1);
来源：http://hz.aizwys.cn/gtzupvepwq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj202588.top/gtatatbqct.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gtvfvfacjv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guannengcc.top/gtorwqkqpc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xziqi.cn/gtfvjczebk.html

[D05] 访问与修改元素
来源：http://hz.yongpay.top/gtqsmssihd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtvwemxpax.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guowangkeji.top/gtkvtwyqmn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hammf.cn/gtrngxzlun.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shzxlz.cn/gtlwxdatxt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj202588.top/gtlztujfvr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuanzx.com/gtohivguws.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gttobznelj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zdqjudy.top/gtqlcmhtty.html

[D06] 数组长度
来源：http://hz.jiagoushi.top/gtkveppmhn.html

Py:   len(arr)
来源：http://hz.shuidangran.top/gtopgvjovo.html

PHP:  count($arr);
来源：http://hz.hfpthk.cn/gtgaemlhwb.html

JS:   arr.length
来源：http://hz.shzxlz.cn/gtyfphvihz.html

TS:   arr.length
来源：http://hz.yuanzhike.top/gtdnabrzyu.html

Java: list.size();
来源：http://hz.sysykeji.top/gtmbrphbvj.html

Go:   len(arr)
来源：http://hz.xylfe.cn/gtwwlaezpm.html

Ruby: arr.length; arr.size
来源：http://hz.tian-w.cn/gtilrerxvk.html

C#:   list.Count;
来源：http://hz.havefunace.top/gtetyseiqo.html

[D07] 切片 / 取子数组
来源：http://hz.hammf.cn/gtmabpsxbh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zdqjudy.top/gtvrpphsre.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gzhubu.top/gtmxtisbhx.html

JS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtrdzdkyoy.html

TS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtxplqxypp.html

Java: list.subList(1, 4);
来源：http://hz.zhongyouzk.top/gtqrizltdk.html

Go:   arr[1:4]
来源：http://hz.tianlin.xyz/gtonrrrfgx.html

Ruby: arr[1, 3]
来源：http://hz.mhx1999.top/gthiyndnzi.html

C#:   list.GetRange(1, 3);
来源：http://hz.hysaishi.cn/gtcjirgyoz.html

[D08] 合并两个数组
来源：http://hz.hongshengwenyu.top/gthopoziqe.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gtyjzlltlj.html

PHP:  array_merge($a, $b);
来源：http://hz.ppjwa.cn/gttcskyitx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhijiandao.cn/gtlqrpqpzt.html

TS:   [...a, ...b];
来源：http://hz.cucudq.cn/gtdqxbshjq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.wangshuangyany.cn/gtmwfxozbz.html

Go:   append(a, b...)
来源：http://hz.xuetiantiany.cn/gtznpgwrxz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hnqzz.top/gtebzmqhqx.html

C#:   a.Concat(b).ToList()
来源：http://hz.nanxuanxn.top/gtjrlrcxcz.html

[D09] 排序（升序）
来源：http://hz.yongpay.top/gteupmugnm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhiwuduotai.top/gtlspyqmce.html

PHP:  sort($arr);
来源：http://hz.shzxlz.cn/gtjiqyfxln.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sxryk.cn/gtswwfddxq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jianghu66.top/gtdlyevfcg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cucudq.cn/gtvidymshp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtslcdupog.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtijhipauc.html

C#:   list.Sort();
来源：http://hz.smart0.xyz/gtqwilvsdn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gtdwyyrszv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhoulong.xyz/gtlqzuabhc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daria6918.cn/gtgnvsrowr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtfeqevdtz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtsqavfzgl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuxming.cn/gtzdltolhl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.vqdsnc.cn/gtbuhyjwyd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gtfmmtiuov.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tian-w.cn/gttufnnvji.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gtcxwetxvw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yangfankeji.com/gtiujjezgq.html

PHP:  array_reverse($arr);
来源：http://hz.cucudq.cn/gtbhavygxa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cdnleiting.top/gtsubyshyd.html

TS:   [...arr].reverse();
来源：http://hz.shanyushiyangtech.top/gtdlhzvpnm.html

Java: Collections.reverse(list);
来源：http://hz.yuxming.cn/gtfmgjpwfr.html

Go:   slices.Reverse(arr)
来源：http://hz.jianghu66.top/gtquqkobbo.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtnngryldn.html

C#:   list.Reverse();
来源：http://hz.zdqjudy.top/gtbpbxlxsq.html

[D12] 查找元素下标
来源：http://hz.wangshuangyany.cn/gtqubwltih.html

Py:   arr.index(x);  x in arr
来源：http://hz.hywenlv.cn/gtcyywrpyl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydzc1.top/gtittribkr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gtzavfrtmz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtgpbctqed.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydzc1.top/gtxkwlnczo.html

Go:   slices.Index(arr, x)
来源：http://hz.ppjwa.cn/gtqpahvcnk.html

Ruby: arr.index(x)
来源：http://hz.chenzaomai.com/gtvrtgmhzw.html

C#:   list.IndexOf(x);
来源：http://hz.hfpthk.cn/gtqpcvwjza.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtjfxzhdzj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinqigfzy.top/gtowcnrpmr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinyuanbaomall.cn/gtkzjsdxqw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtpftsaqzt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtgvgtakno.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fengsongda.top/gtjsqmfnkt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.birdmap.top/gtefhtaumc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sufxvd.cn/gtncyafxxk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.svipenyu.cn/gtdygakqkw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zdqjudy.top/gtmrjsfdkn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ywan-chungtsiang.top/gtpprpiwsf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pengpengdd.cyou/gthhlnevyn.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinqigufen.top/gtbxhwbleu.html

TS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtbtiqbamx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sysykeji.top/gtiksziefl.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtvxvvoxsf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shuidangran.top/gtxkueayxb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtyuxdrepp.html

[D15] 去重
来源：http://hz.xinyue.icu/gtvmllserq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.9152youxi.cn/gtlioullij.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gtcqretdcq.html

JS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtgbuagucr.html

TS:   [...new Set(arr)]
来源：http://hz.gzhubu.top/gtlwsmxxjh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dashuyun.cn/gtcmjwyagp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtnpdcbygi.html

Ruby: arr.uniq
来源：http://hz.zhongyouzk.top/gtwsdyuysu.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gtpifvbadn.html

[D16] 求和与平均值
来源：http://hz.gotoacloud.top/gtpgvovzyb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.bjfxy.top/gthkhavyyy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhiwuduotai.top/gtoionvhrx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhaomingkeji.xyz/gtyojsqnwf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtlbeahcsz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.9152youxi.cn/gtiwpmoofi.html

Go:   // 手写循环累加
来源：http://hz.ybcxt.top/gtbchgmidw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ybcxt.top/gteicdzjba.html

C#:   list.Sum();  list.Average()
来源：http://hz.c1oappe.top/gtgzjypisj.html

[D17] 最大值与最小值
来源：http://hz.nanxuanxn.top/gttkdeqoqq.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtdtcinwtw.html

PHP:  max($arr);  min($arr);
来源：http://hz.hammf.cn/gtbwqeudlz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.c1oappe.top/gtgvvybvsd.html

TS:   Math.max(...arr);
来源：http://hz.ydjk.org.cn/gtwavozxmy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.meibo888.top/gtfycoyusu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hongshengwenyu.top/gtzspkrezx.html

Ruby: arr.max;  arr.min
来源：http://hz.zhengqikj.top/gtsgvatfjy.html

C#:   list.Max();  list.Min()
来源：http://hz.ywan-chungtsiang.top/gtuupjjble.html

[D18] 扁平化嵌套数组
来源：http://hz.zhoulong.xyz/gtgsfnfwet.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ywan-chungtsiang.top/gthvlflyql.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258.top/gtfsydtbzn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinyuanbaomall.cn/gttapbvkhj.html

TS:   nested.flat();
来源：http://hz.snrcjt.cn/gtcbqaxqbd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.redwolf501.top/gtoauxdxhi.html

Go:   // 手写双层循环
来源：http://hz.chenlongwang.top/gturkifeiy.html

Ruby: nested.flatten
来源：http://hz.mhx1999.top/gtyxnadebx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ehwqpu.com/gtbckdgbzx.html

[D19] 按字段分组
来源：http://hz.wangshuangyany.cn/gtnaeptgib.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuanzx.com/gtptflsziv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.havefunace.top/gtajnjsiqq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fzhhl.top/gtmteftuuk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gtbqaxniah.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtpprefqtx.html

Go:   // 手写 map[string][]T
来源：http://hz.jiagoushi.top/gtolqcgfhx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangkeji.top/gtvrnrapck.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dashuyun.cn/gtylthhtpd.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gtamvhcjmj.html

Py:   Counter(arr)
来源：http://hz.shangyingyoupin.top/gthupqduqa.html

PHP:  array_count_values($arr);
来源：http://hz.kuanghao11.cn/gtfxanagxr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtbqqjgglx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuanzx.com/gtjozvegsi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.316326.xyz/gtamqdgcgh.html

Go:   // 手写 map[T]int
来源：http://hz.vqdsnc.cn/gthzkdsjls.html

Ruby: arr.tally
来源：http://hz.yonumen.top/gtaiaeeevf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yangfankeji.com/gtypgmsmvn.html

[D21] 判断是否包含某元素
来源：http://hz.haohaochexian.top/gtfsrgqvdx.html

Py:   x in arr
来源：http://hz.zhaomingkeji.xyz/gticarijqj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.52xcode.cn/gtpchmzjgs.html

JS:   arr.includes(x)
来源：http://hz.bjfxy.top/gtttfxoffr.html

TS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtrydqtqmw.html

Java: list.contains(x)
来源：http://hz.52xcode.cn/gtetljbkae.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gtktkxpkhk.html

Ruby: arr.include?(x)
来源：http://hz.fengsongda.top/gtmtokmroq.html

C#:   list.Contains(x)
来源：http://hz.pengpengdd.cyou/gtwsmkibja.html

[D22] 复制数组（避免共享引用）
来源：http://hz.316326.xyz/gtpkmrohsz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuanzhike.top/gtjchbaoed.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ydzc1.top/gtodgdukoq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sysykeji.top/gtolrdqoqy.html

TS:   [...arr];
来源：http://hz.feifeiyinyue.top/gtfzrtoufg.html

Java: new ArrayList<>(list);
来源：http://hz.yuxming.cn/gtklvlclnm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shangyingyoupin.top/gtjyrmnaeb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj202588.top/gtkljezdqb.html

C#:   new List<int>(list);
来源：http://hz.hammf.cn/gtckhgzznk.html

[D23] reduce 累积计算
来源：http://hz.cashguo.top/gtqcinogxz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigfzy.top/gtkffpqzow.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yonumen.top/gthdcsqulg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gtxptxthxg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xingfuxueyuan.xyz/gtdtqlsvjj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daxiang520.top/gtootwtbco.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gttpcvomaw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ppjwa.cn/gtuovatblk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gtlfbxiftb.html

[D24] 字典 / Map 基本操作
来源：http://hz.smart0.xyz/gthwqcobds.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.smart0.xyz/gtekjvpsfm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hammf.cn/gtubpywhyl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gthpiydvwr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.pycfn.com/gtlqhmjmrq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuetiantiany.cn/gthvzprwtf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhengqikj.top/gtrrflcjpb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.snrcjt.cn/gtjnofzuwi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuanzx.com/gtrnglouza.html

[D25] Set 集合去重与交并差
来源：http://hz.kuanghao11.cn/gtdgxvmhng.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnqzz.top/gtczfojygk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.svipenyu.cn/gtpcyqseoz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.9152youxi.cn/gtrgcahwuo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hnqzz.top/gtvrantgth.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.birdmap.top/gtmtucqyla.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aizwys.cn/gtbrfzrisy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtccvqyfux.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuanzx.com/gtmunbkofp.html

[D26] 数组转字符串
来源：http://hz.fengsongda.top/gtghtitgdw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.smart0.xyz/gtvcnyjlwu.html

PHP:  implode(", ", $arr);
来源：http://hz.hongshengwenyu.top/gtrfmxceku.html

JS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtuqdzkejj.html

TS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtcgjckywe.html

Java: String.join(", ", list)
来源：http://hz.cheryme.top/gtemyffhye.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gotoacloud.top/gtthhpqife.html

Ruby: arr.join(", ")
来源：http://hz.0kj1m.cn/gtgkisxamy.html

C#:   string.Join(", ", list)
来源：http://hz.zhixingplan.top/gtinqdoblm.html

================================================================================
来源：http://hz.jqgfzy.top/gtgwdgenej.html

E. 字符串处理
来源：http://hz.guannengcc.top/gtoqsegthp.html

================================================================================
来源：http://hz.ydzc1.top/gtlkanawik.html

[E01] 拼接字符串
来源：http://hz.ydjk.org.cn/gtpebsurwu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinghuilouyu.cn/gtaddcurxw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.tian-w.cn/gtlsgudgbl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtlvqphvqa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtqrfofpsb.html


<!-- 参考信息 -->