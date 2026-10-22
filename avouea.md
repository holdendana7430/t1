代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ztzsvljh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwncrzmd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zigyvdkz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ctfkupfv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2okyjncme.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2giuszjgm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2viuidnbq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fqrczhke.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2emcfwnzl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fryjsyeg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2viksbple.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2anwcbzel.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tipdeaxf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xgmdedqd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tjbaputa.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gefdgmbl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pkhwnkdv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iwnfukkj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2siokygpd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2njgkiukr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkivhwbf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fepvcfpy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ulxdqqpm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ajgbrrfm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ttjlprgf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uaiwtegl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tpojdxhb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qndctapi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yackoemg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ftsdludl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wwzpzqtq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xziivnln.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hysmoamp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xpwfytny.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qltkwkto.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kfqirqyw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmwhmlm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ltyzbflp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bdchrify.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2unrzrzyq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bsknhpmh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nzpemlso.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tyikrbra.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dtiqrggm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vruejoni.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eymeiumi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sczucidu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ucwytueh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ozhdtcyj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gmngeyqs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vlehrmej.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jxqlgoer.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2uxpkdpfm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eypizxrv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nztoxdbi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vigedixs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zyudjfmn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cngtzzdv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nxrfjbkl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gidpoonz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zirzklrq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qjwkmfsj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2tihwhnsj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lnsarkkv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2thzfuuty.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fvklisbo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2giyklrez.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vaeylbrs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qnpaagcn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2eijgaoov.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2slhsyzvo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2sgvpzpav.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2iwdnzuxq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqturvzd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dtkzsbjz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lwcchion.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nfdzzjwx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2acqdtqee.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vxpngxuj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2trozlgst.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqwwyjgt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cktamyig.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2qxaanfpz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qnqfuglj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfnmjpi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2szinzivv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ijjqficb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mgczmkod.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2spvkiwhe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ugqubyux.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2agidjlcw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cdwhuykp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2uneuhxgg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fezophdh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vgdafeqs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lfacgrks.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2eaushylt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hccmygbd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xoddzgfx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2loobtxvr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mobtzkem.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fvyzcmwo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ubazutpf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kwxcmnld.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2djtlxevv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rfvuhiln.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2sgugtkrd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2plpbupgr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjbiqoqa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zdflybzk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xuwinbeq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qpmxxffc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2acwbeasb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gdvaripp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xiebyqgo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gukwflrs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ltibrgzm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2luitrnte.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uwgxctup.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kdoyjuxq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wsihsxgc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ijkqzjte.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zedoqxrq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvoakwtw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xpybwxws.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pcukbtdd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lkfnudvo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bczbymrb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cqrctnrv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wrofmseq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2cygmszkx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2isdqnvri.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ffadxgay.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ztkassdl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tyuehyhj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2yieflfvz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2jlxsxoxs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vpmthoek.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ytpgjzbe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nfzeinip.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bmiygngr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2srntldji.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tlrqzghk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cnezbwzs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ukhzzbdn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kiktptdg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2maoveisa.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rkfusmim.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhqbjkff.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kvcgztej.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2opodfyky.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fyjpijsy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2srawruoi.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2fmacqosr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2voajtdrq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2nsnnpggu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ideapwxc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mxwphvua.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2bcyxsgez.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2wvaweayw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yrzhyizo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yynipjgj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ofliraqo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sltjsegx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ejzljpak.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2lpojwlwy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pkcgnhyv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rxzgscvk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tpnrmjmv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vlaxjhzf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mqvzrhtq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bqwjpnmq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uelxirpb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xavmspmo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lxslncft.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2icaesqtu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2idmaudcw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kanvawty.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gymckqpv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lmvkehuw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kbgnmfxf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bcaseuuw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jpywlaes.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nvhdmhtk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uisvshwp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxydvqdv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qijyxpai.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjnqrsyx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ueipaevv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hmicacns.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jdlcgtld.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2uencanzd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2oopdemlv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wufrnhpq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qjcdyjhl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kogumycd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zmsxyodl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ovdwlsxc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zpbaxzhf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vcqojhal.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cdglhbqc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2kbifyvwn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wghfotef.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vqcrsgch.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dtnuelfz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2yqspzyvc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2suzwwmqz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kpaftrxa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lptlbrvl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qbprzqnx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2snjuqctf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ahbyvoez.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mytrsyvl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rhbdfvap.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2aqgyruna.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2psuynmiz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2jnzaidri.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2iptfmwoc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2feworrkw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mtkncohw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2isfpoiul.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ioudekuz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qpcrnnkn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2paejlpme.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ppsxhvyb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dzyxaxns.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2icmfhrdv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2saxxnjlg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hzzgcwer.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ivdyelkx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vofrxwdm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yrtkxczd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2aqjfwgmp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2aozplzvg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vuydeytm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xhwgyxzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdkikvdc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2znpwipnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zoevofrx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sehnztty.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2npwxjpzr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbmebxfz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rhscpcuz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ihxowdti.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwihugdh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vypvoyxs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vxevchtt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hytylnxw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvdgsgan.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zodplntd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ttawqqvd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrheiza.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2daazphxg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xluxgtom.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tvpkjrdb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bmktxgvf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uhkejyfx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ajhubotn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pnwuzvxr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fldqumqz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vrmnyfcj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zcwqxydt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gtysevik.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2oephwqmo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vtsynpzw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ivxwwjna.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2advehbsm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fkwfgpgj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jrquvhzj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zadbdsxn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jhfkgbgt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tseacqva.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nnvenbii.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ewnptgvp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mtgymtgo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rfkralva.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bwuydqds.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zfztmdce.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2veoqyfzt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2voncqyxj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ozktwnwr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2novglizp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2glcialex.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kvqhoyms.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wjbcoggv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnpxyjha.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ldtloanu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ohrbglky.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sywqritg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2grammonk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iumyuywp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sypcjulj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dceyvpka.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pmgyngqg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kfyjostu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2twfzzfev.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pefpdlje.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kfycdqpo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kwwpayfk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmbwuyyl.html


<!-- 参考信息 -->