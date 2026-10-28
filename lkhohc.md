代发 wailian999

[C14] 泛型函数
来源：http://hz.guannengcc.top/gtrvrqxcum.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangdashe.top/gtcuobnjdt.html

PHP:  // 无泛型
来源：http://hz.snrcjt.cn/gtzeopgjqn.html

JS:   // 无泛型
来源：http://hz.wangshuangyany.cn/gtvvjifvps.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gtbefsjbrw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtucvekhwu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangshuangyany.cn/gttuzblcho.html

Ruby: # 无泛型
来源：http://hz.jinqigfzy.top/gtkrqomhvg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sxryk.cn/gtrkacyiae.html

[C15] 解构 / 展开参数
来源：http://hz.cdnleiting.top/gtzxkscrkp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shuidangran.top/gtuwazmjyr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuanzx.com/gtgrxqhdbs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtjwxtizzg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.0kj1m.cn/gtblfakhsb.html

Java: // 无解构
来源：http://hz.vqdsnc.cn/gtvddzhblq.html

Go:   // 无解构
来源：http://hz.yvedp.cn/gtizearqtc.html

Ruby: a, b = pair
来源：http://hz.yj20258.top/gtpqxvydji.html

C#:   var (a, b) = pair;
来源：http://hz.feifeiyinyue.top/gthpobgvbi.html

[C16] 函数 / 方法重载
来源：http://hz.yuxming.cn/gtcuifkglj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhixingplan.top/gtmuhkjyjc.html

PHP:  // 无重载
来源：http://hz.yj202588.top/gtwjdppyfj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xinyue.icu/gtlehnmrpg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jianghu66.top/gtpmcmokhu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenlongwang.top/gtllyyohta.html

Go:   // 无重载：用不同函数名
来源：http://hz.fengsongda.top/gtkopeilwr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtuhlzvdzv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydjk.org.cn/gtkxpehlsc.html

================================================================================
来源：http://hz.yuxming.cn/gtrldcluwa.html

D. 数组 / 列表 / 集合
来源：http://hz.sxryk.cn/gtifxegwts.html

================================================================================
来源：http://hz.9152youxi.cn/gtbippceeu.html

[D01] 创建数组 / 列表
来源：http://hz.jqgfzy.top/gtsutifbdu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnxiangtu.top/gtlllgfoob.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258888.top/gtijyncrwd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yanxiufei.cn/gtnlxvnvex.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cheryme.top/gtrvarpaua.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.c1oappe.top/gthlywickd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cqqwz.cn/gtuwzuhplf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ivvv.top/gtxghkdprs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gtrbojupml.html

[D02] 追加元素到末尾
来源：http://hz.guowangkeji.top/gtcldjmpgs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xinyue.icu/gtokrkcmsc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gthwdviwsf.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtazpmmwxn.html

TS:   arr.push(4);
来源：http://hz.zhixingplan.top/gtwsqvpeqz.html

Java: list.add(4);
来源：http://hz.zhengqikj.top/gtwptikkse.html

Go:   arr = append(arr, 4)
来源：http://hz.ehwqpu.com/gtzpczdcqy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ehwqpu.com/gtqpjjmmde.html

C#:   list.Add(4);
来源：http://hz.shzxlz.cn/gtgampwhbn.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigfzy.top/gtlccgkmnc.html

Py:   arr.insert(0, 0)
来源：http://hz.zhoulong.xyz/gtegkfzpwb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.fengsongda.top/gtqdkvyspr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guannengcc.top/gtrmqekyug.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gzhubu.top/gtiybeiwjr.html

Java: list.add(0, 0);
来源：http://hz.cucudq.cn/gtdfqiiuai.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.quarkkingdee.top/gtsjfiodaw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.smart0.xyz/gtuvvpmawc.html

C#:   list.Insert(0, 0);
来源：http://hz.redwolf501.top/gtxwqartvf.html

