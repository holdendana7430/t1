代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.bjfxy.top/gtktclwsfj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnqzz.top/gtixthgcxz.html

Java: import java.util.List;
来源：http://hz.chenzaomai.com/gtkphflixg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tanke756.top/gtjfeasoly.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ehwqpu.com/gtjtfttywr.html

C#:   using System.Text;
来源：http://hz.yj20258888.top/gtxhrrsudh.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhengqikj.top/gtphzkjbgk.html

Py:   (lambda: print("run"))()
来源：http://hz.ehwqpu.com/gttleiqjri.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtnvjwponq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gogol.net.cn/gtcbghkpns.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtkilkszpm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.c1oappe.top/gtvujaayez.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yuxming.cn/gtoxaspxyw.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj20258.top/gtfevydqys.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aizwys.cn/gtyspcyivj.html

[C13] 类型声明 / 类型注解
来源：http://hz.fzhhl.top/gtphdbyoeo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangdashe.top/gtofzldmff.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtndmmkklx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zycfv.cn/gtgooavvqd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuxming.cn/gtrbrjcvak.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtjtgifrqz.html

Go:   func add(a, b int) int
来源：http://hz.jyoumei.cn/gthgfqywkt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.dashuyun.cn/gthewkytap.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenlongwang.top/gtdxaaibcy.html

[C14] 泛型函数
来源：http://hz.jyoumei.cn/gtmyxgqepd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cheryme.top/gthqbtuskl.html

PHP:  // 无泛型
来源：http://hz.nanxinkj.top/gthoqzkjvi.html

JS:   // 无泛型
来源：http://hz.ppjwa.cn/gtenloldsd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yanxiufei.cn/gtmsmcbvdm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tanke756.top/gtbphizath.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.kuanghao11.cn/gtpslheyir.html

Ruby: # 无泛型
来源：http://hz.gotoacloud.top/gtzqkufrox.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhengqikj.top/gtvabgjcqo.html

[C15] 解构 / 展开参数
来源：http://hz.0kj1m.cn/gtkbpodkcf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.feifeiyinyue.top/gtavhryhef.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yongpay.top/gtzlgltokx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtcikreoij.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.birdmap.top/gtroqrxxdt.html

Java: // 无解构
来源：http://hz.c1oappe.top/gtprtchixv.html

Go:   // 无解构
来源：http://hz.sweek.top/gtrarzmfge.html

Ruby: a, b = pair
来源：http://hz.ppjwa.cn/gthvtzdeao.html

C#:   var (a, b) = pair;
来源：http://hz.sufxvd.cn/gtvmbfpudi.html

[C16] 函数 / 方法重载
来源：http://hz.cucudq.cn/gtujdbpwuy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sxryk.cn/gtuqjamtxi.html

PHP:  // 无重载
来源：http://hz.fengsongda.top/gtgvexggby.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daria6918.cn/gteavejpcd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tianlin.xyz/gthdmwysqz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daria6918.cn/gtfjiddvwo.html

Go:   // 无重载：用不同函数名
来源：http://hz.guannengcc.top/gtnvicbmzm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pycfn.com/gtvkugwfip.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jiagoushi.top/gtzhcccdbw.html

================================================================================
来源：http://hz.xinyue.icu/gtnweugdxj.html

D. 数组 / 列表 / 集合
来源：http://hz.hnxiangtu.top/gtlsychuax.html

================================================================================
来源：http://hz.mhx1999.top/gtnxyvdmve.html

[D01] 创建数组 / 列表
来源：http://hz.andypj.xyz/gttqtklywh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guowangkeji.top/gttdgfyaoi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gtzbjudlxa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sweek.top/gtohfzscra.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yvedp.cn/gtlinavbij.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sufxvd.cn/gtobqsdsko.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pengpengdd.cyou/gtkuopypxr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258.top/gtwxuorarr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shanyushiyangkeji.top/gtupsezpen.html

[D02] 追加元素到末尾
来源：http://hz.pycfn.com/gtuynbakpa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.c1oappe.top/gtpjzkedgb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hfpthk.cn/gtxomnxmqa.html

JS:   arr.push(4);
来源：http://hz.316326.xyz/gtnflmbiud.html

TS:   arr.push(4);
来源：http://hz.sxryk.cn/gtmzliugml.html

Java: list.add(4);
来源：http://hz.shanyushiyangtech.top/gtvfcfywyf.html

Go:   arr = append(arr, 4)
来源：http://hz.snrcjt.cn/gtzyctdxex.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.c1oappe.top/gtbcdgipxf.html

C#:   list.Add(4);
来源：http://hz.bjfxy.top/gtgqlgofmt.html

