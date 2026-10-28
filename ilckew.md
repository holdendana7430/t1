代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnxiangtu.top/gttkmmsair.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ywan-chungtsiang.top/gtrfcnvmcs.html

Java: import java.util.List;
来源：http://hz.mhx1999.top/gtlevotqth.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gzhubu.top/gtqfmthhcx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shangyingyoupin.top/gtbmkyfiyc.html

C#:   using System.Text;
来源：http://hz.xziqi.cn/gteatxwzkn.html

[C12] 立即执行函数 IIFE
来源：http://hz.zycfv.cn/gtbyiqnzak.html

Py:   (lambda: print("run"))()
来源：http://hz.havefunace.top/gtnrzbnnwb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.iojbl.cn/gtrvohzjum.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtomksobzo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtsfeqmyex.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigfzy.top/gtpighpwkz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tanke756.top/gtrirrciay.html

Ruby: -> { puts "run" }.call
来源：http://hz.daxiang520.top/gtrfcwiqoa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yongpay.top/gterchavjw.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtdukrqohd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gzhubu.top/gtlokzhzce.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtrnxshupr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yangfankeji.com/gtbqpeqpfl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dashuyun.cn/gttqjlgozp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gttdsptwou.html

Go:   func add(a, b int) int
来源：http://hz.daria6918.cn/gtmqofnnyu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gtwnkngkuc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shangyingyoupin.top/gtgirnpohi.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtdcupqyku.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtltrbxuhe.html

PHP:  // 无泛型
来源：http://hz.yuanzhike.top/gtbhvvxfbo.html

JS:   // 无泛型
来源：http://hz.zdqjudy.top/gtioxutfwo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gtxnkktmix.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pycfn.com/gtkanskxxo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxinkj.top/gtxkvfgjen.html

Ruby: # 无泛型
来源：http://hz.shuidangran.top/gthxrpowcy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhiwuduotai.top/gtkjmtkxgo.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtunvxfoat.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fengsongda.top/gtlmmwfvta.html

PHP:  [$a, $b] = $pair;
来源：http://hz.haohaochexian.top/gtavuxtmwi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hammf.cn/gtpabpbhua.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zycfv.cn/gtvwgqlfdh.html

Java: // 无解构
来源：http://hz.yongpay.top/gtajwcaosx.html

Go:   // 无解构
来源：http://hz.shzxlz.cn/gtbdiaxgne.html

Ruby: a, b = pair
来源：http://hz.andypj.xyz/gtjngkjcem.html

C#:   var (a, b) = pair;
来源：http://hz.c1oappe.top/gtncleoqgt.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtjxrexjjr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinyuanbaomall.cn/gtowcugkun.html

PHP:  // 无重载
来源：http://hz.chenlongwang.top/gtvsbydvnz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxuanxn.top/gtjawjreyu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinghuilouyu.cn/gtlrtisxia.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xylfe.cn/gtdknnkkiy.html

Go:   // 无重载：用不同函数名
来源：http://hz.gotoacloud.top/gtwcgoezbu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuanzhike.top/gtwfxwzjpq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhiwuduotai.top/gtshbritoa.html

================================================================================
来源：http://hz.xuanzx.com/gtsvxenrct.html

D. 数组 / 列表 / 集合
来源：http://hz.guowangkeji.top/gtwgtzfvcp.html

================================================================================
来源：http://hz.yangfankeji.com/gtqwufodxa.html

[D01] 创建数组 / 列表
来源：http://hz.yueranfly.top/gthhnoflbk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yueranfly.top/gteqhvqaab.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sysykeji.top/gtogvlbffb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.316326.xyz/gtplculnnl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daria6918.cn/gtalkewarw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtuzuuyeef.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.wangshuangyany.cn/gtohqwoszs.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sysykeji.top/gtwwimwsft.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtjrtmajli.html

[D02] 追加元素到末尾
来源：http://hz.jyoumei.cn/gtymyifnrt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shangyingyoupin.top/gtcyhubqru.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ehwqpu.com/gtqemkzfuc.html

JS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtrrsupdfv.html

TS:   arr.push(4);
来源：http://hz.andypj.xyz/gtlzkibarv.html

Java: list.add(4);
来源：http://hz.jinqigufen.top/gtjbqkzilg.html

Go:   arr = append(arr, 4)
来源：http://hz.sysykeji.top/gtmtitrqtc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aibaodan.cn/gtrgnbakoj.html

C#:   list.Add(4);
来源：http://hz.nanxuanxn.top/gtlgslpyve.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258888.top/gtxavcwacn.html