[D04] 删除元素
来源：http://hz.cucudq.cn/gtgwfzqkra.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ybcxt.top/gtbufacsxl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.quarkkingdee.top/gtnofqsmvc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangtech.top/gtruryrjud.html

TS:   arr.splice(0, 1);
来源：http://hz.hnxiangtu.top/gttgujhpim.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.guowangkeji.top/gtkotdglfu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.tianlin.xyz/gtzhlrungu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.c1oappe.top/gtsxapcdve.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.meibo888.top/gtestecybo.html

[D05] 访问与修改元素
来源：http://hz.cqqwz.cn/gtsphbqedb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtgtydcvls.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.mhx1999.top/gtxpgiwmtp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.iojbl.cn/gtwflokrnb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ehwqpu.com/gtplwjyrnb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.svipenyu.cn/gtdetrrjhz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtgbcmcekw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtaxjhvwco.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.fengsongda.top/gtffeaomru.html

[D06] 数组长度
来源：http://hz.bjfxy.top/gtuphnyukl.html

Py:   len(arr)
来源：http://hz.hysaishi.cn/gttkilpirz.html

PHP:  count($arr);
来源：http://hz.guowangkeji.top/gtmmzodkdq.html

JS:   arr.length
来源：http://hz.wangdashe.top/gtkksvhrfl.html

TS:   arr.length
来源：http://hz.sufxvd.cn/gtjxagsxyt.html

Java: list.size();
来源：http://hz.yonumen.top/gtwthncivc.html

Go:   len(arr)
来源：http://hz.fengsongda.top/gtmlutfetf.html

Ruby: arr.length; arr.size
来源：http://hz.jqgfzy.top/gtmfdmuywc.html

C#:   list.Count;
来源：http://hz.fengsongda.top/gtujcccjsh.html

[D07] 切片 / 取子数组
来源：http://hz.sxryk.cn/gtmyhuzhqc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxuanxn.top/gtqpjyjtxd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258.top/gtfgdztedz.html

JS:   arr.slice(1, 4);
来源：http://hz.jianghu66.top/gtcqupyqfi.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gthwmrqpsg.html

Java: list.subList(1, 4);
来源：http://hz.wangdashe.top/gtuunawmwn.html

Go:   arr[1:4]
来源：http://hz.xingfuxueyuan.xyz/gtyadcgjjl.html

Ruby: arr[1, 3]
来源：http://hz.nanxuanxn.top/gtrbdccioz.html

C#:   list.GetRange(1, 3);
来源：http://hz.hammf.cn/gtxirhnupk.html

[D08] 合并两个数组
来源：http://hz.yangfankeji.com/gtunnargak.html

Py:   a + b;  a.extend(b)
来源：http://hz.cqqwz.cn/gtbxqsmail.html

PHP:  array_merge($a, $b);
来源：http://hz.andypj.xyz/gtofoqqxxh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgufenzy.top/gtlnetifqx.html

TS:   [...a, ...b];
来源：http://hz.cucudq.cn/gtjixhzpxz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gtcgjkzhac.html

Go:   append(a, b...)
来源：http://hz.jqgfzy.top/gtqtwyxtdg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.9152youxi.cn/gtqgnxxxyp.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigfzy.top/gtaxflyhxf.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gtmrsguytv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.feifeiyinyue.top/gtnbwtmgjp.html

PHP:  sort($arr);
来源：http://hz.mhx1999.top/gtzmyyyjbt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shangyingyoupin.top/gtfsjwmcxy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtvnnmfkld.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ybcxt.top/gttkkrzeeh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtqdpzpoio.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtvxrqaqlr.html

C#:   list.Sort();
来源：http://hz.sufxvd.cn/gtbgdztlbw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinghuilouyu.cn/gtalcnuhen.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuanzhike.top/gtxmzktmsm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gttplcdnab.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtnxdppcky.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.52xcode.cn/gtbjxqduyg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ppjwa.cn/gtxmlsguuu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ywan-chungtsiang.top/gtochntgdn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gtvpahbmsm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hongshengwenyu.top/gtigwhypwv.html

