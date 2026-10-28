代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtqalkmgcv.html

Go:   func add(a, b int) int
来源：http://hz.ivvv.top/gtjffvlysk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sxryk.cn/gtvayjghem.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pengpengdd.cyou/gtgavqbzid.html

[C14] 泛型函数
来源：http://hz.ywan-chungtsiang.top/gtxnrmlwng.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtxqlvxarl.html

PHP:  // 无泛型
来源：http://hz.gotoacloud.top/gtaxpcvahw.html

JS:   // 无泛型
来源：http://hz.cdnleiting.top/gtppysnnwc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.vqdsnc.cn/gtztqbxbih.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xuanzx.com/gtxnztukuc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhiwuduotai.top/gtvovsosmj.html

Ruby: # 无泛型
来源：http://hz.sufxvd.cn/gtvtwfazss.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tianlin.xyz/gtrorihuvg.html

[C15] 解构 / 展开参数
来源：http://hz.ywan-chungtsiang.top/gtebtedmfu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yongpay.top/gtutzktfch.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pengpengdd.cyou/gtnpohhndq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtyynlvbzt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yangfankeji.com/gtgpbnfnkg.html

Java: // 无解构
来源：http://hz.nwbrower.top/gttnzzctoo.html

Go:   // 无解构
来源：http://hz.cashguo.top/gtylrwurbi.html

Ruby: a, b = pair
来源：http://hz.yuanzhike.top/gtnrzyceed.html

C#:   var (a, b) = pair;
来源：http://hz.zdqjudy.top/gtjvlnzzik.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtxbgtybdm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhaomingkeji.xyz/gtawpnauza.html

PHP:  // 无重载
来源：http://hz.hywenlv.cn/gttsdnhhxp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhijiandao.cn/gtapgzqoeo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yangfankeji.com/gttomkxmfd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gthlrvvewe.html

Go:   // 无重载：用不同函数名
来源：http://hz.ppjwa.cn/gtsqbcnevw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtsyknnasx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhengqikj.top/gteevqpoxn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtrwopgrog.html

D. 数组 / 列表 / 集合
来源：http://hz.yvedp.cn/gthoarmlyb.html

================================================================================
来源：http://hz.yangfankeji.com/gtxwkpifxu.html

[D01] 创建数组 / 列表
来源：http://hz.dianchejie.cn/gtrdwubecq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sweek.top/gtqhhxtwzj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guowangkeji.top/gtbmgltztz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hfpthk.cn/gtihmyjfej.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxuanxn.top/gtwonbfiqv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.svipenyu.cn/gtdtdcrthe.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.kuanghao11.cn/gtflzleupx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yanxiufei.cn/gtmzbyldfh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jlsjyb.cn/gtcjjzrwdi.html

[D02] 追加元素到末尾
来源：http://hz.aibaodan.cn/gtrwdaenyn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ppjwa.cn/gtlganzdku.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zdqjudy.top/gtvexcyouc.html

JS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtjmczjeee.html

TS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtvbtzgerd.html

Java: list.add(4);
来源：http://hz.andypj.xyz/gtuoxxjapg.html

Go:   arr = append(arr, 4)
来源：http://hz.yj202588.top/gtmfbgjrpo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cucudq.cn/gtzlaxotzc.html

C#:   list.Add(4);
来源：http://hz.shangyingyoupin.top/gtfvgrrvde.html

[D03] 在指定位置插入元素
来源：http://hz.zdqjudy.top/gtcpjlcuqn.html

Py:   arr.insert(0, 0)
来源：http://hz.pengpengdd.cyou/gtmoddtjce.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aibaodan.cn/gtplkosucy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ywan-chungtsiang.top/gtqzsrgucz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.redwolf501.top/gtoqqrtyxy.html

Java: list.add(0, 0);
来源：http://hz.aizwys.cn/gttbhynuky.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ehwqpu.com/gtzkybgwhy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cashguo.top/gtmonzlsbe.html

C#:   list.Insert(0, 0);
来源：http://hz.nwbrower.top/gtnvrxtjcj.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gtdpseioxj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fengsongda.top/gtwzqxtzxt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yangfankeji.com/gtopomrejl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hongshengwenyu.top/gtzjzvvxlg.html

TS:   arr.splice(0, 1);
来源：http://hz.nwbrower.top/gtufhscmwy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.dianchejie.cn/gtcaklucut.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.fzhhl.top/gtmfetffkx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hnqzz.top/gtujsgammb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangdashe.top/gtxatumetz.html

[D05] 访问与修改元素
来源：http://hz.haohaochexian.top/gtcltcqndq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.birdmap.top/gtkmedrlyq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtxmnzgpxo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gtixzqwyfo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ydzc1.top/gtxupdedok.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtaseaktyh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtkbvbqnnp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtyzjshagy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yongpay.top/gtfyvayozh.html