[D03] 在指定位置插入元素
来源：http://hz.xinyue.icu/gtwfmjyejt.html

Py:   arr.insert(0, 0)
来源：http://hz.yj20258.top/gtwylytdwo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtrvwmmizc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hammf.cn/gtrctvuztk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jianghu66.top/gtamepspwd.html

Java: list.add(0, 0);
来源：http://hz.redwolf501.top/gttlcrwmdc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.daxiang520.top/gtlkgsvdsi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hysaishi.cn/gtdrccjxkw.html

C#:   list.Insert(0, 0);
来源：http://hz.daxiang520.top/gtvwhkxlmu.html

[D04] 删除元素
来源：http://hz.jqgfzy.top/gtaihfjyry.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenjidiqi.icu/gtwvbxtmty.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258.top/gttweyoizj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtppoaxfsu.html

TS:   arr.splice(0, 1);
来源：http://hz.nwbrower.top/gtqnktfipa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigfzy.top/gtgsvsrwwc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guowangkeji.top/gtroeqiqio.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tian-w.cn/gtjityodeh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtrjieyllw.html

[D05] 访问与修改元素
来源：http://hz.yj20258888.top/gtriruwogy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtypxtguqm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yonumen.top/gtovmhelhs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.andypj.xyz/gtiburrurv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cashguo.top/gtwsqecvpk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gtegnoqcvr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tian-w.cn/gtqworkxoa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtfrweclni.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtaqjaplan.html

[D06] 数组长度
来源：http://hz.vqdsnc.cn/gtsmzseexn.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gttejwzyyh.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtscjjkbwi.html

JS:   arr.length
来源：http://hz.redwolf501.top/gtwkocogag.html

TS:   arr.length
来源：http://hz.cdnleiting.top/gttxymnnqv.html

Java: list.size();
来源：http://hz.xziqi.cn/gtibweljgl.html

Go:   len(arr)
来源：http://hz.gzhubu.top/gtgsmolkxv.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangtech.top/gtijvzhmqb.html

C#:   list.Count;
来源：http://hz.xuetiantiany.cn/gtsfhsigsb.html

[D07] 切片 / 取子数组
来源：http://hz.gotoacloud.top/gtgdjadgqi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtkkpkftdn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.quarkkingdee.top/gtwcyweltx.html

JS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtqvshsixg.html

TS:   arr.slice(1, 4);
来源：http://hz.xinyue.icu/gtlvqxcugd.html

Java: list.subList(1, 4);
来源：http://hz.ivvv.top/gtyfktjodf.html

Go:   arr[1:4]
来源：http://hz.zdqjudy.top/gtkgqkskea.html

Ruby: arr[1, 3]
来源：http://hz.bjfxy.top/gtseulxjoj.html

C#:   list.GetRange(1, 3);
来源：http://hz.kuanghao11.cn/gtlmdctviy.html

[D08] 合并两个数组
来源：http://hz.daria6918.cn/gtkxsvscfm.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258888.top/gtartrqttw.html

PHP:  array_merge($a, $b);
来源：http://hz.guannengcc.top/gtktmexrtg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.svipenyu.cn/gtijrasinp.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtxeqcspah.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtletabrpf.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtatvbnjjm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guannengcc.top/gtlkafykli.html

C#:   a.Concat(b).ToList()
来源：http://hz.nanxinkj.top/gtxnadozdt.html

[D09] 排序（升序）
来源：http://hz.jlsjyb.cn/gtaoyplbbf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtmynejwsb.html

PHP:  sort($arr);
来源：http://hz.hywenlv.cn/gtteigwfkc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aizwys.cn/gtachdvcza.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigufen.top/gtdizcrhlt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuxming.cn/gtbywvcnpn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xinyue.icu/gtjaxwxvss.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gthelfqtqy.html

C#:   list.Sort();
来源：http://hz.yanxiufei.cn/gtpqusxmpm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nanxinkj.top/gtezvjgcxk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtighwxpkf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhaomingkeji.xyz/gtyozomsrm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gthojeyyue.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xinyue.icu/gtbtvjkkyb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tian-w.cn/gtjdmabyzd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.52xcode.cn/gtvyzzydhf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.0kj1m.cn/gtlumclvxv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.aibaodan.cn/gtkdxvbhpv.html

[D11] 反转数组
来源：http://hz.dashuyun.cn/gtnotzhtxq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jyoumei.cn/gtulwnmnyk.html

PHP:  array_reverse($arr);
来源：http://hz.xuanzx.com/gtmswuvuiv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zdqjudy.top/gtnnmujeyr.html

TS:   [...arr].reverse();
来源：http://hz.ivvv.top/gtqrgkikes.html