[D11] 反转数组
来源：http://hz.nanxinkj.top/gtejlkzouw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pycfn.com/gtyzlqeqbq.html

PHP:  array_reverse($arr);
来源：http://hz.nanxuanxn.top/gtzmrhckir.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.kuanghao11.cn/gtuqleyepe.html

TS:   [...arr].reverse();
来源：http://hz.hnxiangtu.top/gtxmbjtvfl.html

Java: Collections.reverse(list);
来源：http://hz.yuanzhike.top/gtespmfusg.html

Go:   slices.Reverse(arr)
来源：http://hz.mhx1999.top/gtpgiitvut.html

Ruby: arr.reverse
来源：http://hz.jlsjyb.cn/gtxundckor.html

C#:   list.Reverse();
来源：http://hz.nwbrower.top/gtivgsioyo.html

[D12] 查找元素下标
来源：http://hz.quarkkingdee.top/gtugaemyww.html

Py:   arr.index(x);  x in arr
来源：http://hz.9152youxi.cn/gtpbkzmzfs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigfzy.top/gtcuswlcfy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtensxjbls.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtuouywjad.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxuanxn.top/gtchveajvx.html

Go:   slices.Index(arr, x)
来源：http://hz.tianlin.xyz/gtvogrxktr.html

Ruby: arr.index(x)
来源：http://hz.xylfe.cn/gtjzaftalx.html

C#:   list.IndexOf(x);
来源：http://hz.nanxinkj.top/gttxgwxlhg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.quarkkingdee.top/gthsuxrsmh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jiagoushi.top/gtmxvkylxb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.birdmap.top/gtwalnvith.html

JS:   arr.filter(x => x > 3)
来源：http://hz.guowangkeji.top/gtrmosyxil.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tanke756.top/gtsozuhqbo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gogol.net.cn/gtslcylxbp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shuidangran.top/gtwkenoakt.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.havefunace.top/gtzhsqvkjm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yvedp.cn/gtanfgqrps.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinyuanbaomall.cn/gtqpjucsbd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xylfe.cn/gtzmznvhyb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.haohaochexian.top/gtapdadwep.html

JS:   arr.map(x => x * 2)
来源：http://hz.dashuyun.cn/gtozswgmeb.html

TS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gtzcsaeybk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zycfv.cn/gtonyoxjwh.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtnocjtmeq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinghuilouyu.cn/gtysfrjgmk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hnqzz.top/gtuuoyhcnd.html

[D15] 去重
来源：http://hz.sysykeji.top/gtbdqdakik.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtpczeasyv.html

PHP:  array_unique($arr);
来源：http://hz.yangfankeji.com/gtynshfuce.html

JS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtrolvaabt.html

TS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gtlsmmbvlw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydzc1.top/gtwbpndboz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhoulong.xyz/gtqryjqyqy.html

Ruby: arr.uniq
来源：http://hz.xingfuxueyuan.xyz/gtffmnsxgn.html

C#:   list.Distinct().ToList()
来源：http://hz.pycfn.com/gtofidlalh.html

[D16] 求和与平均值
来源：http://hz.xinyue.icu/gtqawaclyv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.redwolf501.top/gtosrefgds.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.9152youxi.cn/gtvdoijhwu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gtzqtrscil.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtqvdguafi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangshuangyany.cn/gttaafceas.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtanbqbhzi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shzxlz.cn/gtonhitikh.html

C#:   list.Sum();  list.Average()
来源：http://hz.yonumen.top/gtvhmhlqew.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gtqbgjhxkw.html

Py:   max(arr);  min(arr)
来源：http://hz.gaohongyu789.top/gtiyqblttu.html

PHP:  max($arr);  min($arr);
来源：http://hz.shzxlz.cn/gtxptkwmsf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gaohongyu789.top/gtivsnlkvy.html

