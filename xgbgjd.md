代发 wailian999

C#:   块级作用域
来源：http://hz.kuanghao11.cn/gtqskjhcwk.html

[C11] 模块导入与导出
来源：http://hz.guannengcc.top/gtgxeccsfo.html

Py:   from module import func
来源：http://hz.cdnleiting.top/gtkcbeiofe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.svipenyu.cn/gtlcxkhvlv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ivvv.top/gtmorfqtzb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhoulong.xyz/gtsobuywdo.html

Java: import java.util.List;
来源：http://hz.jinqigfzy.top/gtbmkdxvcg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhongyouzk.top/gtqlemzged.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhaomingkeji.xyz/gtuqhhsipo.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gtmuprlfwi.html

[C12] 立即执行函数 IIFE
来源：http://hz.9152youxi.cn/gtxagnaibm.html

Py:   (lambda: print("run"))()
来源：http://hz.fengsongda.top/gtddkmravn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yanxiufei.cn/gtrtsegqai.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtodudrpjd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gtyvxhsjxt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhiwuduotai.top/gtppedrdss.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhaomingkeji.xyz/gtirmdswia.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhongyouzk.top/gtnjzpbssq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xuanzx.com/gtzsfeenns.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydzc1.top/gtljtdilab.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guannengcc.top/gtphrmphzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtrrowlsfn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.kuanghao11.cn/gtekfgqzzo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtdrioscru.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtfxiwcqmi.html

Go:   func add(a, b int) int
来源：http://hz.yvedp.cn/gtudeaglgj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.vqdsnc.cn/gtciprupuo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fzhhl.top/gtwctxnoqk.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtarvwiynk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigfzy.top/gtryszgpws.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtwnckluvl.html

JS:   // 无泛型
来源：http://hz.jlsjyb.cn/gtbjyhymjw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.haohaochexian.top/gtrpzzinmq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.dashuyun.cn/gtgfeeddra.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.andypj.xyz/gtwnptadxy.html

Ruby: # 无泛型
来源：http://hz.gzhubu.top/gtofmjrkfv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.bjfxy.top/gtgchrrqci.html

[C15] 解构 / 展开参数
来源：http://hz.mhx1999.top/gtqbdijapu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daxiang520.top/gtwdibhyny.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shanyushiyangtech.top/gtlagzbdts.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yongpay.top/gtnuojeqsv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.0kj1m.cn/gtakpfstoz.html

Java: // 无解构
来源：http://hz.hnxiangtu.top/gtktiucegx.html

Go:   // 无解构
来源：http://hz.jiagoushi.top/gthtkptuja.html

Ruby: a, b = pair
来源：http://hz.cdnleiting.top/gtdmttuqqv.html

C#:   var (a, b) = pair;
来源：http://hz.vqdsnc.cn/gtuoefahqp.html

[C16] 函数 / 方法重载
来源：http://hz.mhx1999.top/gtzukoklqd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.mhx1999.top/gtsezijnyh.html

PHP:  // 无重载
来源：http://hz.yvedp.cn/gtyocrznks.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sysykeji.top/gtauzbkpne.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gtveybvxvn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.havefunace.top/gtsnquvrnb.html

Go:   // 无重载：用不同函数名
来源：http://hz.guannengcc.top/gtxvhuacun.html

Ruby: # 无重载：靠动态参数
来源：http://hz.quarkkingdee.top/gtwhygofjd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cashguo.top/gthzkxzqhb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtflwskpid.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gtmybtvmif.html

================================================================================
来源：http://hz.yongpay.top/gteywpaqhy.html

[D01] 创建数组 / 列表
来源：http://hz.yongpay.top/gtyrqcabmu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.mhx1999.top/gtcwontcbm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shzxlz.cn/gtyymggksw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenlongwang.top/gtizkmprlj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pengpengdd.cyou/gtvlyermjz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cheryme.top/gtabekqiqn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xylfe.cn/gtpifffzzl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gtavyjlucl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.guowangkeji.top/gtkuqcjbok.html

[D02] 追加元素到末尾
来源：http://hz.sysykeji.top/gtgoygfatl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shuidangran.top/gtwofrdmgc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fzhhl.top/gtlaeztiox.html

JS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtdookiaia.html

TS:   arr.push(4);
来源：http://hz.sweek.top/gtxvsqwmmh.html

Java: list.add(4);
来源：http://hz.jiagoushi.top/gtehdnpehm.html

Go:   arr = append(arr, 4)
来源：http://hz.gogol.net.cn/gtbilbhsdm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinqigfzy.top/gtrinihglu.html

C#:   list.Add(4);
来源：http://hz.jinyuanbaomall.cn/gtlytewwqo.html

