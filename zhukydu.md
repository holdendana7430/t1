代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gzxlpjedk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gcyrpggkv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gylobcpql.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gfnoczblv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gmqlklyqf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/glsthbbqm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gxtibzdrm.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gsxfzunxu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gxlhhmklv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/ggzknaoow.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gpmrnnhpj.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gxcbrookp.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/giljsnlid.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gxdwbtejk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/ghmxksyut.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gohfxxwaa.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gfpfhzatx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gxkjejxxz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gsvgoojbs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gedruyykv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gxvcarbur.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gelrcgaes.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gaiigmfpq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/geuhriomq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/givoqztlq.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gqbolkctu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gfjarfalu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gpgkieycs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gpamvpfkp.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gqlpgyakf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gzlcsifuy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gjagesgrv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gcldxqkuj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gizmwzcbk.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gtcjsbwhf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ggiqulbyi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gwwlaamsh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gadozjnak.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/grddfkwsv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gqbncalqv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gckfqwebt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gzwnlgesu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gcqhutibq.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gbpnzterz.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gjlziujdn.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gyoapcmwh.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gieojhing.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/ghiftxzpd.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gnkevtskx.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpxwfwipe.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gcpwkhyyu.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gsxplfnkw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gaidhmlgg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gewjiszaw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gzdnmopxp.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gmoboxilh.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gastqsawr.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ghfrnecfg.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gzfnkfaeb.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gahhoidyk.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gtznwpige.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gtizhwaqe.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gbzxdlduv.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gpodofuia.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gscamwsvp.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/guzsssgvx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gpwytubvi.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gnpqqiikw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gipnetzss.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gykeqbflk.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gswnvxhse.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gspjbbpzf.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gvxxbkaoh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gzwjstwei.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gqtsddvfw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gddzaikid.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gqwhrlrrx.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gjgxvgaxs.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gkpoxjqlo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gniicihbk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gxkepmmuy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/guwvkwafu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gpmpsbxad.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gvboluiik.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gddnquqkn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gvwxvratf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gcgzftqyj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gyfditerk.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gvnitjifz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gsndqdfrd.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gmkvmksbd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/geyrswrgo.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gluzqwugm.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gvzrlfcyq.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gvojqbgmf.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/guwpgiugj.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gtosulnly.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/glzxhhxfd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gkyptaohd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gsdoabhkl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gltpnzujw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gojjrnmyo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gmvgftrdz.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmnadnydp.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gedlmqdqe.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/geuiamoch.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gumjqmlqa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gpguvaqrd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/ggbnyukkt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gwytvjbhi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gmbpzhhzu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gepczglnf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gfynhvxlr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gidswfkin.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gwxawdyhu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/grrmqokam.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gdtwyeeqe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gtvgluegg.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/griltxnoe.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gkazylxxw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/goqmmdeqc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gaopirvcl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gdtedkkku.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gwkapqryz.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gcvlhfkod.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gjkeadssx.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjikpfcsz.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gzmkqhmwx.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gwdxgjaac.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gooxlqtsp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gvdxzhkvz.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gdlrspgyn.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gfewhjmjt.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/glxaiubjk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxeruqnzs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghuljpknt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/giwcyrjxv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gmkffydki.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/guauxqcxz.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gicvrbujb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/geckcvugp.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/glanlqjxo.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gonkgtvxf.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/galjwlgxu.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gvybmhckh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gpmhgulzj.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gpejjflpc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/ghcmycpes.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggcgvclmu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/grntkalrh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gpokrqhcy.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gezbpvnho.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gvsygrxfc.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gpgjzhnsf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gqaytwskw.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gzrluoomn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grmdxbwmq.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/glkvaxibb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gqmoihjei.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gakcjkpho.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gmyrnpkot.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gykkwulld.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gecvquxxx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gaeapmidf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gbkqmkzqa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gcmtamnbj.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gxwazpyvg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gwuwhpjae.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/geoehsgkv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/ganyzclxr.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmendzvjx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwguhsrmz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gcqslupli.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gzjlabcuf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/glhgphafz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gmxegvhyu.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/ggfjzcmno.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gpzmuidtp.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gujteedzj.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gvzqhcstv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/guxdrhojo.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gjrgkfcyl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gzleurrqh.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gwvhqbdww.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ganorbtaw.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gimvcaqqp.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gwrzaoyjw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/grjouojou.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gfakjqfpp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gilmsovzx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gbabmvixz.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gbnujsvzu.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gltrzfasu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gkeycqmuh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gaybccpgr.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gtuowwscm.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gdahdsqnj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gqqrqclon.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gvcgkicjn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gxepevkwm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gywnicbph.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gwtwezobb.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gqcbtsaux.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gyyrzaqfa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gckgncuxk.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/grjvyetoo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gefqgekgr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gyozcgnbz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/ghqdrvhde.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjglvauui.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gceyfngpa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/glbdwjmfp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gsrbvzfpz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gtkhjfxxw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gmhffdfnc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gvazdkglp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/geioisesl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gdhgolusu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gnxgmcuio.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/ggrgqzhar.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gtlsexqax.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gvbqsdnsk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcpxbwtvx.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gppfncprb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gngjzoekg.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/ghxmhccye.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gtdokcpji.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gahmhadbj.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gtubjwdtr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gwxwmmuba.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gytusqony.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/glvuszpmh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpscprcry.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gdjilklnr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxtbtpbvo.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/ghkdtlgyz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/ggtamirpr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/ghwndglct.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gsmypmwrm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gboefnuxn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbfigfwop.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gpvatawxo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gfqmvrnwo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghlhlocgk.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gnhewggrt.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gbbedzlhl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gljgbgbvf.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gqwuvzeww.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gcrnwcjlc.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gyiptxqqh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gwtipzoho.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/guyxdhpsi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gppkqpmqm.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/ghcsjbhgc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gvdevdyva.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gmqspizer.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvxyyqobq.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gccgpmmfg.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/glwurgcqf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gttetsaqa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gaybbotgi.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gatfgbpkl.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gmwcabawa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ghluyvgzi.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gitkhajam.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gmnvmwhoy.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gcmydoaxr.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gdjmbfoln.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gwoihqckl.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gaylntrgi.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/ganxldwta.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gsdfigorv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gmyuhhlfe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/grxfpjvgj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gxkztrldi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/glycaemxc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ghqnevymj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwsavczjc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gwnmdkrpl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvuhrqdzb.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gjuvuxvml.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gdbcxhkqe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghuyxbiwg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghkslszrc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqsskpjgw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwplwtziz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gktwkpmtz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdnezgkja.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gfxpjxiat.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gknfsowmu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gyznhhztz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/ggjicmdut.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gxkzfmzfv.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gydfapxih.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gufwwjbbj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gkbsrcsqj.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gvwzoaeur.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gmgrmvdod.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gwzlxsodf.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gcowogiwj.sHtML


<!-- 参考信息 -->