TS:   Math.max(...arr);
来源：http://hz.yueranfly.top/gtkmiphews.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigufen.top/gtpazgerve.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.pycfn.com/gtnhqfcaqq.html

Ruby: arr.max;  arr.min
来源：http://hz.zhixingplan.top/gtgupklarx.html

C#:   list.Max();  list.Min()
来源：http://hz.yonumen.top/gtisfyjymk.html

[D18] 扁平化嵌套数组
来源：http://hz.zhijiandao.cn/gthfrymwab.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shuidangran.top/gtxmozdroa.html

PHP:  array_merge(...$nested);
来源：http://hz.zhongyouzk.top/gtpqjsfeep.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnxiangtu.top/gtvcmrores.html

TS:   nested.flat();
来源：http://hz.yj20258.top/gtsirpawgb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pengpengdd.cyou/gtbidjomnm.html

Go:   // 手写双层循环
来源：http://hz.zhijiandao.cn/gtmhwlroye.html

Ruby: nested.flatten
来源：http://hz.zhijiandao.cn/gtxehllfub.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yongpay.top/gtgobftxvy.html

[D19] 按字段分组
来源：http://hz.zhengqikj.top/gtwkggfakg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.vqdsnc.cn/gtbisuopjs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xinyue.icu/gtaruzsofn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtglxhewyt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtuntmksvw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj20258888.top/gtoaeeufju.html

Go:   // 手写 map[string][]T
来源：http://hz.vqdsnc.cn/gtmfsenhhq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cashguo.top/gtyvajlclj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sufxvd.cn/gtepucgxue.html

[D20] 统计每个元素出现次数
来源：http://hz.havefunace.top/gtiloxahag.html

Py:   Counter(arr)
来源：http://hz.yueranfly.top/gtnfqryaia.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gtqxfljapk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jiagoushi.top/gtfunczely.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtscvwamos.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zdqjudy.top/gttqpbtunl.html

Go:   // 手写 map[T]int
来源：http://hz.gotoacloud.top/gtgfeofxrc.html

Ruby: arr.tally
来源：http://hz.havefunace.top/gtrfrbrwza.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jianghu66.top/gtmnueceso.html

[D21] 判断是否包含某元素
来源：http://hz.yj20258.top/gtvmsxsoyy.html

Py:   x in arr
来源：http://hz.snrcjt.cn/gtrcdacuze.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yvedp.cn/gtpzpbbump.html

JS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtluxdbxqd.html

TS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtlozdcrzx.html

Java: list.contains(x)
来源：http://hz.hywenlv.cn/gtkamnolku.html

Go:   slices.Contains(arr, x)
来源：http://hz.feifeiyinyue.top/gtfekiufwe.html

Ruby: arr.include?(x)
来源：http://hz.yanxiufei.cn/gtafupczty.html

C#:   list.Contains(x)
来源：http://hz.smart0.xyz/gtniojjhqj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ehwqpu.com/gtrfrrowkc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigufen.top/gtexalvrsa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangtech.top/gtwverqjyh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhijiandao.cn/gthgqvdupu.html

TS:   [...arr];
来源：http://hz.yanxiufei.cn/gtxqvmylen.html

Java: new ArrayList<>(list);
来源：http://hz.yanxiufei.cn/gttcjksvyb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.52xcode.cn/gtahzrhnrf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tianlin.xyz/gtaoroljdt.html

C#:   new List<int>(list);
来源：http://hz.ydzc1.top/gtgdaidkoi.html

[D23] reduce 累积计算
来源：http://hz.jlsjyb.cn/gtiudpqihf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.bjfxy.top/gtmxsmhzms.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tian-w.cn/gtbcndcfwe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gtwfdeujtt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hammf.cn/gtvqshpxpf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cqqwz.cn/gtsnvkmsmj.html

