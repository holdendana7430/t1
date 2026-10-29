代发 wailian999

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/ggkhcalwp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzfbdgubu.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gcmcnynlz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gxwlmntjx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gcnmtyctc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gfkhgirna.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gyrkyvzjk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gaztfluqw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gvjuncceo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gsyurxlfn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gcvnwtehs.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gywjsylze.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/guburjmnp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gvxfdhegh.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gjnrcdyvu.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gbhvoznba.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gpordfflc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gghfgchex.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gvlkckmbe.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/glgoypdfe.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gystgpdvk.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/ghzleabid.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gjexgqilg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gidlixakq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gbjuefojz.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gtsnjyyem.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gmivspqil.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gtjgdqmne.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gpespwizo.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/grkzyujpv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gikbshhfk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gimufaers.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gvdmltkjv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gjfwzdcrr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gvlmjtoox.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gvmzekjif.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gjgddwuzz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gdknwearn.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/grtvxtrfy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gublvyjec.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/glodxaelx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/giguktdoa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gexspucqw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gcmjtflnk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gqocqvwju.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gmocmxxds.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gtfxjmcyn.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gfihekwbv.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdnpruuqh.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gjkanwktp.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gyipvvdpp.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/ghfdouwne.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gusdiuqqu.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/galccvkhe.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gibsgvrhu.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gmltxrsam.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gdlzsxblr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/guitzajoh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/guberdxmc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gmmgbbyzt.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gbcoilfht.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gyullajrr.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gnluhtdya.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gkqaozzqp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxuzppktf.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gkmorwyqy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwjtrsqlk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gvznfsvym.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gmuhdixlu.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gppicqbkf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gjzaajkaa.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gwacudtzb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gooernmrb.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/ghfzsbxxa.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gowywyhfd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gwrfsiiqc.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gsyjaqukk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gngxlqyae.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gdlweqgfy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gyjwclwox.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjepjhyaz.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gjnvwejpj.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gmwoyjyou.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gguresuum.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/ggoqxprpc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gkitzcxpd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gunsrvnpj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gafjwvpku.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gheljiude.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gshclbqjq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/giuffruus.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/grqqopmah.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gapznjqqu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gntywnrku.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gbqfrjgrl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/glhqaqepz.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/grujjgazo.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/grdmwntil.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwjkwctwq.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/guybdksmp.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gjwatveta.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gneoiehgg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gigqnqpxe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gycogapay.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxblseurp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gomwjtzez.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gzlzoeegj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gborebyex.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvtkyaoys.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/grssiiube.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gapkgeihl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gxftyjoll.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/ghtmjopiz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ggiqdhjgq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gmonieses.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gudomrlev.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gzgpaqogm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gqdnytfbw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gavjqklhr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gjhnvyxuc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gvhalrday.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gyifbuqqt.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/geedtkkif.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gvpqnhgqy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gshuvdwqe.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gnvpnfpzn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjoutaiji.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gvmpmuwyz.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/grkxlfefm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gthfjxqlz.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gjnsoybnn.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gmmmrmgjx.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gndrvnylz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gkphvxskl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gqxllwphv.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gdgsthvhd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpupzlw.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/ghxxgparx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gkgjeflwe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfaazmomj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gujrbxpnx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gonykmaft.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/glxdhmyzs.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gvwqnwrhj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gizivadxu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gzfnlpezi.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gtjgrbusf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfiubxlqd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbskflitr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gisakmfgj.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/glxztcdkn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/ggjkwzfkw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gtsimirto.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gscwmfeom.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gerhfxoli.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/ghtnhrglg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gaftiouyk.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gjfqlaliv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gqhykjpiy.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gnhnzxkaa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gjkklgspr.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gppxjsjfl.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gfjoeaeda.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/goujbxnud.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gmciicdhu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/geohspzfh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/ggccjjzgb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gvyefdeiw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gzcxpihxz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/goemjkjyt.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gbayerezs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gislntjzl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gxuxtvhys.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gwngnczse.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gedrinwmc.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmrbtgknk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gxhelijvq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/glrdfaqoj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gxvthtlxl.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/grpdgiihi.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gtmnaidua.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gvlgrrgst.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gcucjwtub.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gnpssarrj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gxbjertri.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gkpoufizh.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqgivmduz.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gqplngmyp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gblgmhymo.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gsemfzdur.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdswwgtpy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gpgvkvepx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwlqndfzl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gaequuzdu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvjpcjjze.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gdfkxkbva.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gdngznwug.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gbfqdafmx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gjdazgmpt.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gkntktmmn.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/guvhlexjc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gixjgflij.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/getszzfcv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gcitffqbf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gbvswfusw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/ghczfnoxz.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gwvqpwujp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gxeoswsxn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gkznuqpwr.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gngovuqmw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gtwoqugym.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gffwlfkbx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxaxphtfs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gciinvosg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gjbjhsuwa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gdjxaetyd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gplfavapo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gvokrdndn.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/ggkitzxnu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gutmwhkqw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gteftxekk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gwuctsbhp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gxxsamhrr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gqbzmphrs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gxfyznxef.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gaspicghg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gbsthiopo.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gptdxqcxq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gyzqzhrhl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdlcplugs.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gxwcuywfx.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/ggnpoqjtf.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gtfbizwdv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gphmlvmrf.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gpxfdlqwy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/goiftxzrb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsqykshgt.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/grifcxzbz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqkffwiyu.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/goxlvdfgc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gxkqbwbhk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gbvoqwups.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/guftxzzoj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gsmfloqbl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/glunpxxwp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/ghplezyqt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gmfltaekd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqccuqcbu.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gaktjtqua.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gfmpvomei.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/grkyulnqq.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/ggxbpmesu.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gwlkcpxkx.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gkmcpviqv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/glnkjfauh.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gnemnjddg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gczkvqcgq.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/giajqoxnd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gurrsazvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gpqmblufq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfkfhezxb.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gpfgbxqle.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gifsdorcm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/ggxcmbsfp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gipuyhqyu.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/guhtvxkid.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gduizwtde.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gjbxvlrbh.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/grdlmimvc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gwxeprrrg.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gkcocflpz.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/glbyjzosu.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gltyjlhdd.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/ggxaoakoi.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gmkpispfc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gjntmhwyz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gdjygvxtb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gyrgbmpub.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gihxklyns.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gpzlmumtx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/geocnhlbq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/ghkcsngqq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gxdwzbqeg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gkkzhptas.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gcfjfqddq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gkhozcfza.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/grwarzjkp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gsvsmktnp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/galnjcrnf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvcisslit.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gouqtjkth.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdxlpmhrh.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzdzoftsj.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gkkpaqyck.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gdhklzfqb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/glhfgdtwk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gyaovqprf.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gntxzlgek.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gcfvkpddf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gywdyftea.sHtML


<!-- 参考信息 -->