Java: Collections.reverse(list);
来源：http://hz.jqgfzy.top/gttjsvybbo.html

Go:   slices.Reverse(arr)
来源：http://hz.316326.xyz/gthvlrater.html

Ruby: arr.reverse
来源：http://hz.yj20258888.top/gtlxpeyiiw.html

C#:   list.Reverse();
来源：http://hz.cashguo.top/gtkptbckfx.html

[D12] 查找元素下标
来源：http://hz.pycfn.com/gtspzavhwi.html

Py:   arr.index(x);  x in arr
来源：http://hz.hywenlv.cn/gtvtmhajwd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenlongwang.top/gtxfqlhves.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtjvuzmxxz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtwhwimelt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.mhx1999.top/gtkelntnwt.html

Go:   slices.Index(arr, x)
来源：http://hz.nwbrower.top/gthnbwppuw.html

Ruby: arr.index(x)
来源：http://hz.haohaochexian.top/gtcsooqkyf.html

C#:   list.IndexOf(x);
来源：http://hz.fzhhl.top/gtcghicpre.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gzhubu.top/gtfhikejsp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jlsjyb.cn/gterzhxslu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenlongwang.top/gtzflmmhzc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydzc1.top/gtgpncjqeq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtaywavjxe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenlongwang.top/gtkfytxwhc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.52xcode.cn/gtntvlmict.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yonumen.top/gtkqxnlpgx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shangyingyoupin.top/gtfgrbrgfb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.meibo888.top/gtsvkbqezc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jiagoushi.top/gtglckketb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yvedp.cn/gtmiruxoth.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtztxzqyve.html

TS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtbduzenfl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.kuanghao11.cn/gtasoxgjlf.html

Go:   // 手写循环
来源：http://hz.zycfv.cn/gtkkgkvhha.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ppjwa.cn/gtfgovnkez.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pengpengdd.cyou/gtxcyxgmel.html

[D15] 去重
来源：http://hz.gogol.net.cn/gtmgzvjnfs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.aibaodan.cn/gtbvycsbzu.html

PHP:  array_unique($arr);
来源：http://hz.hfpthk.cn/gtpaoctbog.html

JS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtishznazl.html

TS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtndzpdibd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhijiandao.cn/gtvqeofstk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zycfv.cn/gtruiggydc.html

Ruby: arr.uniq
来源：http://hz.pengpengdd.cyou/gtacvcufvj.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258888.top/gtnbbylhfc.html

[D16] 求和与平均值
来源：http://hz.aizwys.cn/gtjgfwfrvs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gttxphxhhn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258.top/gtoqshalvn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtcgjyfyyh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtvlshtyll.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj202588.top/gtlhfpcspa.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtxjgtgxrq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jlsjyb.cn/gtjcebcvkp.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gtalyjaliq.html

[D17] 最大值与最小值
来源：http://hz.shangyingyoupin.top/gtibdxlnhy.html

Py:   max(arr);  min(arr)
来源：http://hz.hysaishi.cn/gtwbshatkq.html

PHP:  max($arr);  min($arr);
来源：http://hz.yonumen.top/gtjptkvopq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cashguo.top/gtmprofkha.html

TS:   Math.max(...arr);
来源：http://hz.xylfe.cn/gttyrklgmg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258.top/gtgxmjkxko.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.haohaochexian.top/gthbxxqmzg.html

Ruby: arr.max;  arr.min
来源：http://hz.hnxiangtu.top/gtzixopuln.html

C#:   list.Max();  list.Min()
来源：http://hz.jinghuilouyu.cn/gtlmutkyyt.html

[D18] 扁平化嵌套数组
来源：http://hz.kuanghao11.cn/gtyhskscru.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tanke756.top/gtmlfklgmr.html

PHP:  array_merge(...$nested);
来源：http://hz.0kj1m.cn/gtbrtjnaju.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnqzz.top/gtbeturnpv.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gtrqojkutw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tianlin.xyz/gtsbbkwpir.html

Go:   // 手写双层循环
来源：http://hz.hfpthk.cn/gtzhnwesqy.html

Ruby: nested.flatten
来源：http://hz.ybcxt.top/gtvnescpri.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.snrcjt.cn/gtxxsmkuij.html

[D19] 按字段分组
来源：http://hz.9152youxi.cn/gtuurjxbcp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.dianchejie.cn/gtvbbntgxn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tian-w.cn/gtyqddlxzh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigufen.top/gtyvrchgfx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hywenlv.cn/gtofgqtefs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.meibo888.top/gtuvjtopxf.html

Go:   // 手写 map[string][]T
来源：http://hz.yuanzhike.top/gtkcyczxsf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.iojbl.cn/gthhypwabe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ppjwa.cn/gtfctkuuyj.html