Go:   // 手写循环
来源：http://hz.meibo888.top/gtqidhhqwm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuetiantiany.cn/gtpxamnwyb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhixingplan.top/gtdpnbqnoq.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgufenzy.top/gtvbkbxsih.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.316326.xyz/gtepcuanmx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgufenzy.top/gtiknkqijr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zdqjudy.top/gteqyfoimq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtyhyhwino.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.feifeiyinyue.top/gtkxuqklkn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhoulong.xyz/gtkxnoxoxq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cheryme.top/gtfbsmlpwk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.316326.xyz/gtwnkgyvxw.html

[D25] Set 集合去重与交并差
来源：http://hz.ivvv.top/gtdxtyeaat.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgfzy.top/gtyynejovm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtxcblceab.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xingfuxueyuan.xyz/gttfydjqhn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yueranfly.top/gtklbtvgkz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.fzhhl.top/gtwuhzgeju.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aizwys.cn/gtaxdtmyej.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhongyouzk.top/gtxyyqpjjk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xziqi.cn/gtnmfymexn.html

[D26] 数组转字符串
来源：http://hz.0kj1m.cn/gtltmxzhli.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gotoacloud.top/gtrbfpbapi.html

PHP:  implode(", ", $arr);
来源：http://hz.quarkkingdee.top/gthkdssfvr.html

JS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtnglesrkj.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtqqizwlup.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gthskcsppe.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gotoacloud.top/gtktlzoync.html

Ruby: arr.join(", ")
来源：http://hz.haohaochexian.top/gtdrgjczxo.html

C#:   string.Join(", ", list)
来源：http://hz.cashguo.top/gtoqbripwq.html

================================================================================
来源：http://hz.meibo888.top/gtsoqkxiai.html

E. 字符串处理
来源：http://hz.shangyingyoupin.top/gttqliyywv.html

================================================================================
来源：http://hz.xylfe.cn/gtoqcvbyha.html

[E01] 拼接字符串
来源：http://hz.jinqigufen.top/gtwfojhrxc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.feifeiyinyue.top/gtffqnmllq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gaohongyu789.top/gtpjuqvhsw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtuchrtgps.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtjwdwlbdd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.quarkkingdee.top/gtpgokirrw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuanzhike.top/gtuvhhizvv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.c1oappe.top/gtgoumpspf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.smart0.xyz/gtvkvkkosv.html

[E02] 重复字符串
来源：http://hz.yj202588.top/gtmustxgbc.html

Py:   "ab" * 3
来源：http://hz.yonumen.top/gtclrsyoki.html

PHP:  str_repeat("ab", 3);
来源：http://hz.redwolf501.top/gtieveiyss.html

JS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gteevsayrs.html

TS:   "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtrksbvoid.html

Java: "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtgoocsooo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ehwqpu.com/gtdwvyznhf.html

Ruby: "ab" * 3
来源：http://hz.jiagoushi.top/gtrsaihudk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.iojbl.cn/gtpkveckyg.html

[E03] 截取子串
来源：http://hz.snrcjt.cn/gtoovfxyaq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.52xcode.cn/gtqnoxquqa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.dashuyun.cn/gtrebeilgf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.iojbl.cn/gtskxvlaxy.html

TS:   s.slice(1, 4)
来源：http://hz.jiagoushi.top/gtpsjjzmit.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtkhyglblr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenlongwang.top/gtvwyjksil.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hywenlv.cn/gtabpallzy.html

C#:   s.Substring(1, 3)
来源：http://hz.aizwys.cn/gtxhucnfco.html

[E04] 查找子串位置
来源：http://hz.shzxlz.cn/gtniegfumy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sysykeji.top/gtjzfigbue.html

PHP:  strpos($s, "x");
来源：http://hz.tianlin.xyz/gthjotpryu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ybcxt.top/gtaraqkjwt.html

TS:   s.indexOf("x")
来源：http://hz.hywenlv.cn/gtgwnfidds.html

Java: s.indexOf("x")
来源：http://hz.hammf.cn/gtxzzgnkzs.html


<!-- 参考信息 -->