[D03] 在指定位置插入元素
来源：http://hz.gzhubu.top/gtlwklytzp.html

Py:   arr.insert(0, 0)
来源：http://hz.hnxiangtu.top/gtfemaghat.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daxiang520.top/gtkaxuwteq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgufenzy.top/gtlsobqkfw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhoulong.xyz/gttjvzfqio.html

Java: list.add(0, 0);
来源：http://hz.xinyue.icu/gtflikiuzo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hammf.cn/gtaectkxxq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gaohongyu789.top/gttxvurbij.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxinkj.top/gtdnkvhqfm.html

[D04] 删除元素
来源：http://hz.daxiang520.top/gtglnfrefs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gotoacloud.top/gttyddftmx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhiwuduotai.top/gtbktepjsd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guannengcc.top/gtavsxwpfa.html

TS:   arr.splice(0, 1);
来源：http://hz.shzxlz.cn/gtwiimdems.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jyoumei.cn/gtjlkwiblc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.9152youxi.cn/gtlgnmixgf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinghuilouyu.cn/gtndedifep.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.dianchejie.cn/gtjmxqxqms.html

[D05] 访问与修改元素
来源：http://hz.wangshuangyany.cn/gtofdjerqk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtdkjrorof.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.dianchejie.cn/gtuwxyveri.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuanzhike.top/gtfrilztco.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hongshengwenyu.top/gtjjqfskih.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.pycfn.com/gtjypnvvgp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hammf.cn/gtoewaluzn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtohgpfpge.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tianlin.xyz/gttszkgofo.html

[D06] 数组长度
来源：http://hz.yongpay.top/gtjyvzwzhn.html

Py:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtnulnjacy.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtbtyaxmie.html

JS:   arr.length
来源：http://hz.hysaishi.cn/gtzxkewwjh.html

TS:   arr.length
来源：http://hz.sxryk.cn/gttqkfzwyu.html

Java: list.size();
来源：http://hz.shanyushiyangtech.top/gtrnrtaryq.html

Go:   len(arr)
来源：http://hz.yj20258888.top/gtokvyiijd.html

Ruby: arr.length; arr.size
来源：http://hz.xziqi.cn/gtcpnhllvj.html

C#:   list.Count;
来源：http://hz.sufxvd.cn/gttxnabcvn.html

[D07] 切片 / 取子数组
来源：http://hz.chenjidiqi.icu/gthxnzfblk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangtech.top/gtncjlocsd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ydjk.org.cn/gtosskkvod.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtmraunbpt.html

TS:   arr.slice(1, 4);
来源：http://hz.chenjidiqi.icu/gtdwrhzigj.html

Java: list.subList(1, 4);
来源：http://hz.cashguo.top/gtlnzittlh.html

Go:   arr[1:4]
来源：http://hz.jlsjyb.cn/gtblgonxjl.html

Ruby: arr[1, 3]
来源：http://hz.chenlongwang.top/gtltjdaglf.html

C#:   list.GetRange(1, 3);
来源：http://hz.hnqzz.top/gtwihqaado.html

[D08] 合并两个数组
来源：http://hz.yvedp.cn/gtovwgnmap.html

Py:   a + b;  a.extend(b)
来源：http://hz.sxryk.cn/gtvldzcpxa.html

PHP:  array_merge($a, $b);
来源：http://hz.chenlongwang.top/gticzdtudr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shzxlz.cn/gttszdqipv.html

TS:   [...a, ...b];
来源：http://hz.svipenyu.cn/gtechteiwp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydzc1.top/gtfovzknol.html

Go:   append(a, b...)
来源：http://hz.yj20258.top/gtsgzrbsvj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fzhhl.top/gtvyfzbkaq.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258.top/gtpbvvvudk.html

[D09] 排序（升序）
来源：http://hz.yuanzhike.top/gtqlezlkmc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtvwubsqmj.html

PHP:  sort($arr);
来源：http://hz.cucudq.cn/gtnfqvnimt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nwbrower.top/gtlwqtntue.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj20258.top/gtazefdktt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daxiang520.top/gtejdjehqh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydzc1.top/gtvrxauxrw.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtbhkvraro.html

C#:   list.Sort();
来源：http://hz.jinqigufen.top/gtgvieighb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.fzhhl.top/gtsrxxiifh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258.top/gtzcwomdur.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gthgiicmrn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gteilrwoph.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtgqzowauy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shangyingyoupin.top/gtrxrdirxt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.smart0.xyz/gtjjnqlkfx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.dashuyun.cn/gtlbdmjrwk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hnxiangtu.top/gtufpxkkux.html

[D11] 反转数组
来源：http://hz.redwolf501.top/gtpoahsrcv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ehwqpu.com/gtvyjgqjtu.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258888.top/gthwjsslac.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigufen.top/gtsgvmuifk.html

