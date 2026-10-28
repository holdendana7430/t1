代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.daria6918.cn/gthxvaalqg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnxiangtu.top/gtcbimzzbp.html

Java: import java.util.List;
来源：http://hz.ydzc1.top/gtltjyfaaj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.316326.xyz/gtjnxnilev.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.quarkkingdee.top/gtrnkhqpgb.html

C#:   using System.Text;
来源：http://hz.chenzaomai.com/gtjucgngji.html

[C12] 立即执行函数 IIFE
来源：http://hz.ehwqpu.com/gtiettwpet.html

Py:   (lambda: print("run"))()
来源：http://hz.cqqwz.cn/gtjnsbpifv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigufen.top/gtjvuprldo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.pycfn.com/gtzthcbnxf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtsvubcnyw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.guowangkeji.top/gtygbjzjdz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zycfv.cn/gtixdpkkla.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangshuangyany.cn/gtkegagshc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pycfn.com/gtlshqwfrs.html

[C13] 类型声明 / 类型注解
来源：http://hz.xinyue.icu/gtwkowfnme.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinyuanbaomall.cn/gtkgpvlkom.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtaigterbs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258888.top/gttjycqlim.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tanke756.top/gtfuwqkxwj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtlwkozxwl.html

Go:   func add(a, b int) int
来源：http://hz.vqdsnc.cn/gthmlonodj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sxryk.cn/gtadqcggdj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yonumen.top/gtdaymwsxk.html

[C14] 泛型函数
来源：http://hz.cdnleiting.top/gttafwfxyk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenlongwang.top/gtkdgpaucz.html

PHP:  // 无泛型
来源：http://hz.shuidangran.top/gtbbtfwfkb.html

JS:   // 无泛型
来源：http://hz.316326.xyz/gtjayoiviv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuxming.cn/gtbtxkbssc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.quarkkingdee.top/gtxwjdnjch.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.quarkkingdee.top/gttjyhatcf.html

Ruby: # 无泛型
来源：http://hz.bjfxy.top/gtvbbejzof.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gaohongyu789.top/gtkvzsbcjl.html

[C15] 解构 / 展开参数
来源：http://hz.wangdashe.top/gttkrvmcxv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhongyouzk.top/gtvmpffbzu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.meibo888.top/gtpjpnvjcq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jqgufenzy.top/gtjwjptqyt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.vqdsnc.cn/gtnrbtkqmr.html

Java: // 无解构
来源：http://hz.cheryme.top/gtovcpwteo.html

Go:   // 无解构
来源：http://hz.cqqwz.cn/gtrbjjgxyb.html

Ruby: a, b = pair
来源：http://hz.pengpengdd.cyou/gtrrxenpdh.html

C#:   var (a, b) = pair;
来源：http://hz.zycfv.cn/gtlmlyogdl.html

[C16] 函数 / 方法重载
来源：http://hz.nanxinkj.top/gtppedqnnr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tianlin.xyz/gtyirtqdnv.html

PHP:  // 无重载
来源：http://hz.zhoulong.xyz/gtcczmvxnr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sweek.top/gthbvfjzix.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinghuilouyu.cn/gtxcdjvfrd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.quarkkingdee.top/gthggeglub.html

Go:   // 无重载：用不同函数名
来源：http://hz.daxiang520.top/gtzssyiycb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shangyingyoupin.top/gtcwcxswfe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangtech.top/gtfqobmkgq.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjlyqdyhv.html

D. 数组 / 列表 / 集合
来源：http://hz.tanke756.top/gtvlpxchhc.html

================================================================================
来源：http://hz.xylfe.cn/gtswjaegdk.html

[D01] 创建数组 / 列表
来源：http://hz.chenjidiqi.icu/gtytzfcyzh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ppjwa.cn/gtfmjhsgnj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuxming.cn/gtoroezlkm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gaohongyu789.top/gtfhweioir.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258888.top/gttgpucvaq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.redwolf501.top/gtrgwjjdnc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cheryme.top/gtfnyhapbj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ehwqpu.com/gtizupgjpg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cdnleiting.top/gtqlbjhkrg.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gtehbkqqje.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cdnleiting.top/gtjdndgmec.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gtsaadtoke.html

JS:   arr.push(4);
来源：http://hz.jlsjyb.cn/gtdmohstcs.html

TS:   arr.push(4);
来源：http://hz.316326.xyz/gttycbokfv.html

Java: list.add(4);
来源：http://hz.jinghuilouyu.cn/gtophajrtc.html

Go:   arr = append(arr, 4)
来源：http://hz.chenlongwang.top/gtcgywghkr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xinyue.icu/gtrxpdnbrf.html