Py:   arr.insert(0, 0)
来源：http://hz.gotoacloud.top/gtrijykoao.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cheryme.top/gtqkqdrids.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gotoacloud.top/gtyqlvrfuw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinghuilouyu.cn/gthezkwmmy.html

Java: list.add(0, 0);
来源：http://hz.chenjidiqi.icu/gtjucbrwge.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.daxiang520.top/gtfneeglhu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yueranfly.top/gtujpsdvdd.html

C#:   list.Insert(0, 0);
来源：http://hz.fengsongda.top/gtoexiunek.html

[D04] 删除元素
来源：http://hz.sxryk.cn/gteoahwdzh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtznfjnnft.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtbefbvefv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tianlin.xyz/gtcqeowjtm.html

TS:   arr.splice(0, 1);
来源：http://hz.hongshengwenyu.top/gtygscewdc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigfzy.top/gtybygmtvs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenjidiqi.icu/gtuuhmobsc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.feifeiyinyue.top/gtldzazqrc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.andypj.xyz/gtatfnusen.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtrllgtjsn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gttkctzrnk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tian-w.cn/gthmgxqeqg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.quarkkingdee.top/gtiyofmorp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnqzz.top/gttplndnxx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigfzy.top/gtkodfcoev.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sysykeji.top/gtzzvyxkhn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtdbksfwfd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnxiangtu.top/gtnisxdkrl.html

[D06] 数组长度
来源：http://hz.9152youxi.cn/gtyammlkui.html

Py:   len(arr)
来源：http://hz.xinyue.icu/gtjimisfpc.html

PHP:  count($arr);
来源：http://hz.yj20258.top/gtypeyzlzt.html

JS:   arr.length
来源：http://hz.xuetiantiany.cn/gtelamaxub.html

TS:   arr.length
来源：http://hz.yongpay.top/gtqafmkugj.html

Java: list.size();
来源：http://hz.sufxvd.cn/gtyuychnqd.html

Go:   len(arr)
来源：http://hz.chenlongwang.top/gtqgxbwrka.html

Ruby: arr.length; arr.size
来源：http://hz.havefunace.top/gteewyeckn.html

C#:   list.Count;
来源：http://hz.ydzc1.top/gtgqnmosis.html

[D07] 切片 / 取子数组
来源：http://hz.jqgfzy.top/gtertpljnb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aizwys.cn/gtljknulwa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tianlin.xyz/gtuaqbwaim.html

JS:   arr.slice(1, 4);
来源：http://hz.xinyue.icu/gtgiukftzg.html

TS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtxxrrrznh.html

Java: list.subList(1, 4);
来源：http://hz.wangdashe.top/gtijupugav.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gtevgakfhf.html

Ruby: arr[1, 3]
来源：http://hz.fzhhl.top/gtrtduwlzr.html

C#:   list.GetRange(1, 3);
来源：http://hz.svipenyu.cn/gtnhcjloru.html

[D08] 合并两个数组
来源：http://hz.jqgufenzy.top/gtrvdixmdz.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigufen.top/gtqwusztmv.html

PHP:  array_merge($a, $b);
来源：http://hz.yangfankeji.com/gtjbogteip.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.svipenyu.cn/gtawvbijox.html

TS:   [...a, ...b];
来源：http://hz.jyoumei.cn/gtkoszkzrm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.birdmap.top/gtmybjivvh.html

Go:   append(a, b...)
来源：http://hz.mhx1999.top/gtvdtznucp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtjnmkxgvq.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtjatmovsu.html

[D09] 排序（升序）
来源：http://hz.hongshengwenyu.top/gttisrudxx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtmiwaewwa.html

PHP:  sort($arr);
来源：http://hz.snrcjt.cn/gtjhawggiz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenlongwang.top/gtdmxajvmr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuetiantiany.cn/gtbmzbscau.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj202588.top/gtdsthgivb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.mhx1999.top/gtowmqjfbz.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtmlagiezu.html

C#:   list.Sort();
来源：http://hz.tian-w.cn/gtmttfrrcw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cqqwz.cn/gttlmtkqxo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.fengsongda.top/gtgbnuxkmu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtfjwrfwbb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtdmemsurq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtchurgmks.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ehwqpu.com/gtufyyglbh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gtdsipdxbp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.havefunace.top/gtobvwqxkm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj202588.top/gtjreulcnn.html

[D11] 反转数组
来源：http://hz.cdnleiting.top/gtgmrfomqz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.redwolf501.top/gtblpkjtdv.html

