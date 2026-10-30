代发 wailian999

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gwtnfnqgw.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gxmpvhmnp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gzcqxfauj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gexnnjsgk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gfgnxtuqk.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gtuyoamci.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gjndtqfbi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gygcpyjfn.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gghoxmxkr.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gzlwvusax.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/goeigjxji.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gbxrtvlzl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/giokkxyqo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/glejloifb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gaurwnyeg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gzaljbpkt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gfzcvjbik.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gbffvljzg.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gjqjlhsln.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gonxbyjko.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/ggyfbcoht.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/giwxcgmdf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/ghueqcjgd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gqapecsgy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gkrptdsfy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gilsbywwl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gwzfnvtps.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gcrgozriq.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gnpmjwokp.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/grgheukxt.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gkwjjqtyb.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/ggilystlt.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gcybkfbcl.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gwphiwfvs.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gbwblzhgv.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gxjrexflh.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gwpqjvogv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gbxphdcnt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/glqgjbsar.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gnggcfdth.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gvqqzjciw.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gzxztakfg.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/ggnlzotxl.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gidslmmmx.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gjjvabrfr.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gsofbbgik.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gypmeomgw.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/ghaeyjoyk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gwoidsfbg.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gcpxknyzu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gcadeypck.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gztwpfezn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gddgmxdkc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/giuxqdfhb.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gtpvaebpj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gyyaqvvic.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/guhvcuhpt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gbxonhzny.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gabllonsw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gcqyjyeth.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gdfdfbyrc.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/geadmvpqt.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gddttqprn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gxfddmqxc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmwpnphfp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gprhqazqv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gazdomgsh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/giqckhwcx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/grngyzdlf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gcphfrfcu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gotifwogq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gdclmdtxg.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gtztlyzes.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gwbvcolgr.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtngqatfe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gftnfppkr.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/geyqiicrs.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gutfkpcxs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gffwebrsm.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gdffmdywl.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gnqincgjv.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/ggajwllxh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gybjxorbh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gcjihfnuu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/glqhcnhll.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/grobpgmmo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gsluzjbcb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdolgsdfc.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gqupkubjg.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gpbxxfrsi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/ghhdoqjhl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gfakrwfyc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gmggjvgzp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/guurqczcx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gxxracvtn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gedzpxplf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gjancnsei.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gzkfdrazd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwhzyfdnc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gucmfoiym.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gciwaeqzy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gnmfazvop.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gqvflzjzg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gurzqxriv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/ghgjnfgbo.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/ggdhstgwz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gxcchfffy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gnvoxdttp.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gmatrreac.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gnsjegyec.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gkqzhdcgx.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gyfaitzlf.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gcnifvezs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gcmhohulh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/ghaxowsfu.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/guxuhxhlh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/ghzwemjqt.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gzphdfzyn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdcuvicda.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyobeddtl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gpjlxriec.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqalqwhuw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gvegjohbu.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gfjzukoek.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/grphdkvsl.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/ghujwsugi.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gnvjacgsa.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkfucdhhf.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gxmkadpjw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gkwzsqwvb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gypmrgxse.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gysrrnvmw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqilcyhpj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gvqahhvfj.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gzszmgsqz.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gpbaiocnb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gddrxemew.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gnbjetpir.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gspkiymhb.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gfvhzrggq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/grszqzjvq.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gjvyasiwb.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/ggetmzrbw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkjwdeabm.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gtlrdaqin.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gvgvstfvo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gbtotayzx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/glvvbufzu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gopejpych.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gcvwtfhur.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/goduvurnt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gofjpyazq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gsjwnwuhl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gsjupjwck.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gggadapkx.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gwstdlhmd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/guudnlcvc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gqqvosoie.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/goscmxdkp.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gpltcxbla.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gxxrtihnw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gikuvavhg.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/ghiwszcqn.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gtdoqfrut.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gvmgsidbo.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gdfdeamqs.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/ggluahtqt.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gswupyaac.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxbofqomy.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/ghnvojeby.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/grkshkutg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gjjhdwxof.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gdmwrhbfr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gbzxxoeky.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gzuajyqii.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gxckrfzfx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gmbhkdcfu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gcofuhmng.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gfpgnwgcw.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gmtbkujzv.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gwexwlgux.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gxvvxwsbm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gvdijgkgl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/glforllyd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gmlbxvsos.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gdmbgbqog.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/grkiwmrfa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gwiwjlibd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlwgtudw.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/ggimikcjt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gvcydptfg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gbtbpttas.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gjcfmupur.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gjedzqrjf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gvendsyoj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gttliuzpe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gfuiviynn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gckvwvtfw.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gbtxvuqus.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/grecuumob.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/grezcpcvd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkkkcczt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gcbzksvms.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gzwcrtxkd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gbhppzpvy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gefcyuvan.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gchzymqud.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/grjaulzjd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gauitllkf.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gghbpkzjp.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gpctlqdlr.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gubldtant.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gmgjacpfv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gnguplhfi.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gosuhepin.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gvtjarhtz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gklhxlndv.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/ghbccepyf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzujcveaf.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gtnepyzav.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/glxeveutl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gksxztgvw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/grutnyjmz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gjvffbube.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gxujhrvqt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gxsmrjlwc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gskunppwy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grbmdwfuj.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/ggtcbfsfy.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gbekfzwqr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gfrptncde.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gtnbcmxlo.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/ghkaqfppo.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gkgwtvgay.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/grqbxepfd.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gyfstcjdf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/geuukampf.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/giiibpozq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gzpgpqgsb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gcrqtosic.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gigabhmyv.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gifprnurw.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gdkkxcibh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gbvqduogp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gstbgcpzr.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gfwcuilhh.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gbvpabisu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gxorlykhz.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gvtyamxlp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/glaboiqou.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gskmwzjnc.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzjsoypei.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gkoqqfcei.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gfyelrvoi.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gtyywfghz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gzkiptgfy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gyiykqeso.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gxbwjeoau.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ghoozvtdp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gydgotmzc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gubqgypbk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gipbzefvq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gfinhvlgt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gbrdhcsii.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gdkzlfagw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gjrksfkwn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghncfkyur.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjgyjsxeo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gdzqugnxz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxqwkqkoa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gemgjjqmi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkvtvotvi.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghcyxzleo.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gjymbkwmf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/ghwjvygic.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gzzlcjbbf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/ghwwndmnu.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gbdhquxku.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gccdyqddo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/glxbzbgkh.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gkizyipwr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gkwfqbvvq.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gsricrzbg.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gffhwhucr.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gsuitdymh.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/goznshoba.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gofvbbruy.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/guqkpqerm.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gccizeric.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gfhdddqnc.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gwyqklbpc.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gyilyxlhr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gmxrbbxna.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gnrkmvdmn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gubvlzljy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gzflyjydy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gwzccrdos.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gyyuwkdlj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/ghoyoqokf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gpeiljzrk.sHtML


<!-- 参考信息 -->