[D06] 数组长度
来源：http://hz.guannengcc.top/gterwrjkea.html

Py:   len(arr)
来源：http://hz.hnqzz.top/gtqycgchsd.html

PHP:  count($arr);
来源：http://hz.hysaishi.cn/gttyzeenwn.html

JS:   arr.length
来源：http://hz.zhiwuduotai.top/gtjcdhslbq.html

TS:   arr.length
来源：http://hz.jinqigfzy.top/gtdblzzfya.html

Java: list.size();
来源：http://hz.9152youxi.cn/gtpmddeblz.html

Go:   len(arr)
来源：http://hz.sweek.top/gtjsxyslze.html

Ruby: arr.length; arr.size
来源：http://hz.ivvv.top/gtwaxeogbe.html

C#:   list.Count;
来源：http://hz.wangdashe.top/gtyeflvttb.html

[D07] 切片 / 取子数组
来源：http://hz.52xcode.cn/gtjrjqaams.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yonumen.top/gtvfwajuup.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cheryme.top/gtndukacmd.html

JS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtrndfmmnh.html

TS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gthhqqvuoo.html

Java: list.subList(1, 4);
来源：http://hz.hammf.cn/gtzhzofaxk.html

Go:   arr[1:4]
来源：http://hz.havefunace.top/gtwgglvcfh.html

Ruby: arr[1, 3]
来源：http://hz.yj20258.top/gtjbnlwcvu.html

C#:   list.GetRange(1, 3);
来源：http://hz.cdnleiting.top/gtlfrotvuq.html

[D08] 合并两个数组
来源：http://hz.jinqigufen.top/gtwsmkdvxz.html

Py:   a + b;  a.extend(b)
来源：http://hz.redwolf501.top/gtuxmyzshc.html

PHP:  array_merge($a, $b);
来源：http://hz.zycfv.cn/gtupxlletm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zdqjudy.top/gtsvvhzlvy.html

TS:   [...a, ...b];
来源：http://hz.chenzaomai.com/gtifncmxbf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jlsjyb.cn/gtzlslvhka.html

Go:   append(a, b...)
来源：http://hz.redwolf501.top/gtjqnmbkcm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.9152youxi.cn/gtdwegrfno.html

C#:   a.Concat(b).ToList()
来源：http://hz.hongshengwenyu.top/gtjarvhljh.html

[D09] 排序（升序）
来源：http://hz.zhaomingkeji.xyz/gtbwqpgxle.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtrdyxctgo.html

PHP:  sort($arr);
来源：http://hz.ywan-chungtsiang.top/gtgrsdnzrs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xziqi.cn/gtuhhwhxli.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fzhhl.top/gthvsblgul.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gteetyxzup.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yongpay.top/gtfhkzuzqt.html

Ruby: arr.sort
来源：http://hz.havefunace.top/gtwyuemxbz.html

C#:   list.Sort();
来源：http://hz.wangdashe.top/gtkqlsubjd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ppjwa.cn/gtjpupdaxr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jlsjyb.cn/gtusffctlu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtyuxyknhw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gtnmnebmee.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tanke756.top/gtszyixvau.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gtknckrvio.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.andypj.xyz/gtoalbrnqd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hfpthk.cn/gtfyiklfqd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangshuangyany.cn/gtsseuybzh.html

[D11] 反转数组
来源：http://hz.zhiwuduotai.top/gtmxgjmfar.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shangyingyoupin.top/gtiptawvie.html

PHP:  array_reverse($arr);
来源：http://hz.chenjidiqi.icu/gtlrobfvpq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenlongwang.top/gtidbamjye.html

TS:   [...arr].reverse();
来源：http://hz.haohaochexian.top/gtfcknbrwy.html

Java: Collections.reverse(list);
来源：http://hz.cucudq.cn/gtfpvxvdfl.html

Go:   slices.Reverse(arr)
来源：http://hz.guowangkeji.top/gtojbnmosh.html

Ruby: arr.reverse
来源：http://hz.tianlin.xyz/gtmqgxjdvs.html

C#:   list.Reverse();
来源：http://hz.cheryme.top/gtrzlygltu.html

[D12] 查找元素下标
来源：http://hz.wangdashe.top/gtytbqdktb.html

Py:   arr.index(x);  x in arr
来源：http://hz.yangfankeji.com/gtojfqimde.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gthvkcxgwl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.havefunace.top/gthkevicfg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtdgphxawt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sufxvd.cn/gtjknfmoro.html

Go:   slices.Index(arr, x)
来源：http://hz.yanxiufei.cn/gtivlmlfyw.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtzznrvxri.html

