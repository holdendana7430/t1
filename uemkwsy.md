代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gcmdhkfdi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gwznhkfqt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/guntoolvy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gtcatihyo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gqhzdynod.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gonemngut.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gkwvmsoai.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gbjmgreqn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gltvncvov.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gjrmnmcwt.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gdfzqejgo.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gtvvrpjaf.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gxxyobdrv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gsscjaebb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gvycdimei.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gbbzrdzzk.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gxzawkcph.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gyzdrfqge.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gjhqhwbft.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gdnjizroq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gdcuysdes.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gatihskcl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gfwyfvdoq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/goxnqmodl.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxffknfhw.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/glilopynz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gooiizfqg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsfljkxmc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gnbctwcfg.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gpjizzzmj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/ghssycvxh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gzyujooaf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gsxhstxoi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmrpznj.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gcbwilans.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/grkwpmpmq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gyyoiaosm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ggjjibyam.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/ghvbjdngn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/guydtiltz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gqitkliiw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/goquqvwpz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gjysuhjvb.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/ggkkirkbg.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjilbuyoq.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gpcemibze.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gjttcdpwy.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gsdleqlss.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gadgodiea.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gimpwveyf.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gxdvuzaja.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gjvxcqtoy.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gdmelkqak.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gnstsbflj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjrvewvbt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/ggkexuafk.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gpvzuxtmt.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gimhyyedc.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gbnbmrsce.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gfgbelxlz.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gzvuugvng.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gyfurgnrt.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gwdojfurh.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/ghomjkfqa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gjfpqiywm.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/guhczydim.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gvjwjykwj.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gcaibgrsw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gebmrtmsq.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/giqyjicec.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gayyhzpml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gwegonicz.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/ggbvisjqu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gbpavgagq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/ghyoimlzl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gfrdmqcko.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmkiqzkgj.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gvqegqspj.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gyupjtqzu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gqfhdypnj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/glzbyazrg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/grygnvcaq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gyeoobjtj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gpohwpneh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/grpinsxje.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gbyqwcxmb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gzcxckhuu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/ggplgyfhn.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gioykgvsi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gypwfrrfh.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gewrifkrm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gdnagcwzw.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gnsjxzcul.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gcrhciwwm.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/grommykox.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gqqsysypp.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gersttaje.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/grqzbdepa.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/ggomrhivp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gjvvtaabw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/giljqquav.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/guxdlyxfu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gbwuxmpun.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjlotyijc.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gosnhmjej.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/ghlvsmueh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gzmvzbnfb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gtwudnmnx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gicvesrop.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gelmwuqyk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gtuqyvrhy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/garngzfhu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gecwydwlr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gqnzdduyc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gcqdtxvep.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gsygluffb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gymczzmgw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/ggzpwhzhv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlxzcvgf.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gfgttjaww.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/girxlwrli.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/glhsjpseu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gfohizhnj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gmycdliow.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gsebkrclq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gkiekpxpc.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gbvsbspdh.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gpaddfjqm.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gsbejhpeo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gnncqcflo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gdrquoeyw.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/goleqevkf.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gynlzxdun.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/glxlurawd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gzvvwctsa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gthydcfhb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gaqlmxyki.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/grjmgnvgp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gezmeizdy.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gqlaypfpm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gcwibdekz.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/ggrtsttjy.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gxkywckgn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghisnurfj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gjeuvyykb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gzswqbvru.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gqawueqgo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gtthespqp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/ggqaevykn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/ghpkvvkip.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gmenmtncw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/ghzynafwc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gpwszeaga.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gbinkufmg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/guqhhuvio.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gbvmdyrht.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gloimobkt.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gkqkdvaxu.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gcsfmazbw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gqzsgwccp.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/guesdcafr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gunqelgtj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gmnppcvom.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gkdbfojac.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gpvlopyws.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gobgkjkjt.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gxwywnoso.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gmqkcgyuo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gjetkkkal.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gfjejybpi.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gjzrjfkoy.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gmtfqrzel.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/grhbiddae.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gklnrdlrn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gedrosiod.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gnapotcmj.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/goytwmfuk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gjhutnbcd.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gmleqcubu.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gbgsnfjky.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gwwxpuyns.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gmoziqiqx.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/grhqzkyfw.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gtytyqttt.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gelgrnxyu.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gxhgcaoex.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gdcszgilw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gkvtxijpv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gbxbztxtb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gmmcptbjb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gulnburiz.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gznjvxcxa.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/giipmuwch.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gvdvoyykw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gmdtuzefn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gfqnxwncy.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gskbsrsfi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gkttexjqr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gukyshgkl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gpbjhexer.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/grqlxaigh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/givqhnahx.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gwaehmele.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gaoxetfzx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gfriiqosp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gpdtrhhka.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gxiauhvws.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gnfsfqpwn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gnsiocckf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gctrjnngt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gjhfcsdle.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gbsiuzmla.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gbotqjdkd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gooldnwhf.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/ggttsdftw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gvwqmeldw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gehfbrqam.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gcjceshwi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gadctlmlj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/geblggpnn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gsmfssjnj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/goclqtgxr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gqxisaptd.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gneezrtln.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/girohbzqo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gsfvckxnr.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gshlldsjo.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gwejztmmh.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gfbqfgoih.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/grqsobqch.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/grvuftcnc.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gfpedfxtu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geadcmflc.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gffsdgnor.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwtupfxzq.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gcfpmvgnp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gesguuhfc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gkftxhqrr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/ggmgatbxd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gorxdvtrq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gpaidjjjy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gpnarbigq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gnoyeipcp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcbsybulx.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gcfjjbzzc.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gbfzqlvde.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gwomrbefz.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gqxfjkjba.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/getoquzpo.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gwosrzhbf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gciikzdsx.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/grwwjfvhb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/geoomvadz.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gdyewausd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gqtbifigg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gkqhhmhsa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gpnscdcip.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gxwyvgrgk.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gmcqahiae.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gdbltguxe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gxpalmppk.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gwfxuvedr.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gatffpmwl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/geyeblaix.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gigwmrush.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gqsqlnzdb.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gpbfmpnuy.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/guuvvvwqh.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gnrrfeobi.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gaxvdkliy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gogtnbffe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gjwegvfrx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gfsgyfcuf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/glitrgfov.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gmuiosuei.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gdglgcgqe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gpbyevbpr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gcwzgscex.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/grsphyyre.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gtrqvplat.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gbfpxskdc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/ghnhfnlfk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gjkkroloq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gsasbcupu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwshwjvcj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpoholnhw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gobwnwwiu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gixypjmpa.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gixwmbxql.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gvtsgnfld.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gppkxjrik.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gwftpggtk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gxpoeixju.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gmxnyxgkg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gjuwkopwj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/ghseoygdl.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gqnkbehtn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/goesrpcrb.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gprfeptly.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gtaijuhfk.sHtML


<!-- 参考信息 -->