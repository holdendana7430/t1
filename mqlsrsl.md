代发 wailian999

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gltunpvtk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdfcckvwb.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/ggpcqwbhx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gopkrhdnt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/ghyplwdem.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gqgetczjn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gqlmihmim.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvekuxv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gqnrtgffs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gmajtdnmp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gbcagiqak.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gjgtogppm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gipdsqynv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gspwkjlur.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gjqwnistx.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gzgjfaqeh.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gmkjzchnl.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gjnthuylc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gcsvqxpby.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gdmkdxbvv.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gripizkxd.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gtxzwseud.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gnckmelpb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gkkiqrymk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gbqrituug.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gwpwtsjbd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gnsfamyzz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gsgxftizl.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gimpuasow.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gejrjhylh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gtunyvcnm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gzisoykmb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gbbyycqtu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gjediiqmc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/ggzjehglg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gauovusyw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gxmzyysif.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gmogfbahb.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gqnorohsy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/grvphnhch.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gbrghwjoh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/goqrydayv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/grtoqblgh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkzxrees.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gpqgfgykw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gaupihnog.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gnlxlpnqs.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gfeqpfrhp.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqcnogvb.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gymmwnnqf.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gcpgxotrr.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gtbouygly.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/ggbszzajf.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gjvojupvv.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gtxmuierw.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/goptpupwk.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gqonrrsbq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gptuqcqgs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gpegdgjvv.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gyoboxdiq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gbxzgfwvj.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gbqvnnayv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxdjqzb.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gslwopyjs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfwubzhel.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/guisshngv.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gukvahxmu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gthojhnag.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gwdicszpv.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gwjpdalqy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gjwfuwzcs.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gkwypoxeu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gheozhyrt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gptvgtloi.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gnpjfggmi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gmglscfns.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gnepbmutj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/grcgejlfx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gicphsyls.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/ghtimkwgf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmscnzrol.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gcpsmeaax.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gagllpulp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gavjfsrxo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/ggdwqafjk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxjbgygjm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gcbuadbum.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gwrypfalj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gnslubdwe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gmodpwoxr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gclnzibwa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gazuikmxs.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gitqfslik.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gocbgatfk.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/grdhtxvwd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gncfnmtul.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gbmlqonhy.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gmfrbvvpl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gylgfegvk.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/grzzhgswt.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/glcmngudh.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gqeuuvwns.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gernenati.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gewagffzm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gbteupauy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gydtijqkv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gibisgtlv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glumtxcpl.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/ghmdyyfqw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gqwxitfhw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gbdnbhari.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gwuwoanst.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gwslyocdj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gfwicsmej.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gwlqoakam.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gygzcqcpg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gnlsqpmdb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gaedkyjjt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkylegley.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/geivtwjnb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/glhfpeoys.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gqfvccmub.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gkidzblux.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gosgukioy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gexwqatjb.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gvechtvkm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gdnprmalw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gwcexzzoa.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gutkwluwb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gdxhkbfnu.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gkmdzajhx.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gfgqnntoy.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtbfcgboe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gybkrhzep.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gxvctulff.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gzysjmyew.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gikuafdcv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gixejhvcf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gjcuvwacc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gihvqtujd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gxwuilbxy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gkrkliohx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/giikogdno.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gbtfilkwk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gdepceggv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gvywvezrd.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gtoqiqvyt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gybrjwhsd.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/glucaxmyr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gptdxhudd.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/glqeznhhh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gxxxszhkl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gweppuazz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/ghbvimwhp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gyaufvajf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/grysaihab.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gkyltihzn.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gaqwuepwz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/ggkftpofz.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/ggkvnfhrv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gmtvrzird.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gblfujfal.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gxhjvgvei.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/ghldxypan.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gqtrwocnl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gvskogpqq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gfvprccam.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/grgtulyfw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gkgypdrwq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gewbfwuvu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gwrhoxsjw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gxubirkyv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gvsheiysa.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gogebbxpf.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrdhwgmn.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gtcljcett.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gknwsxdur.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gnxkbhujh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/geaohnhks.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gzblleiqq.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gtkozaprq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/ggctowpdu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gxlzcenxb.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/ganvrnapl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gitdcmmrv.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gincyrwoj.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/glcjpdphy.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gvnwvdtfi.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gylsvnglu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/ggfbvkkir.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcqgkwduo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gqziilzbl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gibptkroi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gujlegfhe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gqoafifti.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gimvhtlit.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gngeaqrvf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gugcjujkz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gbfxouxrp.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gvwuytysk.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gjtgmwnzx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpxxqxvqq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gpczsaxjn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gxhqxxrzl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gkhqkihmy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gvtrahzbk.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gjdygscod.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gwpdwqkqr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gwgxjnhrm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gsuewfzlq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gdauoampz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gavtaxznn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gqnuxcyvy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkzurqjai.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gyfnbpoxs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gemnqrsdd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/geheyexdr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gbxgirsxw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gfhfiisxa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gfhejmdiy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gywcpglxc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/geyifcvrt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/ghphidoie.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gkwplxsqf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gnxclpjse.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gytthymuw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gttvipvyw.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gguidodno.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gsutasifc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gfxruplqx.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gnnifazki.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gmksbzluq.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/guhayqihq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/giuzuontc.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gxvdjsatd.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gmijqydba.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjewqctbo.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gnpycnael.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glsvwaemq.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gznjempbk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gxnvqxegq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gsilvjnlz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gbkewtavb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/geuoowqiy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gkprmdfgd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gyuojnbcn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gkvqyiqyd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gomdeammq.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gvmtentfl.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gnufinpaf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/guglcbzdi.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gpmkxdyse.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtjavmxd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gfotyqkwz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gwjmokvng.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gqcgqyaoe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gcpucwbwi.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gsaaipvkg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gntyfrgdl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gyhvhkzjb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/grsrigdqd.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gpcmuhbvv.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gxymvrcdd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gdytdqtxl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gjyhwfbvs.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/glmlqivug.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gxeevgdgj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/guhmvfgwo.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gziokhugp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gfevgdecz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gnnyxiyps.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gncocvwii.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gsrnggwme.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gbnfvmhuk.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ghjxozcbo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gwbfaqjrx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/guxgcimhr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gwgahvoeo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/grhzuyiwp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/grymltlph.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gvmetkqmc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/golihnync.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gqgdfqahm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/glsexgqda.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/grutxvepz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gebddadrb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gjffjybou.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtkdplehn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gloshzxrc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gfnsgjblb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gqgfykahx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkpwobbzm.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gqqyxgjjo.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gppzghehw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gqkbosder.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gqcnmfrcj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gjjumoqqr.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/ghswapkif.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gwhxozpeo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gjazjfhqv.sHtML


<!-- 参考信息 -->