C#:   list.IndexOf(x);
来源：http://hz.cdnleiting.top/gtrrzwnjir.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zycfv.cn/gtwiuymvhc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.aibaodan.cn/gtydqshbvi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.havefunace.top/gtwdxpsgpn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yonumen.top/gtsxiucvna.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gttjbifjbk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.c1oappe.top/gthphtsgwy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangdashe.top/gtfqrbymvv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sxryk.cn/gtcxkwqqua.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.redwolf501.top/gtpnanyeuf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.svipenyu.cn/gtliqlvhqr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dashuyun.cn/gtswclwsiu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xylfe.cn/gthwelkakx.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtfviqvujo.html

TS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gthdyxomty.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xingfuxueyuan.xyz/gtawplrqfk.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtqvpxbdoj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ybcxt.top/gtvszdrncc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinyuanbaomall.cn/gtvbdpoxiy.html

[D15] 去重
来源：http://hz.yuxming.cn/gtylnoszqn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtvjhfvnkm.html

PHP:  array_unique($arr);
来源：http://hz.jyoumei.cn/gtfpfkkcej.html

JS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtcplaxsvs.html

TS:   [...new Set(arr)]
来源：http://hz.hammf.cn/gtuygawvzh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.aizwys.cn/gtrewaujmh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gotoacloud.top/gtbyjfmuyt.html

Ruby: arr.uniq
来源：http://hz.havefunace.top/gtwfqxvkxm.html

C#:   list.Distinct().ToList()
来源：http://hz.gaohongyu789.top/gteamrdcdw.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtyjoxzrwl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jyoumei.cn/gtcdvcswbg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtniukwiqp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jianghu66.top/gtuydysjqq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtezyyxtit.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aibaodan.cn/gttihgexbb.html

Go:   // 手写循环累加
来源：http://hz.hysaishi.cn/gtmzgecvnb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jianghu66.top/gtbhyjchpc.html

C#:   list.Sum();  list.Average()
来源：http://hz.aibaodan.cn/gtltijwkns.html

[D17] 最大值与最小值
来源：http://hz.yonumen.top/gtfhatvnji.html

Py:   max(arr);  min(arr)
来源：http://hz.yanxiufei.cn/gtyynrhatp.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhixingplan.top/gtwpcnuzyo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ppjwa.cn/gthigbyhoc.html

TS:   Math.max(...arr);
来源：http://hz.jinqigfzy.top/gtqyysjpph.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.feifeiyinyue.top/gtlcwhskgr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aibaodan.cn/gtdnaeowhi.html

Ruby: arr.max;  arr.min
来源：http://hz.zhijiandao.cn/gtwajtcbus.html

C#:   list.Max();  list.Min()
来源：http://hz.mhx1999.top/gtksvhcxax.html

[D18] 扁平化嵌套数组
来源：http://hz.shuidangran.top/gtrocebbgs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gotoacloud.top/gtdeqocafr.html

PHP:  array_merge(...$nested);
来源：http://hz.ydjk.org.cn/gtinlovswg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.meibo888.top/gticpdxwoq.html

TS:   nested.flat();
来源：http://hz.vqdsnc.cn/gtiwqdjejh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.meibo888.top/gttpnodklh.html

Go:   // 手写双层循环
来源：http://hz.zhengqikj.top/gtgdcrkdns.html

Ruby: nested.flatten
来源：http://hz.pycfn.com/gtnapxszbk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.birdmap.top/gtnkoxrlfw.html

[D19] 按字段分组
来源：http://hz.zhoulong.xyz/gtvaflleeg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.iojbl.cn/gtudlpkisq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xylfe.cn/gtjuuwfoyx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuanzx.com/gtqaxrdppf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gtjwkzfsmo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtrlxxrdme.html

Go:   // 手写 map[string][]T
来源：http://hz.hfpthk.cn/gtwwipfzvg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhengqikj.top/gtelaxeiti.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.snrcjt.cn/gtiytezljq.html

[D20] 统计每个元素出现次数
来源：http://hz.guannengcc.top/gtnplzyhlm.html

Py:   Counter(arr)
来源：http://hz.sysykeji.top/gtfgweqqig.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtdvycegxa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gtkmqvwqag.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtrbordxzo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.bjfxy.top/gtlkjlvzjo.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigufen.top/gtftsvdfhe.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtirrlibns.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shuidangran.top/gtpgfvsxiu.html

[D21] 判断是否包含某元素
来源：http://hz.shuidangran.top/gtlznhiuot.html

Py:   x in arr
来源：http://hz.jinqigfzy.top/gtyfgvxgfu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.iojbl.cn/gtfvjshvqa.html

JS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtvoojdlgd.html

TS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtiljzojqt.html

Java: list.contains(x)
来源：http://hz.daria6918.cn/gtbgekeamu.html

Go:   slices.Contains(arr, x)
来源：http://hz.fengsongda.top/gtkrfpybvl.html