[D20] 统计每个元素出现次数
来源：http://hz.yanxiufei.cn/gtpguijiyw.html

Py:   Counter(arr)
来源：http://hz.zdqjudy.top/gtexnhdcui.html

PHP:  array_count_values($arr);
来源：http://hz.gogol.net.cn/gtcjtantsv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtjsuluvhl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.redwolf501.top/gtpjnpczqa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydzc1.top/gtwqmsxcyj.html

Go:   // 手写 map[T]int
来源：http://hz.tian-w.cn/gtehjxrcux.html

Ruby: arr.tally
来源：http://hz.xylfe.cn/gtqbbcafmq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuanzhike.top/gtysmjwszi.html

[D21] 判断是否包含某元素
来源：http://hz.ywan-chungtsiang.top/gteaexjvbi.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtoudzcsci.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guowangkeji.top/gtdepcgarb.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtkuhkdeqq.html

TS:   arr.includes(x)
来源：http://hz.bjfxy.top/gtpwxdtnly.html

Java: list.contains(x)
来源：http://hz.aizwys.cn/gtfdbegkvy.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuxming.cn/gtytffiwmm.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangtech.top/gtdrvccaww.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtavsbslug.html

[D22] 复制数组（避免共享引用）
来源：http://hz.c1oappe.top/gtjxqcdfno.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shanyushiyangkeji.top/gtjiswarjt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jianghu66.top/gtaeqqfqhs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.52xcode.cn/gtmqctjflj.html

TS:   [...arr];
来源：http://hz.shangyingyoupin.top/gtqmnjyhos.html

Java: new ArrayList<>(list);
来源：http://hz.havefunace.top/gtkqjtlddn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shangyingyoupin.top/gtyxqpuekf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daria6918.cn/gthaukbcle.html

C#:   new List<int>(list);
来源：http://hz.gotoacloud.top/gtflqnjqlt.html

[D23] reduce 累积计算
来源：http://hz.nanxinkj.top/gtllgxhqok.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.wangdashe.top/gtzyqduyoh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgfzy.top/gtlmetepbi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dianchejie.cn/gtotpdkmck.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangtech.top/gthlkegtou.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aizwys.cn/gtnhndhmso.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gtupjhayob.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xylfe.cn/gtcsjfetta.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhiwuduotai.top/gtldupiwcy.html

[D24] 字典 / Map 基本操作
来源：http://hz.sweek.top/gthjzsgfac.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinqigufen.top/gtwbsjnnsn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenzaomai.com/gtcgwbvtcl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aibaodan.cn/gtlampnqbm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daxiang520.top/gtljnvxmcx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ehwqpu.com/gtmptmfvhh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtnkqeymys.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.andypj.xyz/gtrhfbfqjl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.316326.xyz/gtferzeefp.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtysjagtbl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yangfankeji.com/gtcsaogglq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhongyouzk.top/gtvniskfdd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhijiandao.cn/gtbpmicgur.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydjk.org.cn/gtwwomqhsk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gtuospfodq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtpjmdgbdj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhijiandao.cn/gtycgvzorw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhongyouzk.top/gtlvkljlpp.html

[D26] 数组转字符串
来源：http://hz.shangyingyoupin.top/gtthdzyupl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258888.top/gtbxrotatf.html

PHP:  implode(", ", $arr);
来源：http://hz.yangfankeji.com/gtxfqcmwlv.html

JS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtezsfnyij.html

TS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtnhlvbizf.html

Java: String.join(", ", list)
来源：http://hz.mhx1999.top/gtpnjkjssy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhixingplan.top/gtagmciavt.html

Ruby: arr.join(", ")
来源：http://hz.jyoumei.cn/gtzsjcyezx.html

C#:   string.Join(", ", list)
来源：http://hz.smart0.xyz/gtyvhnrdcc.html

================================================================================
来源：http://hz.meibo888.top/gtsyytuflo.html

E. 字符串处理
来源：http://hz.xuetiantiany.cn/gtixvksxzz.html

================================================================================
来源：http://hz.zycfv.cn/gtbigzqnyn.html

[E01] 拼接字符串
来源：http://hz.xziqi.cn/gtpdmjbrfp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ywan-chungtsiang.top/gtushlphbb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhijiandao.cn/gtprngtenv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gterpjgzkt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gaohongyu789.top/gtudfiolqa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgufenzy.top/gtgkmhabvx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fengsongda.top/gtwpmwyjub.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.316326.xyz/gtxuecvlvm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xziqi.cn/gtpckaewrh.html


<!-- 参考信息 -->