C#:   list.Add(4);
来源：http://hz.zycfv.cn/gtyugookcf.html

[D03] 在指定位置插入元素
来源：http://hz.cdnleiting.top/gtrdblyskz.html

Py:   arr.insert(0, 0)
来源：http://hz.dianchejie.cn/gtpmmqzjcm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gteoyndjpr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hongshengwenyu.top/gtotgqkfox.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.0kj1m.cn/gtyazggtjt.html

Java: list.add(0, 0);
来源：http://hz.zycfv.cn/gteypzjbwu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuetiantiany.cn/gtnpbmcqwc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sufxvd.cn/gtwykjllbl.html

C#:   list.Insert(0, 0);
来源：http://hz.ydzc1.top/gtkkmhznoj.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtudkjrqpa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.daria6918.cn/gtoemczcba.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gtviodhrvc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gotoacloud.top/gtxbihgbdl.html

TS:   arr.splice(0, 1);
来源：http://hz.ehwqpu.com/gturcbulff.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jiagoushi.top/gtsdesjlzt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.daxiang520.top/gtukaqivas.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hywenlv.cn/gtkyykpise.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pycfn.com/gtraynashy.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gtmsvmycqu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtqqaeovba.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtkcajvmje.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.havefunace.top/gtzjjzvdfd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ywan-chungtsiang.top/gtimkbrdfp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtrzvrptpn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yvedp.cn/gthnjoummi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtqnrmbtgn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtngkdtyld.html

[D06] 数组长度
来源：http://hz.c1oappe.top/gtvdwsyyss.html

Py:   len(arr)
来源：http://hz.ydzc1.top/gtbbfqbyoy.html

PHP:  count($arr);
来源：http://hz.hongshengwenyu.top/gtexrvinrp.html

JS:   arr.length
来源：http://hz.guannengcc.top/gtugjkyydg.html

TS:   arr.length
来源：http://hz.jinghuilouyu.cn/gthjoqliew.html

Java: list.size();
来源：http://hz.sufxvd.cn/gtrslsfycl.html

Go:   len(arr)
来源：http://hz.ppjwa.cn/gtrjybklli.html

Ruby: arr.length; arr.size
来源：http://hz.cdnleiting.top/gtqrqzhmyp.html

C#:   list.Count;
来源：http://hz.sweek.top/gtzcvcigau.html

[D07] 切片 / 取子数组
来源：http://hz.zhengqikj.top/gtdiqqofwi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hywenlv.cn/gtjndtewey.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aibaodan.cn/gttpleddvb.html

JS:   arr.slice(1, 4);
来源：http://hz.hywenlv.cn/gtyfkkprst.html

TS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gtumfeobtx.html

Java: list.subList(1, 4);
来源：http://hz.yvedp.cn/gtdisykeuo.html

Go:   arr[1:4]
来源：http://hz.quarkkingdee.top/gtvlnvpqvw.html

Ruby: arr[1, 3]
来源：http://hz.ivvv.top/gtzsrjrfjv.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangkeji.top/gtbontezrl.html

[D08] 合并两个数组
来源：http://hz.cqqwz.cn/gtfmpsybih.html

Py:   a + b;  a.extend(b)
来源：http://hz.hysaishi.cn/gtainknndq.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258.top/gtnjxhonle.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.redwolf501.top/gtcanntwea.html

TS:   [...a, ...b];
来源：http://hz.zhoulong.xyz/gtznddgtyr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.vqdsnc.cn/gtykgmyovj.html

Go:   append(a, b...)
来源：http://hz.shangyingyoupin.top/gtetugdgaj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.haohaochexian.top/gtamsabqkh.html

C#:   a.Concat(b).ToList()
来源：http://hz.nwbrower.top/gtwdarlqkd.html

[D09] 排序（升序）
来源：http://hz.gaohongyu789.top/gtmjjrjgnw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gtrbawumya.html

PHP:  sort($arr);
来源：http://hz.hywenlv.cn/gtrkegmfwp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hongshengwenyu.top/gtpjniwmcm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuxming.cn/gtbgiqwwun.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.redwolf501.top/gtrzqwjmfr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nwbrower.top/gtvlyzsadl.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtjkzfmadh.html

C#:   list.Sort();
来源：http://hz.jyoumei.cn/gtnifhiqgh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nanxinkj.top/gttvapfles.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hywenlv.cn/gthyeggcvx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtyvypahui.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gtrafgelqj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangshuangyany.cn/gtzrmatuqr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gtfaiixsql.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhengqikj.top/gtvsugwhtz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.vqdsnc.cn/gtysnwverl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.vqdsnc.cn/gtivxhmwfy.html

[D11] 反转数组
来源：http://hz.cucudq.cn/gttdbfnfyu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shuidangran.top/gtoedebhmo.html

