代发 wailian999

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gebucwjnk.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/glmsbzikz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gpwyritsu.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gatxpuftf.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gutxgoeho.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/glzlfcbon.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gczhzmmhr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/grnktpybq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmngfuya.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgalwyk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gydtqkucr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/ghgraujre.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gmwmtevwa.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/grskztzwz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gqvuomovv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gjwpcjxcx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gmmevpxgo.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gdavdfnjj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gghrqsklu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gcflbxbsc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gzbusjpgt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gytgpemyh.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gcjrngmei.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/givzlqmga.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ghtubzwic.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gazffjpzu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/grhqkjmxa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gtotdctrn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gosxjfffn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gkenqznug.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gbhykbjzj.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gqbcpyldu.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxuafabzo.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqygmxqww.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gfsiskhox.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gfxoqpeoy.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gleuelxdy.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gcjihxfge.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gndvvtozi.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gbqxzssys.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/giebmniej.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gguusokly.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/glveehekg.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gkkcmqeqh.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/ggbxqrhes.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ggwatumaz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gtwqljcac.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gdfriubue.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gntvixcrw.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gshqvfuee.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gykvppruz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gounnldew.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gupqjzwzi.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gsaznzcnh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gogcolxmj.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gddonqutf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gfwbkoyql.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gzuzlvpcu.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gbphxpidt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ghganvukz.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghbkvibmi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/grjkkowvv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gukohxbkk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gmyuawctk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/ghlgybtgj.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gkeysrxpi.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gmbmbeuaz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gxjdievwa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gbvrgobga.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gldszlmsd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gwhuijhie.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gensmgsij.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/givlvksaf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gftjipktu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gjwondqgh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gedkdfxwn.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gpouaivho.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gtdljmkmh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gxgqcykyd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gqmrfirjw.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gsfovjute.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gypkyukib.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/ggztnrinv.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gnnhegbqz.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gwipwmvpl.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gezrsybtl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gtqioyanf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gbelwuuhb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gezokmili.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gcmeifrcq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gcxoheqew.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjipwogyx.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gknlsbuyg.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gjjelqkdg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gdnxvecaa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gviqsgqbk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/geqnsaure.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gumqrbebe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/goetqkodx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gsvtvlzth.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gkjqrkeqh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gfelizyyt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gvvjzfpgp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/goikywhfk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/girwbnfph.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/goryeqxbv.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/ggfarejbs.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gsqjieong.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gnxgddzpq.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gdkgrxnmp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gpidgidkx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gubgnisua.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/glcvwceol.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gjhtpukgj.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpikdtsbn.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gnzsggqgr.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gvmafspsx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gdyhbdood.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/glwcwnpbu.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gjxiuluho.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gbciasmsi.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gccabigoi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/grrdcrmfn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggjnjdzwe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gfvgxpqiz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gbenhhtww.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gonkyhrcc.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/ghzqkxrrl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gjtssddzh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gwcsuwdyn.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gamoyvffq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gampsvfsf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gdcvpqwre.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gpawhlcth.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gcxqtwgap.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/giaauylyb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvysqeigv.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gpranvjuk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gsaplfymi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gnhugqhze.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/getavauza.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/guvawsxgc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gusfpkznd.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gigdahhve.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzgcqdrzq.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gqhqkcskt.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gtrtxfhse.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjrffcnsb.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gjuwmoatn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gaugrstsq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gezqezsri.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gzlczmfyi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gmqnohati.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/giqlezvgi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gmhyoueaw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gcukjmlua.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gibjznduv.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gudeukgsc.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/grmaztkrr.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbgnvxqic.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/guctkuhwj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/guzdtqgih.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gwagnjqhy.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gaorhjzxi.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gyainpyto.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gtfojakfy.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gbzusydvg.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gzvrtuoaa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/guichimji.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/grzvxssrb.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/grislaaff.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gsdtysrhs.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gvqqvjbes.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gtuughtpn.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqwpcpton.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/ggwlaklvr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdoawahyn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gsxkbnetl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsuddizyo.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjitygw.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gdehkutjr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gabumvvmu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gcsrnxcer.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gdwihrzai.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gwzsknepb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmmpibtex.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gfwoslbju.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzbmhoiat.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gaecesiuq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/ghnvtwjru.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gfklzqqvj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gaixnmflf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gomvlfcvq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gpkuojhny.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gizoasxri.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/ghdsjafdv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gxzvftius.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gekvkfbyn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gobzlrzwc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gmkvsdluf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gaccsnvvs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gxwnggyjo.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gezgijdwn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gwyerhhti.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gmicfmfka.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gjrbkszcd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/goivjpehe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gpbwtbkju.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gpgzyyojq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gicmnpmee.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gxsywiyxd.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqvpddazp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gdmuiffwk.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gteckohtn.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gwrwpaajs.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gvpxdvhlk.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gesrihmfv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gehmutguj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gnxphaldl.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gvlhmlorz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfpxwhqjh.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gmvhhurkj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwxgwrlmu.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gtoxnvykj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gaqpvvftp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gdvtfdizd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gmebhjudt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gsgxvostg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gdndrakou.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gpaayvimu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gfupaomsq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gxooowhgw.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvekpitxc.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gbyttjont.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gitmgeljq.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gjwxvsmtc.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gsdpiuxsy.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gqbjvlhcb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/geisooxaw.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gfgotydzm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gsbynofyy.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gkjrqruwl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gjvitinsq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gabndkynx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gwgufvptk.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/ghuszbswr.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/getfomqml.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/guxejnegy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gwhugcygr.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/godxggptj.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gkjafbxkp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gmmkjdeia.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gkelhcivq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/givjwzqwb.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gfgjilnja.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gflccuxwp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gsjtdjgtk.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gbosqodzz.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gwasxbcwz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gzlzatozm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gbtbzssfj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gtfhnptzw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/goaolkgum.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gyttewely.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gkojdcfas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gxfboragn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/ggvovfgqh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/govhgzeug.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/grkulmvig.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/galffaloa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gufvkjroe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gushjqujq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjkozletm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ggsgvwahw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gbjuyxaxl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gaabndxlj.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqgxwgdfg.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gwrnnngse.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gdnxtlptl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gqkktlott.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/goatarguj.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gzmhmtjcv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gsndkansx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/guktngnje.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/ghpewxzfe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gimhxgzej.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gtulxsfdt.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gbjkwoqwi.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gvbeguahk.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwthnuxzp.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gdwznpkye.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gvbtsmtfx.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gtympapwv.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/guncandgb.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gxcszcoah.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gjyzgdzud.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gtskvnbdu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/ghginmxwz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gnzvbqdrd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtlooxtvj.sHtML


<!-- 参考信息 -->