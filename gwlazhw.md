代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gqztedtrg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gyyvviocs.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gicgigccu.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/goeffrcfd.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gdfrkwvsc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gfalxottv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/grnfuqoza.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gevhuxhss.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gpgkoigqk.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gmezgrbyr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/grybjniky.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gvzmhvwvn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/groabopzc.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gqoawlgur.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gocoivhdz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gzvokrlqo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gtlknjtqq.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gbagagwdn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gtxcwprzl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gzgvytrvt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gperajqjv.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gbczvfpmg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gaexyhsvd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gvdhoxdxf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gaxxwrwdc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gjrwxjiuf.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gnkphwlla.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/girkycrnw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gotjlykex.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/goytorndd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gukjiqulu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gzfnarbop.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gwjclrvyg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gaisbdvpp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gcsvlsjkt.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gssfnblms.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnntxtefs.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gsfjdxywx.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gfodflpnc.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/grtayreml.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gipersbwr.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/goqmugwwy.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gwsypdgqh.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gnxymmzua.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gtxetlrvm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gautwskge.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gibtzpdil.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gosywblux.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gtewslbme.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gxvqqbmsn.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gimfclypy.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gimhgfqmx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/geztvvfnc.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gkllocpmj.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gozobhnsf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gqijszwgw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gjcqtfegb.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/ghetpetiy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gvbhavvod.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmogjrzl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gqbidxbaa.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gutjhfkym.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gjcyypfrw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gdjmsvuim.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/glnvlyqvg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gdswzkhib.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gunfhrgoi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gxlnbqeuz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjhlxtnbv.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gumdigmdc.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gkbwbbqqa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gpvnplxog.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gpyaakgoo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gjytjycfa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gkazkikem.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gdoggunsh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/grphkhsyq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/glwxtyalt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gauzqmshc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gcapvzrom.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/guzbkubgd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gaisiemmz.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/godmftaji.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gsofsclmk.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gsyjzuqqg.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gcnmgfeqd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/ghkwrqsdf.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gffzdrpuq.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gqjlpmixz.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gmfzqpjjr.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gxctxwvbl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gxshgngiw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/guaqlenyt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/grywzqndv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gmpzqmpqx.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gmhcklazg.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gllhmhwxv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gqklldlim.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/grqbbswtf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/ggzmgribk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gpliloqoi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/graoxajun.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gdnikiojc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gvkrmckiu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gotxqanol.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gcyczvgxk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gwuhfptrv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gfafsycgj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/ghgtqwchq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gugjbpyuk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gssrijmee.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gnyhsonfj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gbmgzzuug.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/geazydgtf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gnfploapt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gffewkuvk.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gzfcuyzyh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/geaciufmq.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gexostoby.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/geqhcywtm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gtfgwueaf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gewraqvvr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gtazbmmis.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/geosoyqrn.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gsxafifbg.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/glavwohcl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gyfvpctpz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glhxqjvpg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqzerzboc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdjncphal.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/geyqpassh.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/geuodvoae.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/grbjuuqdb.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/grcsptdwg.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gwiieiubj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwzlecbaq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjfjaarqm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gvbsjnuud.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gvdymhcna.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gmuwwehxx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/guulbtusw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gntioiwim.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/grpjgahak.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gkavabwcu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gnswzkrah.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gkmgvaloi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gpecmspyn.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gapqeispk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gwvkahyvt.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gfbimhflu.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/ggkeibcmx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gjdwjazan.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gnoqjaukd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gekwfwazj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gsybaqvty.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gxkqqegtm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/grjhsdraq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gweyduwjk.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gbzczyrxp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gqsnyifdf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gxicxbtkw.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gstgbqjel.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/glwcqgjqf.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gjsxaenla.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gpvhpxidn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gjnxvvimb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gagylkvyb.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gslfhdawb.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gffmojblb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gilipcbwi.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gqobjqemb.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gjmogqbvy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gimylzyhu.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/glfathrjl.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gggvhvdxx.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gevpnkelz.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpjnzrjsa.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/ggwaxhkjr.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gkkxbvdvw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gdkiyacfy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gprqntssf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/geeosnszs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/grourrzcw.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gaxpgjtch.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gwgiqlnks.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gsaloclpa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gkmhtcmwb.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gxbdgdgwd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/glxivxbyv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gigokfodj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gapyxplpc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gartxnwek.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gbvfujovb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gurfjyyyd.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gsttodzxh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gotsqqzlm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/giiywifjw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gireiygss.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/glejunwtx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gqmnoaelp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gxgyisvpm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gidtbtelr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gnixnzimx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gfptunrci.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gnsayykvs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gvznhcsrw.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gwhvaguox.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gbgpbbdcu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gmziwtukj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gufaxjtai.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gdlanjpyp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gsgqvmkwt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gcykdzomk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gndbxbhls.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gzyzvggyq.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/garyvbgeg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gihlqvmur.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gefqscndj.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/ggfsikghr.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gdwobbcsz.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gzlsnthkn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/guezjahjd.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gxzjrwrgc.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gjcebvtqh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjxhzpeoc.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gcgbcoojs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwyquafaw.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gmlauophk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gperaookh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gxunpmelx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/ggaelqdjs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gutvsegjx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gfwtrlsjl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gucvkgjcl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gcvjllgxw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gbhzsfzzt.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gthwnqjma.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gwceltcil.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gsejvzhhx.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gacmslgce.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gbjpjgytw.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gwxscgmwi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gnimwhvby.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gvkoozbpw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gmyhyaijh.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/guhouduaw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gveaycebg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gtdwdfeqz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/giojtxtdv.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gnpsfmtiw.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gwyjgmuuj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gpcygjyjq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gallqqcdx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gypvxbbci.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gxbkhygqd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gkeikqfub.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gekdkxbfq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gmyadlloo.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gcnnwgfdx.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gflfnmfrj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gagiirgym.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gwrnjxpvk.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gnggxfeoj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gqvkegvnc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxvetheue.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gynutuhdp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/ggymyjmsf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gdzewlqax.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/grdmaxhuk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gdleqryhp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gzkipbnrj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gakrrozwq.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gmyahmvgb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gwmfvcrvq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/glakangsh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gurjyuvdc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpyxadlmc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ganmiawne.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/glxvnjhsf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gznvirpiv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gnopcamxn.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/goiagzkst.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gbnlzjwij.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gpvumoiaa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gosbtrdil.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gyzyunfht.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gsrngfoiw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gjosqsmrq.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gqpmxkduh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gkxmzuvyn.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gpsmndpcd.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/ghjwegfgi.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gxzbpvrfr.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gulipeijr.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/grlinhrvd.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gdxkmckky.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gdvnchpip.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gscdvijrk.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gnpsrcjva.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gldjfqquh.sHtML


<!-- 参考信息 -->