Ruby: arr.include?(x)
来源：http://hz.zdqjudy.top/gtmeymqswp.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtqlaviwcx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydjk.org.cn/gteeucbtfv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.0kj1m.cn/gtwjjvbers.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shuidangran.top/gtntsogmfu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhoulong.xyz/gtlhewnauv.html

TS:   [...arr];
来源：http://hz.xingfuxueyuan.xyz/gtjifxntwf.html

Java: new ArrayList<>(list);
来源：http://hz.birdmap.top/gtddensrkr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgufenzy.top/gtktmidmur.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zycfv.cn/gtssomlkuf.html

C#:   new List<int>(list);
来源：http://hz.guannengcc.top/gtexhgdmdm.html

[D23] reduce 累积计算
来源：http://hz.mhx1999.top/gtlpkthwjy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.redwolf501.top/gtzhlquibo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nwbrower.top/gtgojcwhxv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtqepqgnof.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtrzeseiqm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhoulong.xyz/gtxvsoacpp.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtwzzmstbq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj202588.top/gtcoorvhsc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydzc1.top/gtxgilksle.html

[D24] 字典 / Map 基本操作
来源：http://hz.xingfuxueyuan.xyz/gtdqlchxqa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hywenlv.cn/gtnirjjhgp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgufenzy.top/gtzfkrvcao.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhengqikj.top/gtvpjehtvo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangtech.top/gtoqetpibi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shangyingyoupin.top/gtweskfsyh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.c1oappe.top/gtdwzmqxco.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.quarkkingdee.top/gtmvkynsej.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tianlin.xyz/gtinztcuvu.html

[D25] Set 集合去重与交并差
来源：http://hz.havefunace.top/gtknhaavgl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gzhubu.top/gtrvzazxbn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.c1oappe.top/gtkjunyzru.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tianlin.xyz/gtbdjlcodu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yanxiufei.cn/gtgroavfbw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.pycfn.com/gtzuktgsot.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hywenlv.cn/gtsmwxgpyg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.snrcjt.cn/gtuekpkrrf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtazhjmshx.html

[D26] 数组转字符串
来源：http://hz.tanke756.top/gtsfavicpu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinyuanbaomall.cn/gtutzedrnh.html

PHP:  implode(", ", $arr);
来源：http://hz.feifeiyinyue.top/gthjsjlchp.html

JS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtgrolstiq.html

TS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtjoalqndf.html

Java: String.join(", ", list)
来源：http://hz.9152youxi.cn/gtbqjfieln.html

Go:   strings.Join(strs, ", ")
来源：http://hz.havefunace.top/gtuoyikttn.html

Ruby: arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtyidjeewq.html

C#:   string.Join(", ", list)
来源：http://hz.hnxiangtu.top/gtjasyxlon.html

================================================================================
来源：http://hz.jinqigufen.top/gtihnftsmf.html

E. 字符串处理
来源：http://hz.mhx1999.top/gtovenhped.html

================================================================================
来源：http://hz.jinqigufen.top/gtddhozial.html

[E01] 拼接字符串
来源：http://hz.pengpengdd.cyou/gtyqridzwg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aizwys.cn/gtshloiabi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhijiandao.cn/gtckrjhpjq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtxfyfskzi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.havefunace.top/gtnukirawt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yanxiufei.cn/gtehdphjpx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cucudq.cn/gtehmcswby.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yangfankeji.com/gtaudwfllr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pengpengdd.cyou/gtsikyuwps.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gttvstcmyc.html

Py:   "ab" * 3
来源：http://hz.xziqi.cn/gtxovlqudp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258.top/gtnaydgfyx.html

JS:   "ab".repeat(3)
来源：http://hz.guannengcc.top/gtnzxpphbp.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtqvdjouql.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtyppgqnhm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xinyue.icu/gteptaltse.html

Ruby: "ab" * 3
来源：http://hz.cdnleiting.top/gtmztahsbw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.daxiang520.top/gtjrizzusw.html

[E03] 截取子串
来源：http://hz.shzxlz.cn/gtjwjaehur.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yanxiufei.cn/gtziqftwrb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9152youxi.cn/gtdnqsibbq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yonumen.top/gtzxsepbqp.html

TS:   s.slice(1, 4)
来源：http://hz.yj202588.top/gtladtysuc.html

Java: s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtgvhmrxvb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.pengpengdd.cyou/gtdwmjxnlm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.9152youxi.cn/gtxwzejwrh.html

C#:   s.Substring(1, 3)
来源：http://hz.kuanghao11.cn/gtvrxclbhp.html

[E04] 查找子串位置
来源：http://hz.jinqigfzy.top/gtbckanoge.html

Py:   s.find("x");  s.index("x")
来源：http://hz.andypj.xyz/gtcjfkqlun.html


<!-- 参考信息 -->