TS:   [...arr].reverse();
来源：http://hz.svipenyu.cn/gtixplbicu.html

Java: Collections.reverse(list);
来源：http://hz.zdqjudy.top/gtfkpneybk.html

Go:   slices.Reverse(arr)
来源：http://hz.cucudq.cn/gtiktdhhhv.html

Ruby: arr.reverse
来源：http://hz.aibaodan.cn/gtkhyrzdmj.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gttvabbncp.html

[D12] 查找元素下标
来源：http://hz.zhongyouzk.top/gtzrvmomxx.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gtstsimckq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.c1oappe.top/gtqapyvwkc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gthshbpbnc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtvqvdidus.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.guannengcc.top/gtxneeaogw.html

Go:   slices.Index(arr, x)
来源：http://hz.meibo888.top/gtsvvcwdzg.html

Ruby: arr.index(x)
来源：http://hz.yj20258888.top/gtijnzpavk.html

C#:   list.IndexOf(x);
来源：http://hz.zhixingplan.top/gtdjezecxr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ivvv.top/gtdcimgzij.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pengpengdd.cyou/gtsnvrvpuy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenzaomai.com/gtdogblutq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtrzxydzxo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gtgaommkiv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinghuilouyu.cn/gtlkxejfns.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhaomingkeji.xyz/gteubfshqx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yongpay.top/gtbxszgjwy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenjidiqi.icu/gtchuucahd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangdashe.top/gtkxqadqwy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gaohongyu789.top/gtxkykfrys.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.birdmap.top/gtvrtqagvo.html

JS:   arr.map(x => x * 2)
来源：http://hz.sufxvd.cn/gtqfhttfxm.html

TS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtogobyqpg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hfpthk.cn/gtidtkrcmn.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtrlnytmnb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgfzy.top/gtrttdeytd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hfpthk.cn/gtspyoavtu.html

[D15] 去重
来源：http://hz.ywan-chungtsiang.top/gtitysihcx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtdcmdzhgt.html

PHP:  array_unique($arr);
来源：http://hz.hywenlv.cn/gtmeaabizj.html

JS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtmlhliebe.html

TS:   [...new Set(arr)]
来源：http://hz.guowangkeji.top/gtofoygmrw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xingfuxueyuan.xyz/gtitekdgxh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jqgfzy.top/gtqqpxfiok.html

Ruby: arr.uniq
来源：http://hz.hammf.cn/gtezokepuh.html

C#:   list.Distinct().ToList()
来源：http://hz.chenlongwang.top/gtqgrwouhq.html

[D16] 求和与平均值
来源：http://hz.jianghu66.top/gtyfcwhefj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenlongwang.top/gtkbpmhnpc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhoulong.xyz/gtpueydosr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtjnmrmber.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtcmpjhawj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jyoumei.cn/gtgegsvczk.html

Go:   // 手写循环累加
来源：http://hz.yvedp.cn/gtxnekwxtn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sweek.top/gtwbhsehje.html

C#:   list.Sum();  list.Average()
来源：http://hz.ydzc1.top/gtthuffdjk.html

[D17] 最大值与最小值
来源：http://hz.birdmap.top/gtvjfvsjlq.html

Py:   max(arr);  min(arr)
来源：http://hz.cdnleiting.top/gtimqgfmza.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtngywpwqt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxuanxn.top/gtseflodvx.html

TS:   Math.max(...arr);
来源：http://hz.xylfe.cn/gtyfhnrmtt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.316326.xyz/gtvhnxocus.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj202588.top/gtnafbmzkh.html

Ruby: arr.max;  arr.min
来源：http://hz.zhixingplan.top/gtdcnxatqr.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxuanxn.top/gttkszmitm.html

[D18] 扁平化嵌套数组
来源：http://hz.jinyuanbaomall.cn/gtzksjzdsy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ivvv.top/gtbljmooze.html

PHP:  array_merge(...$nested);
来源：http://hz.feifeiyinyue.top/gttftpidph.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangtech.top/gtuebowyaj.html

TS:   nested.flat();
来源：http://hz.xylfe.cn/gtstonqjev.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuanzhike.top/gtvkzypckp.html

Go:   // 手写双层循环
来源：http://hz.smart0.xyz/gtdkdkofop.html

Ruby: nested.flatten
来源：http://hz.yuxming.cn/gtbppiojdt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtauwhbdnp.html

[D19] 按字段分组
来源：http://hz.nanxinkj.top/gtwuadwqlo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daxiang520.top/gtxvputlly.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtsozwtjgm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtoldvofal.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daria6918.cn/gtnforjgdu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cheryme.top/gtzeqkosfg.html

