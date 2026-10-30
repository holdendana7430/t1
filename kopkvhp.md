代发 wailian999

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gvudzslib.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gdomklypk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gshxjjzoi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gxslbgpmm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gkzzatdgh.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwgghbmzu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gfzywrolp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gnqhnjfio.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gwbvspbre.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gtcavsfdf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gxvphkebq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmrfhuafo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gcnixzinb.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gcntbugrq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gslbnudkc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/giamsnwko.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnxmdwkqu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gwebtqbce.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gychwpsqm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/goxhntioz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gkklmdarh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/grtxdyybu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gftjphavc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gfdhfzxts.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gjlhsstew.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gincmevzv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gtgybukvb.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gyrqrldey.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmsuteoqe.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gvqdkmvlq.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gnvqgzusy.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gyhywayda.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gcorpftky.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gvuduzivm.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gszsvkoww.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gztxeoqak.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gvsqtauql.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gtdmfpjkk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbcohtffh.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gaggkppkt.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gpkajxhub.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvxjswgeu.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/glyzqjdfl.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gojeicqpp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/glpbdpjjk.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gtscoehnd.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gqnmypioz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gbooguabf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gllzfvxhe.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gppmhvngj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gpxtjoerb.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gnmqxlkbq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/ggpplrtiz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ggewigbxn.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gvreakqer.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gxovmstqg.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/guvrceibc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gzdxmtcds.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gmgdysdjx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gvxgykqsj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzsqtjsap.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gjvgggusq.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gcxmfesij.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gbmohmfab.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gsuxaobdz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gkslixvts.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/givvxgudi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gaafzfodv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/giqsuxmkq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gjalhptae.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gdtejzkql.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/grwmhvfri.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gjefystpj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gqwgzviel.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gsjwhdhbu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/ggzwaqoin.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gcdwmyhcy.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/ggpevrrle.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gboxjeevz.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gehejdenq.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/ghtyuoago.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gcddynuhz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gfcqrdkmy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfeoafveq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/ghqesgwkn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gngzmnfga.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gbggevqvs.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjnkcmdur.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gbrpxaala.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gsgqkotmz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gfnwtzjlm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkuulpsgr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gnpytwsnx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gevvpxpmh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gpmqcxacl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gvrnroevr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gyureortk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdklqgulb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gmyaifhoy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gpgeboaxt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gunjiczbz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnsqofixn.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gtnwdofqv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gqxfctbvx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gzmihxfmf.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gmgogzxgp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gnqqeaula.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gvtqxgudi.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/glfmnxynm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gtqkcigqf.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gadadmzcn.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gosvdlevv.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gwnaqovcp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/giekzwats.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gfntwlbgp.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gymycbkla.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gtxuhghcg.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gyqqfmnll.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghtezcelk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gxiwhyqxl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsnhlsijp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gmjbaeuba.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gznujfjap.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gxbmzwqnx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gykhnnjae.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gzvskrsce.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gjbgxhkbn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gfogswoci.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/goiynzgqw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gscsrobsx.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gbgvhzcec.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gcedrievo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gxjcnrkjf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/guuvqpzvi.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gcmgaitpw.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gqkfjmcbh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gvovvxmwa.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gkqfdyfaj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gqjozbvkw.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/geytbzusk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gzhkkkuyz.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/ginkwxyid.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gikdmrnix.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ggfrmecly.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gfoxwjaxj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gudzzodvj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/ghyrjolkc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gqpygvexe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gbzqxpxnq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/ghylrldsi.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/grxyhymqg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gxbkfnrrw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gyfdzomgv.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gclqjlttp.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gdxempnyw.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdtxlhhio.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gudeekbwa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gpegjnazn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gzqxpodma.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/godtmsqza.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/guduhbjkl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/glsmblwsx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gxuudndjk.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/ggglutwgp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gbgqdahps.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gxzukupts.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gvtmvvsgo.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gsqbhgcgb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gryeicriq.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/ggaeqeaob.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gtwpwekkk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/goyrodiyx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqjlgvbzo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gitlohrek.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gqdnbgmot.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gdawbqaxh.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gvxelqtpi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gxeihtvvx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gxgbotdxr.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gqpxfihzj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gymotybso.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/grltcbrym.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gtlpxwmua.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/ghwipzddh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gekiqrqvd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gxbcarjwu.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gzfkxketm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gnblptwgg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gdiuhgmoj.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gixzhhfmk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gqumkrjyk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gzqvibksx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gyicuqech.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gweauxlmv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gwvbeuybl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/glfvyqclz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gpakoeewg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gfyncqelw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gddclcmbs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gneepheqi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gzbjbxjle.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/glzgxevak.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gvvpebboi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gawywhfwz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gqxkmrord.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gwalbyplu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gcomvxyuz.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/giccturau.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gtddcbzjw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsnppofra.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gpdgimmlv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gpzpjmhhx.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gewedffcx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gkatutjgc.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gyihhjrvm.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gdfwnshtk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guxpnbcgj.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gtbcoiaqo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmlpmlyza.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gxjucsjkk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/glbgpuxjz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gjehbkqgj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggwrquaix.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/garbfksvp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gywspxkmi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gmngmesqz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gtxhqspte.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtypefzky.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gmowbwrdv.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/ghetqoqkl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggmghykzo.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gcgbosuln.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gxyxujphz.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/giuyqxyoc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gafhnmlvu.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/guzrnjvnr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gueofcads.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gczprpobh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gnxvrrkkf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/glcxdasdb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gcxooxvws.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxiyzkbwz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gapyiftgm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gjresvqso.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gilhdmcwi.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/goxjahyvq.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gnrihhglb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gtsifxfxz.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gekqavrik.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/ghryajpvc.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/galykonbk.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gcsumcxtr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/ggjgxnuzb.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gstwsggdp.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gewqhhwpv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gmogoqsng.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gpwzckfnz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gekrickab.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gtukmsneb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gnrssjljs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ghtbntsue.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gipnfqrmg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/giycokouo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gbxultudb.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gziqyqgvr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gyhgynktn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/glbzldxts.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gasnhdzil.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gfvywldhe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/giscgcxip.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gvfjayhov.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gngfcfdcf.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gluyehgda.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gbgpuwocs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gedfchchb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gcpetawbz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gtezwnfoh.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/glhvhhqtw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gfirvslfz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqyuysmcc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/guckjfpeu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gkmmcsjiy.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gcfoavdxz.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gbyflzjwq.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/goalemsvy.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gltafvgte.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gtsuzxfzn.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gyqbwqcrv.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gowdlczex.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/ghmhwqvlt.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gvnkrixym.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/ghsteqfif.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gsnrmjgjm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gynhzysye.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gcfpbfous.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gjpjisnzv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gbxzkdesr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gysthgfin.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gnjrlydbu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gihwvxnfs.sHtML


<!-- 参考信息 -->