PHP:  array_reverse($arr);
来源：http://hz.zycfv.cn/gtztcnjtjm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.redwolf501.top/gtqpjkmdzt.html

TS:   [...arr].reverse();
来源：http://hz.daria6918.cn/gtbrdzuvhm.html

Java: Collections.reverse(list);
来源：http://hz.cucudq.cn/gtzncnsrsn.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtvecxzumg.html

Ruby: arr.reverse
来源：http://hz.yonumen.top/gtphucikrd.html

C#:   list.Reverse();
来源：http://hz.316326.xyz/gtpxlurjrc.html

[D12] 查找元素下标
来源：http://hz.aizwys.cn/gtnqrsuziw.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinqigufen.top/gtciuwvahw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cheryme.top/gtqgteyjoo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.c1oappe.top/gthyflbmlw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtukqmjars.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hongshengwenyu.top/gtzixztdtc.html

Go:   slices.Index(arr, x)
来源：http://hz.zhijiandao.cn/gtbiysmced.html

Ruby: arr.index(x)
来源：http://hz.mhx1999.top/gtuvgdgmkf.html

C#:   list.IndexOf(x);
来源：http://hz.xuetiantiany.cn/gtprcuflhx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.haohaochexian.top/gtocgyseqi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jyoumei.cn/gtalfnadfv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shzxlz.cn/gtprpeoipe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gttqynywjq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtsgkoahyd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hfpthk.cn/gtkdakdwkt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gogol.net.cn/gtupkyftbq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.smart0.xyz/gtzsawsnut.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yangfankeji.com/gtnbvdxwcd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aibaodan.cn/gtwmmldats.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shzxlz.cn/gtktuitrrk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tanke756.top/gtgthsydhd.html

JS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtihkcytmi.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtnfxrqbcq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xylfe.cn/gtrtlmjuds.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtekprfuvk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gotoacloud.top/gtqgiawbei.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinghuilouyu.cn/gtcikhmicu.html

[D15] 去重
来源：http://hz.cashguo.top/gtrmflnrye.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtxvppbdcj.html

PHP:  array_unique($arr);
来源：http://hz.sysykeji.top/gtafmgaaoe.html

JS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtcmtvcpgw.html

TS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtuwhthgmc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xingfuxueyuan.xyz/gtyzwhoaqi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.snrcjt.cn/gtfozpjtja.html

Ruby: arr.uniq
来源：http://hz.hfpthk.cn/gtytijmucw.html

C#:   list.Distinct().ToList()
来源：http://hz.hfpthk.cn/gtytxntnhh.html

[D16] 求和与平均值
来源：http://hz.chenlongwang.top/gtjyqtlbwd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinyuanbaomall.cn/gtvxriefoa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinqigfzy.top/gtqxhvpvlk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtinoilqlx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtbelpehmr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhijiandao.cn/gtpewjsrwp.html

Go:   // 手写循环累加
来源：http://hz.gaohongyu789.top/gtbxqyqxws.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.meibo888.top/gtmhkffqyc.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuetiantiany.cn/gtdwgadojm.html

[D17] 最大值与最小值
来源：http://hz.jinyuanbaomall.cn/gtmchlsbqn.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtvacjsyfm.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtmkgmicgi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gaohongyu789.top/gtkmycwysc.html

TS:   Math.max(...arr);
来源：http://hz.hywenlv.cn/gtfhdxdyki.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258888.top/gtgvrmgulz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hammf.cn/gthovqxdih.html

Ruby: arr.max;  arr.min
来源：http://hz.nwbrower.top/gtxhnzyljw.html

C#:   list.Max();  list.Min()
来源：http://hz.yj202588.top/gtaynakyqj.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gtkaojhivr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangdashe.top/gtuoafogmp.html

PHP:  array_merge(...$nested);
来源：http://hz.iojbl.cn/gtcuvtfgbg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.daxiang520.top/gtiozqunri.html

TS:   nested.flat();
来源：http://hz.meibo888.top/gtbukeosgc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.vqdsnc.cn/gtvvugmefj.html

Go:   // 手写双层循环
来源：http://hz.xylfe.cn/gtshdudcey.html

Ruby: nested.flatten
来源：http://hz.birdmap.top/gtzcworyfg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.feifeiyinyue.top/gtsfzggkfo.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtvdbviefv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daria6918.cn/gtjgkvwslg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nanxinkj.top/gtofekxgei.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.9152youxi.cn/gtayrvbhbm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gtbxzbutnb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtvbtygtvw.html

Go:   // 手写 map[string][]T
来源：http://hz.zhoulong.xyz/gtylopymrz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangtech.top/gtclhuwebr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxuanxn.top/gtarjohcbj.html