Go:   // 手写 map[string][]T
来源：http://hz.snrcjt.cn/gtofjqgdmz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgfzy.top/gtkfikhous.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gtcicjmppy.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtbuqvpykc.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtgefdcdui.html

PHP:  array_count_values($arr);
来源：http://hz.fengsongda.top/gtnwqhhoht.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtxksgwmcf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtxmaffoig.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gogol.net.cn/gtoyhuqlpr.html

Go:   // 手写 map[T]int
来源：http://hz.xziqi.cn/gtotbccajk.html

Ruby: arr.tally
来源：http://hz.jianghu66.top/gtooixxfkt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tanke756.top/gtcdkifkcb.html

[D21] 判断是否包含某元素
来源：http://hz.fengsongda.top/gtmuvxacsh.html

Py:   x in arr
来源：http://hz.jqgufenzy.top/gtedumkcwa.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhijiandao.cn/gtgueuvagd.html

JS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gtmdahdadj.html

TS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtiabqphqs.html

Java: list.contains(x)
来源：http://hz.tianlin.xyz/gttabxnjlh.html

Go:   slices.Contains(arr, x)
来源：http://hz.kuanghao11.cn/gtqbpyzhcn.html

Ruby: arr.include?(x)
来源：http://hz.daxiang520.top/gtjvbjrkic.html

C#:   list.Contains(x)
来源：http://hz.jinqigfzy.top/gtrmimxmds.html

[D22] 复制数组（避免共享引用）
来源：http://hz.meibo888.top/gtlzqvaael.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.smart0.xyz/gtbyccgltu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sysykeji.top/gtnxutycwx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cashguo.top/gtbmnrdmfp.html

TS:   [...arr];
来源：http://hz.jinghuilouyu.cn/gtfthzmymx.html

Java: new ArrayList<>(list);
来源：http://hz.sxryk.cn/gtjwwumcoy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigufen.top/gtpdwgblrx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.smart0.xyz/gtnjsmyewr.html

C#:   new List<int>(list);
来源：http://hz.chenzaomai.com/gttqlqfkir.html

[D23] reduce 累积计算
来源：http://hz.chenlongwang.top/gtioffylpp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aizwys.cn/gtvebromak.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.svipenyu.cn/gtdrhejdpz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.316326.xyz/gtaamodpts.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gttjwvpphs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cqqwz.cn/gtxavhysfh.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtetgcxpre.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangshuangyany.cn/gtscjiqyfs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtuntxlmdx.html

[D24] 字典 / Map 基本操作
来源：http://hz.yvedp.cn/gtroydjtlj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tian-w.cn/gtpkvfuqcx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.havefunace.top/gtpgvtlcra.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dashuyun.cn/gtgjpemtdb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cashguo.top/gtcftckazc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hongshengwenyu.top/gtxlcjptei.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sufxvd.cn/gtstgwimdw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.havefunace.top/gtmcjpbpxi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.wangshuangyany.cn/gtbjbruppw.html

[D25] Set 集合去重与交并差
来源：http://hz.fzhhl.top/gtjboyfhbe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daria6918.cn/gtbmuizpuh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuanzx.com/gtjnxvuqym.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yonumen.top/gtrzmzlura.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgfzy.top/gtilfxnqtv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gotoacloud.top/gtcqkotmnc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenzaomai.com/gtsgodbtty.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xylfe.cn/gtbbqvgqgv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hywenlv.cn/gticpwfzzm.html

[D26] 数组转字符串
来源：http://hz.pycfn.com/gtuizbkpek.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ybcxt.top/gtbukydicz.html

PHP:  implode(", ", $arr);
来源：http://hz.guannengcc.top/gtqpxkczte.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtshwxsdzp.html

TS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtjlyyvdcj.html

Java: String.join(", ", list)
来源：http://hz.shangyingyoupin.top/gtrabbsrge.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jianghu66.top/gtqwinjoan.html

Ruby: arr.join(", ")
来源：http://hz.snrcjt.cn/gttlelgukb.html

C#:   string.Join(", ", list)
来源：http://hz.aizwys.cn/gtuydenbvx.html

================================================================================
来源：http://hz.hywenlv.cn/gtqbvoqprl.html

E. 字符串处理
来源：http://hz.fzhhl.top/gtuyokbaiv.html

================================================================================
来源：http://hz.snrcjt.cn/gtrjxtdjex.html

[E01] 拼接字符串
来源：http://hz.tianlin.xyz/gtnvizenmu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhongyouzk.top/gtcnxaqgop.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.svipenyu.cn/gtfexxpiub.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dianchejie.cn/gtbrqpbgwf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtxzeztxhd.html


<!-- 参考信息 -->