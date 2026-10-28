代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.cqqwz.cn/gtspwwtvkr.html

C#:   using System.Text;
来源：http://hz.hfpthk.cn/gtogkbwwdd.html

[C12] 立即执行函数 IIFE
来源：http://hz.ybcxt.top/gtqnoskuyb.html

Py:   (lambda: print("run"))()
来源：http://hz.sysykeji.top/gtyicaeyjg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sxryk.cn/gtkmxavene.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sweek.top/gtvaukmknt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenzaomai.com/gtwommzjfp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigfzy.top/gtppbcyrwf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cashguo.top/gtcctcfaxm.html

Ruby: -> { puts "run" }.call
来源：http://hz.feifeiyinyue.top/gtyjxkibxs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jlsjyb.cn/gtxluudkbo.html

[C13] 类型声明 / 类型注解
来源：http://hz.cdnleiting.top/gtaofveqny.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj20258888.top/gtbpbpnatm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtbaxfssgm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.aizwys.cn/gtictznvbj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtfoisnkkg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtnqpibxdz.html

Go:   func add(a, b int) int
来源：http://hz.hfpthk.cn/gtvfrciuqc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ybcxt.top/gtkvwqcngw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hammf.cn/gtmsyiezvr.html

[C14] 泛型函数
来源：http://hz.hywenlv.cn/gtosmorgdz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenjidiqi.icu/gtqmgzjwem.html

PHP:  // 无泛型
来源：http://hz.jinyuanbaomall.cn/gtryvcpitn.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gtorbiktiy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gtuvdqunuo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gogol.net.cn/gtavpndxzo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.redwolf501.top/gtscngnszl.html

Ruby: # 无泛型
来源：http://hz.jinqigfzy.top/gtokzvhxds.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cheryme.top/gtgutdejei.html

[C15] 解构 / 展开参数
来源：http://hz.xylfe.cn/gtndfrpgja.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258.top/gtzifhjbze.html

PHP:  [$a, $b] = $pair;
来源：http://hz.316326.xyz/gtnafqxrau.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shuidangran.top/gtbxlcoyeu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fzhhl.top/gtxidguzuc.html

Java: // 无解构
来源：http://hz.cheryme.top/gtosubsfum.html

Go:   // 无解构
来源：http://hz.yongpay.top/gttutdfexb.html

Ruby: a, b = pair
来源：http://hz.bjfxy.top/gtyvdbgcdh.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangkeji.top/gtbedbirep.html

[C16] 函数 / 方法重载
来源：http://hz.jinyuanbaomall.cn/gttvuhgmld.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.kuanghao11.cn/gtxdjtczqo.html

PHP:  // 无重载
来源：http://hz.birdmap.top/gtwkgartwn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hammf.cn/gtvuwnxgmt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258888.top/gtvtfbvyes.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.smart0.xyz/gthnmlmwhn.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhiwuduotai.top/gtuvfhoijf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guowangkeji.top/gtfazhfirk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hysaishi.cn/gtrzhwqwsl.html

================================================================================
来源：http://hz.yj20258.top/gtrmxkjato.html

D. 数组 / 列表 / 集合
来源：http://hz.jlsjyb.cn/gtmeitntqe.html

================================================================================
来源：http://hz.gotoacloud.top/gtvmprbuwc.html

[D01] 创建数组 / 列表
来源：http://hz.nanxuanxn.top/gtqflupyne.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnxiangtu.top/gtwydffzjw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.snrcjt.cn/gtitdlsyxw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangshuangyany.cn/gtfrilotjz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cucudq.cn/gtrnfzmtwf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aizwys.cn/gtqwindkfq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangkeji.top/gtrcccuqsy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.smart0.xyz/gtghueedvn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cucudq.cn/gtsxrevlld.html

[D02] 追加元素到末尾
来源：http://hz.xziqi.cn/gtqstjxghy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgfzy.top/gtszsgrvkx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhengqikj.top/gtogornvoe.html

JS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtoylciphd.html

TS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtzygngjil.html

Java: list.add(4);
来源：http://hz.snrcjt.cn/gttyafzcnf.html

Go:   arr = append(arr, 4)
来源：http://hz.andypj.xyz/gttnpizpkx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.kuanghao11.cn/gtlippawpw.html

C#:   list.Add(4);
来源：http://hz.zhixingplan.top/gtihflxllb.html

[D03] 在指定位置插入元素
来源：http://hz.ivvv.top/gtcoupgrfx.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangkeji.top/gtndmvtife.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtkqftuill.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.iojbl.cn/gtqbnkgaop.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtzhjcojti.html

