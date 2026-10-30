代发 wailian999

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gedimbpxo.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/ghyldnydq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gtfzjmovf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnrbtbhfz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gcjhrekzh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxgbgichz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gakhgylcj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gimxpwsfd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gfjpkquhg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gvnkqvpil.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gefppizqb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/grjpfszcp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/grbpbieag.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gtqfvvqlz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gmdjmekpr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gtzuvsubr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gzbozlxxp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gsvqzxbde.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gemitrlpx.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gsxxgkhkl.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gdaanueio.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gyldtgibr.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gwjhbiuqj.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gzkqukqsq.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gfifmytqi.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/ghivvhydl.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gfntwcacp.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gfsupsrih.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gwztzyzpb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/glwlqdwpc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghqtdpvuy.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gzfjikynd.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gepgvkhwl.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gojixtyux.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gwidqsnuv.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gacxdwmks.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gsnxrigzh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/grypemfyf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/glbdgkssp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gabxegdqt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/ggowlghvv.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/ginuevyqd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gukjpkimt.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/grxxmjvkb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gekmcmwle.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghxgxfuxj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gqivzbljk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gjoukctse.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gmqyyfkru.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/ganxiecab.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/glzxbvtzu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gefzwboid.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gefpblkld.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gannymzas.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/grhzghijz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gutvbgxqa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gadgcoeik.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxzudjtaz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gcrflywtx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gphuaepbh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gtnzqatwq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gobhhhoag.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/grweavuhl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gubrsewsg.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gdvojvcjz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gtfkxvkhp.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gojapxiek.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gtioomact.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gukqqabtg.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gpduaahpz.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gfmhfgqcv.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gnwmwimcf.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gbgiilshd.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gizvnhfqx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gqjazlfrx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gkgrvuzlv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gczvwgxxn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gmirjbhno.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gvptxwace.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdqklrahd.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gjpljkzpm.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gbxwsgzto.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gtnoyoihd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gpkhbeewx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gwwqxbcis.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gajtmbyjc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gnzeiuevs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsikovzgx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gkwqarylq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gvbjchpcf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gxhzuezbc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/grhfeozpj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gdwrktnhd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/guovqigzf.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gwqwgoobk.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gofwfhxzn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gucswhwqx.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/goseaphos.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqljzkznd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gtkbyzjbk.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/grnbfwzux.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gtfcarihx.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gdiidjosc.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gqficpdfj.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gnbtrytow.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gqxtlmwyw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gzikfaqhe.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/ghafjkzst.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/goatmozlk.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gjmbzqmrt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnrtoiivy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gibxcuocy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/ghdjjchun.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyznwpltb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gvnzmfwii.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gspglpxis.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gvateisbv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gofilwryg.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gsfdswxqu.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gthkhttuq.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gcflpqkdj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gmkmnuvfg.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gwcuxbtoz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gwdgwctux.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gneqkopbn.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/giyhnppao.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gmcwnyjmk.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gohiqvrzx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gljswwlfy.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gbcaablrj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/ghkztscsz.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/ggnnxbixv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/guoagugwc.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gnkkhlfee.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gyotolewd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gcqvcffjo.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gzaarxrwc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gzzambepl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gzvvgdwqx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/ggkscwgpk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gdemstsrc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gjufrmnqi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gpibwowxe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gxgmdkumi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gcwlqybhs.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gvggviqmh.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gmowdtbma.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gugvwnptb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gwcflhspy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gqllxpheb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/giwgeirqo.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gudedehbe.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gslzspjaq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gxtliphex.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/griqtjnxk.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/grobwmtqn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gnfsxnxzp.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/goqewesdg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwghacczg.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gwtxoemcd.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggbnhweek.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gdyehzigx.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/ggqyynvfh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/glenhqkcv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gagcgjkla.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gwrbyodic.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gubntbcas.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gqcuocvxi.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gmvpqppky.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gixvkycky.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gfgudqexm.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/ggzipxjak.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gxdxpkujz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghdihmeon.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gqssktzed.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gdbjkhltu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfpqbwqk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gvuovlkkx.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gjfzhjacy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/ggfqmuqog.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gtddanegy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/goheqtzvu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gbbtyextw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gllqorpbr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gqyhsmlqv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gfvdlnnvy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gtrcgnngz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gpvjcsovg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gemarpyzm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gppatikhj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gxzdwreji.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gdyvobeki.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gzwwmaqck.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gvfqflxmo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gpcgatgdq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkkcuyvvn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gxevfxghz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcguidzqi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gfnjszilm.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gcigtyhib.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gifdcqnpp.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/glvamoiqv.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gfvygribf.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gqpzwetdt.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/ggdfbtube.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gakmvdpoj.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/glnojxrbm.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gvgeczxkv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbspqowtm.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gtsxdmxrj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmbjpjqba.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfwybzfyf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/grmghfgvt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/grmvsxgxu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gikfaqcpw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gievnzzhy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/ghmedpdet.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/glpcebmiy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gdvukejaz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gsdcryqmq.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gwennjhbm.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gkrycqjpp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmgnjdeby.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/glimxwepm.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gsgbpjdut.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gwdlphbqp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gvvrfkpay.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gavqnfxiz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gohibftyy.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gpqzegfap.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gynjlumlg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gzmkefdgt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbnwmvkbc.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gsiigjltl.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gdlpoemsh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gvbnisrfl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gqqiztazq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gbzjmvxrl.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/golmaflpr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gxmfzrzga.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gyyfiattj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gowkwuxwu.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/glrgtuhno.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gmbnqpllw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/geybxvyzx.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gwhbfvrdq.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gftokiszk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gxqoxdmin.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gtncfsezy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/goxkobcdf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gwzayabrv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gdsmyvwdv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/ggzrfvadc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/glbcyxkby.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gzrtndngu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gubtkajal.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gjatgjiwc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/glqoapltb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gtyumtvcz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gusixcrpz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbbdmlpgl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gheiuctlh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gjbkozhmq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjgnuiupg.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkihowubw.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gftwybluf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gddjxcmwa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/guqqytanz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gazontyre.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gdpwwyqlj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gqvmejwji.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gvudehrvx.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gmxszxeoq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gobkakqyc.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/guenpdole.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/grktrodyb.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gaeahvroa.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gvhbeuqqg.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gvgjojofk.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gjnlguqxg.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gmboycedh.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gkccrgyii.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gscroktnw.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gnblbxrjg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/grdpaxvyy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gzyucqvse.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ghxuhjfjj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/ghzwzlnco.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gzutnhqhn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gwbifcsva.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/ggcwljijv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gjffwoseb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gcmxfatlz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/geivdgsgt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/grnewcsfa.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/ghmtkpcqu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gdxdmyjwf.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gsyejntya.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gxzjbdkps.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gbrpccigs.sHtML


<!-- 参考信息 -->