PHP:  array_reverse($arr);
来源：http://hz.cdnleiting.top/gthuqchrqz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sweek.top/gtaaqsuyuc.html

TS:   [...arr].reverse();
来源：http://hz.ybcxt.top/gtrwtcjzoe.html

Java: Collections.reverse(list);
来源：http://hz.smart0.xyz/gtnjlsfmhr.html

Go:   slices.Reverse(arr)
来源：http://hz.gzhubu.top/gtxuwyxttm.html

Ruby: arr.reverse
来源：http://hz.xziqi.cn/gtjipkyiwl.html

C#:   list.Reverse();
来源：http://hz.9152youxi.cn/gtjefpugxv.html

[D12] 查找元素下标
来源：http://hz.zycfv.cn/gtyoovxuyk.html

Py:   arr.index(x);  x in arr
来源：http://hz.sufxvd.cn/gtlaaeivwb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hammf.cn/gtgezikxfx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtbvegjauj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtgdokgulb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jlsjyb.cn/gtcqlqkdoe.html

Go:   slices.Index(arr, x)
来源：http://hz.xziqi.cn/gtichfwmiz.html

Ruby: arr.index(x)
来源：http://hz.cucudq.cn/gtjkzvadmt.html

C#:   list.IndexOf(x);
来源：http://hz.meibo888.top/gtjlflnswl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.kuanghao11.cn/gtsetemist.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daxiang520.top/gtqqnriqss.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gogol.net.cn/gtrjskdhbg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.bjfxy.top/gtscwpxrwc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hammf.cn/gtirbnennu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenzaomai.com/gtllshoszf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tanke756.top/gtbbtwekxl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.feifeiyinyue.top/gtsbnsrfsv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigufen.top/gtpyajcuhr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.feifeiyinyue.top/gthaoglnth.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cdnleiting.top/gtqdaszuqz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.meibo888.top/gtzzlpscyu.html

JS:   arr.map(x => x * 2)
来源：http://hz.cheryme.top/gtosojtrdl.html

TS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtkdatfdhc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ehwqpu.com/gtpfkgugok.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtpnwvdafn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtwbuolkct.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xylfe.cn/gtpnbgfnza.html

[D15] 去重
来源：http://hz.fzhhl.top/gtvqpbvway.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhengqikj.top/gtgwqupldn.html

PHP:  array_unique($arr);
来源：http://hz.pengpengdd.cyou/gttgiptody.html

JS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gttjiawbmp.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtlgrknndp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sysykeji.top/gtkompuvkm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hfpthk.cn/gtlnoyajrk.html

Ruby: arr.uniq
来源：http://hz.bjfxy.top/gtljocktdd.html

C#:   list.Distinct().ToList()
来源：http://hz.yvedp.cn/gtbsknrbqg.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gtzqpjlasj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenzaomai.com/gtoydocbhb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtqerbvldw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydzc1.top/gtmcoynygf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtkvgyutvj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydzc1.top/gtflubyzub.html

Go:   // 手写循环累加
来源：http://hz.shuidangran.top/gtszawnbrj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hongshengwenyu.top/gtfjmurucf.html

C#:   list.Sum();  list.Average()
来源：http://hz.haohaochexian.top/gtxwgtiicu.html

[D17] 最大值与最小值
来源：http://hz.xziqi.cn/gttbjcegep.html

Py:   max(arr);  min(arr)
来源：http://hz.iojbl.cn/gtgfkmjylc.html

PHP:  max($arr);  min($arr);
来源：http://hz.aizwys.cn/gtrwekiyso.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gogol.net.cn/gtuxurevfu.html

TS:   Math.max(...arr);
来源：http://hz.yj20258.top/gttsypmncr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhaomingkeji.xyz/gtocgsmznd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dashuyun.cn/gtnaaojtka.html

Ruby: arr.max;  arr.min
来源：http://hz.sufxvd.cn/gthkihrvwj.html

C#:   list.Max();  list.Min()
来源：http://hz.havefunace.top/gtvtxjjuft.html

[D18] 扁平化嵌套数组
来源：http://hz.fengsongda.top/gtaiovsqzj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cucudq.cn/gttkngwcvj.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtpvlsgrpa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shuidangran.top/gttmetbyrq.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gthjffgbsy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xuanzx.com/gtakisnebs.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtobxnfkgc.html

Ruby: nested.flatten
来源：http://hz.pycfn.com/gtyeqtifcl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gogol.net.cn/gtswbyhlbm.html