Java: list.add(0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtylsmtqoa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yongpay.top/gtsfubxlis.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydjk.org.cn/gtvtmxdhpt.html

C#:   list.Insert(0, 0);
来源：http://hz.zycfv.cn/gtqrmksxok.html

[D04] 删除元素
来源：http://hz.jiagoushi.top/gtaioxcqeo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sufxvd.cn/gtagsrlbtr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aibaodan.cn/gtltbpmbfj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.316326.xyz/gtywvhanlj.html

TS:   arr.splice(0, 1);
来源：http://hz.tianlin.xyz/gtjlsfaijl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shzxlz.cn/gtgziyyevn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jlsjyb.cn/gtnrxrapkj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tanke756.top/gtmimuavpi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenlongwang.top/gtguatnqjo.html

[D05] 访问与修改元素
来源：http://hz.pengpengdd.cyou/gthfzklopn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtxzybfgfa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtlphuivzg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtlvmjxeeo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yvedp.cn/gtxetpasgi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.birdmap.top/gtexhjmful.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtbxvvdxjl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gthacpvcdj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xziqi.cn/gthyvwfhkm.html

[D06] 数组长度
来源：http://hz.iojbl.cn/gtkrwxxjeg.html

Py:   len(arr)
来源：http://hz.shuidangran.top/gtjeppsuto.html

PHP:  count($arr);
来源：http://hz.hnqzz.top/gtnielpnlt.html

JS:   arr.length
来源：http://hz.316326.xyz/gtoeqvsqeh.html

TS:   arr.length
来源：http://hz.jinqigfzy.top/gtzjgfttja.html

Java: list.size();
来源：http://hz.yj20258.top/gtlcitsyfo.html

Go:   len(arr)
来源：http://hz.jlsjyb.cn/gtftlpmnak.html

Ruby: arr.length; arr.size
来源：http://hz.yuanzhike.top/gteyjoyxvg.html

C#:   list.Count;
来源：http://hz.yongpay.top/gtlrhcrdwn.html

[D07] 切片 / 取子数组
来源：http://hz.shanyushiyangtech.top/gtwsboywjj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xingfuxueyuan.xyz/gtmgqeiqai.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yueranfly.top/gtzfhhiksb.html

JS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtantbamqq.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtfwrdkqrb.html

Java: list.subList(1, 4);
来源：http://hz.nwbrower.top/gtkezwvcdg.html

Go:   arr[1:4]
来源：http://hz.sxryk.cn/gtzftwogel.html

Ruby: arr[1, 3]
来源：http://hz.wangshuangyany.cn/gtrvxevgru.html

C#:   list.GetRange(1, 3);
来源：http://hz.tian-w.cn/gtvvhlgxyg.html

[D08] 合并两个数组
来源：http://hz.jinqigfzy.top/gtdgtdcbsq.html

Py:   a + b;  a.extend(b)
来源：http://hz.hfpthk.cn/gtepotijke.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258888.top/gttuitshrc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.pycfn.com/gtjswcpqor.html

TS:   [...a, ...b];
来源：http://hz.dianchejie.cn/gtzfkkjivp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinqigufen.top/gtppdfthvw.html

Go:   append(a, b...)
来源：http://hz.wangdashe.top/gterixboyy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nwbrower.top/gtejiezild.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenjidiqi.icu/gthevpomud.html

[D09] 排序（升序）
来源：http://hz.shzxlz.cn/gtwpmcvmqw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtayhvrfrt.html

PHP:  sort($arr);
来源：http://hz.quarkkingdee.top/gtupydiblr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xylfe.cn/gtbytotvwb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cheryme.top/gtbwvzvomy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hywenlv.cn/gtgnonhfqz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.smart0.xyz/gtdhwhjawv.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtnbiqtjpa.html

C#:   list.Sort();
来源：http://hz.tian-w.cn/gtoumzlylw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.kuanghao11.cn/gtkorwywem.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jqgfzy.top/gtrgwhrhpd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtingeefky.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guowangkeji.top/gtjqfndnmw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtyclbvjna.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinyuanbaomall.cn/gtivpgkswz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtwlbunihl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sysykeji.top/gttmlhfexq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.aizwys.cn/gtkthopecu.html

[D11] 反转数组
来源：http://hz.zhixingplan.top/gtuscadpzt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.feifeiyinyue.top/gtkqscbiwf.html

PHP:  array_reverse($arr);
来源：http://hz.zhaomingkeji.xyz/gtelygwjkn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yongpay.top/gtgqrwrrdz.html

TS:   [...arr].reverse();
来源：http://hz.cqqwz.cn/gtitzmvqje.html

Java: Collections.reverse(list);
来源：http://hz.jiagoushi.top/gtoibnripj.html

Go:   slices.Reverse(arr)
来源：http://hz.nanxinkj.top/gtpvuguwqc.html

Ruby: arr.reverse
来源：http://hz.jqgfzy.top/gtzzghopic.html

C#:   list.Reverse();
来源：http://hz.shangyingyoupin.top/gtapzvvzrq.html

[D12] 查找元素下标
来源：http://hz.yj202588.top/gtrbsjgcnu.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258888.top/gtesqgksdj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenlongwang.top/gtbszjyryb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.havefunace.top/gtnsjqdvmj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gthayjqwaj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.wangdashe.top/gtzwlnjiiw.html

Go:   slices.Index(arr, x)
来源：http://hz.dashuyun.cn/gtlxrbsgze.html

Ruby: arr.index(x)
来源：http://hz.hysaishi.cn/gtflhkcnhy.html

C#:   list.IndexOf(x);
来源：http://hz.ydzc1.top/gtzzcofsih.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cdnleiting.top/gtufovcktb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.0kj1m.cn/gtnmnkisia.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydjk.org.cn/gtzlayuacn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtsuwtsuno.html

TS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtkjakrdfx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guannengcc.top/gtkvvdxzqj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigfzy.top/gtokuxmfla.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gaohongyu789.top/gtrlzjqdlv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hfpthk.cn/gtlkvjwoin.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gzhubu.top/gtablrriuv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ybcxt.top/gtnbphnmla.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangkeji.top/gtwxqtedri.html

JS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gtynxyanee.html

TS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtkazxnevr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hammf.cn/gtsvntlfbb.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gtuftuxhyu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.meibo888.top/gtokogrpjn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgufenzy.top/gtecqryqgk.html

[D15] 去重
来源：http://hz.zhongyouzk.top/gtsgyjcsnw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtpawbjgjx.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtfhmagvob.html

JS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtyhehseuf.html

TS:   [...new Set(arr)]
来源：http://hz.gzhubu.top/gtitfpnyzh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fzhhl.top/gttfqpwizi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shzxlz.cn/gtwnsyaugq.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtmecxbirq.html

C#:   list.Distinct().ToList()
来源：http://hz.gaohongyu789.top/gtmynifloc.html

[D16] 求和与平均值
来源：http://hz.chenlongwang.top/gthjqasacm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guannengcc.top/gtzlmlmiey.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuetiantiany.cn/gtiststyvb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtyhmgoxum.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtugoarlvf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtltsgutwj.html

Go:   // 手写循环累加
来源：http://hz.zhiwuduotai.top/gtoygtskek.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.9152youxi.cn/gtldypbfde.html

C#:   list.Sum();  list.Average()
来源：http://hz.jiagoushi.top/gthrsrxtxu.html

[D17] 最大值与最小值
来源：http://hz.quarkkingdee.top/gtftxvauis.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtatxofzkm.html

PHP:  max($arr);  min($arr);
来源：http://hz.yanxiufei.cn/gtotjchxus.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aizwys.cn/gtbviaqugp.html

TS:   Math.max(...arr);
来源：http://hz.xingfuxueyuan.xyz/gtuvmplvls.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jlsjyb.cn/gtxsedqora.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cashguo.top/gtgzanggmd.html

Ruby: arr.max;  arr.min
来源：http://hz.gaohongyu789.top/gtwxmexfcp.html

C#:   list.Max();  list.Min()
来源：http://hz.shanyushiyangkeji.top/gtullxudsd.html

[D18] 扁平化嵌套数组
来源：http://hz.zhaomingkeji.xyz/gtkdlnuite.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gaohongyu789.top/gtlztwazsz.html

PHP:  array_merge(...$nested);
来源：http://hz.havefunace.top/gtyqkrxbwt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.feifeiyinyue.top/gtbrdwupxh.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtficyphkz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hysaishi.cn/gtdzfelthg.html

Go:   // 手写双层循环
来源：http://hz.wangshuangyany.cn/gtvdqsvkju.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtbkouqyrk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gaohongyu789.top/gtyqezmhpd.html

[D19] 按字段分组
来源：http://hz.andypj.xyz/gtpadqkxim.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jqgufenzy.top/gtoaivenix.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gtnusrlzsg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.9152youxi.cn/gttivxqswb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jianghu66.top/gtdvhpqnmx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sysykeji.top/gtfuqtgmvn.html

Go:   // 手写 map[string][]T
来源：http://hz.hongshengwenyu.top/gthosoztur.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.bjfxy.top/gtegcqhzxk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shangyingyoupin.top/gtqqxqllbe.html

[D20] 统计每个元素出现次数
来源：http://hz.sufxvd.cn/gtevfayesd.html

Py:   Counter(arr)
来源：http://hz.gzhubu.top/gttjsjxcen.html

PHP:  array_count_values($arr);
来源：http://hz.hongshengwenyu.top/gtnbrseeto.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtemybgjuq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.vqdsnc.cn/gtzaenswpx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.vqdsnc.cn/gtnfwmvwzj.html

Go:   // 手写 map[T]int
来源：http://hz.sweek.top/gtmfegsmru.html

Ruby: arr.tally
来源：http://hz.guowangkeji.top/gtsmkcfsuf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gtwqeixczt.html

[D21] 判断是否包含某元素
来源：http://hz.ppjwa.cn/gtmfzduojq.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtgpulhjua.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhaomingkeji.xyz/gtwbeaqevh.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtpjqcepje.html

TS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtniyvbrby.html

Java: list.contains(x)
来源：http://hz.jinghuilouyu.cn/gtanbzbjns.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhixingplan.top/gtzeycdtzp.html

Ruby: arr.include?(x)
来源：http://hz.zhixingplan.top/gtpplibmnp.html

C#:   list.Contains(x)
来源：http://hz.tian-w.cn/gtolegvvry.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gtfoigidts.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jianghu66.top/gtexnkhmyg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yangfankeji.com/gtelvshuiw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhoulong.xyz/gtiutkvoau.html

TS:   [...arr];
来源：http://hz.zhijiandao.cn/gtakcqixeh.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gttegaqwov.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhongyouzk.top/gtzzmbxebp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.9152youxi.cn/gtlmygtzqp.html

C#:   new List<int>(list);
来源：http://hz.smart0.xyz/gtqhiwlgju.html

[D23] reduce 累积计算
来源：http://hz.vqdsnc.cn/gtwtehqjqq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xinyue.icu/gtndtpoclv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.svipenyu.cn/gtuvqkmhtq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xziqi.cn/gtvyhhrmxw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hammf.cn/gtpglhdabf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.fengsongda.top/gtbhizbteo.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtcuiyqoii.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yuxming.cn/gtczioyhbp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhiwuduotai.top/gtsvxgkpts.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigufen.top/gtnrbpynpa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gogol.net.cn/gtveopxvtf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tanke756.top/gtuzahwerb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.tianlin.xyz/gtcubcobhm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gtnzryystx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ehwqpu.com/gthcdwicfp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj202588.top/gttuyijloc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.svipenyu.cn/gtdjzfhyju.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtxhalxvur.html

[D25] Set 集合去重与交并差
来源：http://hz.sufxvd.cn/gtltkjzreh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.svipenyu.cn/gtqykqlfxa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.birdmap.top/gtlbaheyzo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ivvv.top/gtrvhskioj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.iojbl.cn/gtmiwvtkrm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinghuilouyu.cn/gtyuleoduz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhiwuduotai.top/gtjlxhhjup.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtpdcbwyoq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cqqwz.cn/gtxtuzyoni.html

[D26] 数组转字符串
来源：http://hz.hysaishi.cn/gttovckmpg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.snrcjt.cn/gttaejqcmf.html

PHP:  implode(", ", $arr);
来源：http://hz.gzhubu.top/gtdhyhvasc.html

JS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtopvugtni.html

TS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtrvzvumkg.html

Java: String.join(", ", list)
来源：http://hz.jlsjyb.cn/gtaplkvnzg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gtxreeueop.html

Ruby: arr.join(", ")
来源：http://hz.ydjk.org.cn/gtszoxduon.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtgflgekol.html

================================================================================
来源：http://hz.yueranfly.top/gtueodloyd.html

E. 字符串处理
来源：http://hz.yongpay.top/gtkngmnuue.html

================================================================================
来源：http://hz.sxryk.cn/gtorjizxsy.html

[E01] 拼接字符串
来源：http://hz.wangdashe.top/gtqwvkohap.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuetiantiany.cn/gtjobzfliy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aizwys.cn/gtvqdunrly.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtbfwsmgkj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtzrgdvryk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xinyue.icu/gtnqfakvnc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.kuanghao11.cn/gtftbmsyba.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jyoumei.cn/gtydbzslcl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj202588.top/gtplcygozi.html

[E02] 重复字符串
来源：http://hz.ydjk.org.cn/gtatuaxgxu.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gtiwdmvmbd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ppjwa.cn/gtmbtdtkqz.html

JS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtvcsyrhyv.html


<!-- 参考信息 -->