[D20] 统计每个元素出现次数
来源：http://hz.yvedp.cn/gtkzzpzjam.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangkeji.top/gtrhacfcbi.html

PHP:  array_count_values($arr);
来源：http://hz.jianghu66.top/gtshmtipzg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jlsjyb.cn/gtdrbjyqdl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtskwylsll.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shzxlz.cn/gtmguaaiyl.html

Go:   // 手写 map[T]int
来源：http://hz.hongshengwenyu.top/gtrihuyikd.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtepaupoxw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258.top/gtobnebvtx.html

[D21] 判断是否包含某元素
来源：http://hz.jqgfzy.top/gtdnpthjqk.html

Py:   x in arr
来源：http://hz.feifeiyinyue.top/gtkddnvnoo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gaohongyu789.top/gtbtefparx.html

JS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtsseuhryc.html

TS:   arr.includes(x)
来源：http://hz.ywan-chungtsiang.top/gtompqqffs.html

Java: list.contains(x)
来源：http://hz.cqqwz.cn/gtgfoasccv.html

Go:   slices.Contains(arr, x)
来源：http://hz.xziqi.cn/gtdvlpcooy.html

Ruby: arr.include?(x)
来源：http://hz.ydzc1.top/gtnbjktmln.html

C#:   list.Contains(x)
来源：http://hz.redwolf501.top/gtrcivpgeh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.kuanghao11.cn/gtqfdpnilz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ywan-chungtsiang.top/gtfzbvjdsg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhiwuduotai.top/gtbuwvmeqn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.c1oappe.top/gtjpupwasg.html

TS:   [...arr];
来源：http://hz.iojbl.cn/gtbizvauub.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtguuemksn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuanzhike.top/gtcokaorbk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yvedp.cn/gtnvrkvobd.html

C#:   new List<int>(list);
来源：http://hz.jiagoushi.top/gtklukxmga.html

[D23] reduce 累积计算
来源：http://hz.tian-w.cn/gtylklkjku.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jyoumei.cn/gtitylzhap.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hammf.cn/gtpdomxzqt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sxryk.cn/gttsopltow.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtafxirigw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.mhx1999.top/gtocmrlimr.html

Go:   // 手写循环
来源：http://hz.dianchejie.cn/gtahyounkh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.daria6918.cn/gttksmvlhr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gogol.net.cn/gttmywqxcm.html

[D24] 字典 / Map 基本操作
来源：http://hz.pengpengdd.cyou/gtmjfwnkuk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.snrcjt.cn/gtufdolddn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cashguo.top/gtvwpekrbu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.pengpengdd.cyou/gtrikkzvog.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gotoacloud.top/gtbrunmgtx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangdashe.top/gtecppfwky.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xingfuxueyuan.xyz/gtamajujbn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnxiangtu.top/gthhzycirx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sweek.top/gtrwftqzhr.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxuanxn.top/gtfirhluvy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hysaishi.cn/gttgapbhhn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuanzhike.top/gthjxrkioy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.52xcode.cn/gtyuxpeqgw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cucudq.cn/gturcuhhgl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangshuangyany.cn/gttynhsfea.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.316326.xyz/gtjytmyaxn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xingfuxueyuan.xyz/gtsdxxburs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.svipenyu.cn/gtuxctjqln.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gtscqcfgcj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ywan-chungtsiang.top/gturxiuwwe.html

PHP:  implode(", ", $arr);
来源：http://hz.jinyuanbaomall.cn/gtcmyutmqk.html

JS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gthdeauavu.html

TS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtmoucnqjh.html

Java: String.join(", ", list)
来源：http://hz.fzhhl.top/gtauegzubw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sufxvd.cn/gtlijefrca.html

Ruby: arr.join(", ")
来源：http://hz.xziqi.cn/gtdjpsupzf.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigfzy.top/gtulctrqlz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjcxdphcx.html

E. 字符串处理
来源：http://hz.birdmap.top/gtayvwtjnf.html

================================================================================
来源：http://hz.haohaochexian.top/gtcmidabfk.html

[E01] 拼接字符串
来源：http://hz.316326.xyz/gtwshxefbr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jqgfzy.top/gtjzoowweo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnqzz.top/gtpcsccjfk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hongshengwenyu.top/gtbeuilpwo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtrvffmakm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shangyingyoupin.top/gtinpsfcbz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xziqi.cn/gthesggjak.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhongyouzk.top/gtsagaexku.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yuanzhike.top/gtytibqyrv.html


<!-- 参考信息 -->