[D19] 按字段分组
来源：http://hz.bjfxy.top/gtyywrhden.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hysaishi.cn/gtfyfeuogm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jlsjyb.cn/gtxxgujkzt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenlongwang.top/gtfkiluzlb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhijiandao.cn/gtfegcnccm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shanyushiyangkeji.top/gtrbdswlvy.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtuaowbgwk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gzhubu.top/gtzkrwuyyi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yangfankeji.com/gtwbjscstc.html

[D20] 统计每个元素出现次数
来源：http://hz.fzhhl.top/gtoqipttgp.html

Py:   Counter(arr)
来源：http://hz.jinqigfzy.top/gtspvsbyph.html

PHP:  array_count_values($arr);
来源：http://hz.aizwys.cn/gtwbozcsfy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtjdjhlsql.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtsnjsbjbv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuetiantiany.cn/gtkoyczvqz.html

Go:   // 手写 map[T]int
来源：http://hz.vqdsnc.cn/gtdjxmuoqq.html

Ruby: arr.tally
来源：http://hz.hongshengwenyu.top/gtqrlsjaah.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gtpswwiprm.html

[D21] 判断是否包含某元素
来源：http://hz.gotoacloud.top/gturcifbmu.html

Py:   x in arr
来源：http://hz.fzhhl.top/gtnpywweyz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jiagoushi.top/gtdbgwfaag.html

JS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtmnirtryu.html

TS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtrhpezhys.html

Java: list.contains(x)
来源：http://hz.fengsongda.top/gtrqveckif.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinyuanbaomall.cn/gttiicupwj.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtxgnokqow.html

C#:   list.Contains(x)
来源：http://hz.yonumen.top/gtsqbnrfqq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sufxvd.cn/gtjmyxqont.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gogol.net.cn/gtmpdxeoha.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgfzy.top/gtykrcdkud.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pengpengdd.cyou/gtqvarhjpt.html

TS:   [...arr];
来源：http://hz.shanyushiyangkeji.top/gtwnbtlwna.html

Java: new ArrayList<>(list);
来源：http://hz.xingfuxueyuan.xyz/gtelmhbevw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangtech.top/gtgduiticu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gtslnadvsq.html

C#:   new List<int>(list);
来源：http://hz.guowangkeji.top/gtujzlaurv.html

[D23] reduce 累积计算
来源：http://hz.jqgufenzy.top/gtjwkimjpq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtgelduand.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydzc1.top/gtkotswput.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtxgywmzbg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtkwntpbij.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hammf.cn/gtngwhppyj.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gtoujamfbk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aizwys.cn/gtdgtqxfoh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhiwuduotai.top/gtnbwvpqdk.html

[D24] 字典 / Map 基本操作
来源：http://hz.hysaishi.cn/gttrieyndw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.haohaochexian.top/gtbksmnokd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shangyingyoupin.top/gtbjspnyft.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.tianlin.xyz/gtsfrwcequ.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.andypj.xyz/gtytanzuzz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.316326.xyz/gtnndtlijr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.haohaochexian.top/gtbkwsmvsw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aizwys.cn/gtaingwstt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gtcrgyrxhn.html

[D25] Set 集合去重与交并差
来源：http://hz.kuanghao11.cn/gtptntavun.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangdashe.top/gtimcfhklg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydjk.org.cn/gtmscuxyos.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.svipenyu.cn/gtixijujds.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gtwznpzhvz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtxgfgetah.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jyoumei.cn/gtwdznoxem.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jyoumei.cn/gtbmlwlatw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cheryme.top/gtluaocqsz.html

[D26] 数组转字符串
来源：http://hz.birdmap.top/gtmxciqxwa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ivvv.top/gtqmppxqvz.html

PHP:  implode(", ", $arr);
来源：http://hz.yonumen.top/gtxusvgeqw.html

JS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtrdltcsju.html

TS:   arr.join(", ")
来源：http://hz.zhongyouzk.top/gtsfpwrrkk.html

Java: String.join(", ", list)
来源：http://hz.zhixingplan.top/gtrkpxqptp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.andypj.xyz/gtxowogtee.html

Ruby: arr.join(", ")
来源：http://hz.jqgufenzy.top/gtjixbafvm.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigfzy.top/gtixemolbw.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtaagplphm.html

E. 字符串处理
来源：http://hz.gzhubu.top/gtinztscff.html

================================================================================
来源：http://hz.hnqzz.top/gtefunbmik.html

[E01] 拼接字符串
来源：http://hz.sufxvd.cn/gtwwtumvyw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cheryme.top/gtsqsvefea.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gtncbqvxud.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtcftviiuf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtnvqwitot.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuxming.cn/gtrevwjrrg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yonumen.top/gtvxvaufms.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xinyue.icu/gtjwiiqonl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ywan-chungtsiang.top/gthmsmabbu.html


<!-- 参考信息 -->