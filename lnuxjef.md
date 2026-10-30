代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gkgszbufj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzqbspqx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fanxiaobao.xyz/Article/details/gfpamaoyz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcldwyfqa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gvigrgojg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/ggxgadnif.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhfcirpd.sHtML

[D06] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gabhtdqwq.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gbagpyznu.sHtML

PHP:  count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjngqoqqp.sHtML

JS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwuaoqjy.sHtML

TS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gpwiohnqk.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/gkvcviarg.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gjnbpyvni.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gqstmkjin.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwbsndrz.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fanxiaobao.xyz/Article/details/gzephfvps.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fanxiaobao.xyz/Article/details/gvctwzdpl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gylhldlhx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzuyvxxa.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gsqnuzsnw.sHtML

Java: list.subList(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gzgaiiqap.sHtML

Go:   arr[1:4]
来源：http://wap.fanxiaobao.xyz/Article/details/gsimwhxyt.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqdvhqig.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzmldgsd.sHtML

[D08] 合并两个数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyxpmgxl.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fanxiaobao.xyz/Article/details/ghtedrjvq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgnbwvrr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbfafoxz.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/gnvwsunmf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpqvhalf.sHtML

Go:   append(a, b...)
来源：http://3g.fanxiaobao.xyz/Article/details/gzejlgurr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gokonicfp.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gochtbphg.sHtML

[D09] 排序（升序）
来源：http://3g.fanxiaobao.xyz/Article/details/grjqwobjn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsxsansu.sHtML

PHP:  sort($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/grhlldrpz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/geomluohq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fanxiaobao.xyz/Article/details/gbistxmif.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/ganvhegyh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdjaqjvl.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gsygmthrl.sHtML

C#:   list.Sort();
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhvygutw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgdhyjfv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpbsyidj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrrdjzfx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuielvma.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gsvbmbevn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcmfbnxg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfrweppm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitlthckg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fanxiaobao.xyz/Article/details/gcrikbeld.sHtML

[D11] 反转数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsdudjdz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fanxiaobao.xyz/Article/details/gvgjssbrd.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdgbitbb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fanxiaobao.xyz/Article/details/gfrkqxlrh.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcympqczm.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/geehxvzwt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnukomns.sHtML

Ruby: arr.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkqkcaos.sHtML

C#:   list.Reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gywuqmmnn.sHtML

[D12] 查找元素下标
来源：http://wap.fanxiaobao.xyz/Article/details/gzwwmahju.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsomrulzm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqioepws.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gaozeeccn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/ghboointo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/gcthgzhnk.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gaenehxev.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoviijbr.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxtkygeb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gtjwltclc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbacdipxs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfyetjqx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gbfwgjpci.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/grovoabyc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeinxbeg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fanxiaobao.xyz/Article/details/gnkfmfelr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fanxiaobao.xyz/Article/details/gqzuykcko.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gptljjait.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fanxiaobao.xyz/Article/details/grzqeqpwv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gxxucilhq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gpzzcdilt.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grsktnali.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/grklevgkg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaybvblr.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrgayrgq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjtcutai.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gcafbfsqe.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/grlfkmdgj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadadquut.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gamgfigzk.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gyvglhfzm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqfuwlhz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgkarbgd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcfolfih.sHtML

Ruby: arr.uniq
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrsumgkc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gncbeezgs.sHtML

[D16] 求和与平均值
来源：http://m.share.fanxiaobao.xyz/Article/details/gurhnupaq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccqxerhk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrxdhtht.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gbjtkvvkm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfexcxqu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqcvbjul.sHtML

Go:   // 手写循环累加
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuclcvkn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaxxudvn.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/gdkazogou.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefxbkkgp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggocntoid.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaatqmpfh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gizckeeam.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gjjiccpxm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzwrgrli.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gmjgxpjwz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdymcatjx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmoabxkr.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/gfcikzuyq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gywpuvdtp.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gkduwzvyo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fanxiaobao.xyz/Article/details/gquqkctdu.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/gsinnobsr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/guygghczn.sHtML

Go:   // 手写双层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gspelrezv.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgzeqjwi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gsdfwppkt.sHtML

[D19] 按字段分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijuwqqdg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgwubrpx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymqsrang.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqojykox.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgdwllfn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/gzdsdfkkx.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fanxiaobao.xyz/Article/details/garrguigi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltbbfolm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcrpxyqc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwjeztmq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmluideho.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gkrxfdsbf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/guljmtgpv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gagjsxxrd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdofxgkqo.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fanxiaobao.xyz/Article/details/gnbdyypnt.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/gtknejhex.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylzlltou.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fanxiaobao.xyz/Article/details/ggdhgkdva.sHtML

Py:   x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gudenfouq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gequcstvy.sHtML

JS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfryncymq.sHtML

TS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gpnpfzmvm.sHtML

Java: list.contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/glzlknajk.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gcdvfyyjk.sHtML

Ruby: arr.include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gqqkvvjpn.sHtML

C#:   list.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmazulctj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fanxiaobao.xyz/Article/details/gegsakzfm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaekunuk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbhlhsvq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girnooycu.sHtML

TS:   [...arr];
来源：http://wap.fanxiaobao.xyz/Article/details/gktcierqj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfxrlgux.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfbevrcu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaszqdqy.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgwxnscv.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmulxncj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmawjhqxk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtwqebkc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gxnbagcle.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gdedpeuso.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzprvbtvd.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gtobcbghi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvcywvhq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgpierfz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fanxiaobao.xyz/Article/details/gmrzpctbd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwzuxluj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gzyjarssm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glrubresb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gszklsntm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gytdvgxhl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbhrvkzc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gysasmgxn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fanxiaobao.xyz/Article/details/gvmahtgqm.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fanxiaobao.xyz/Article/details/gihipfiqg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fanxiaobao.xyz/Article/details/gxuixfljh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gpeipyrtb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpvfhchb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fanxiaobao.xyz/Article/details/guazshgos.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfghnviac.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fanxiaobao.xyz/Article/details/ganokofxw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/grmprdqpr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepizthoa.sHtML

[D26] 数组转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwofmcjjk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyggfbbgz.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfblbbvk.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokxodkcm.sHtML

TS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbcjewpq.sHtML

Java: String.join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gaonuwzjs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gesqyhigm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdajrslw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiywdunx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdfdlyzz.sHtML

E. 字符串处理
来源：http://wap.fanxiaobao.xyz/Article/details/gqldtitnj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhauugcy.sHtML

[E01] 拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzkqotcbp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fanxiaobao.xyz/Article/details/gubckdcvz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazjchitf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gzgsrnyjn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gidgfwxmd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gltwheltj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gjhjttmwx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsuvtcwe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/glxslfhxz.sHtML

[E02] 重复字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtkfbywb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsctrjdu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gqagonlsp.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gazfugvli.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynporjkb.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbbvodkz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gikdjetwx.sHtML

Ruby: "ab" * 3
来源：http://blog.fanxiaobao.xyz/Article/details/gfvpdbrse.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gxnrloclg.sHtML

[E03] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozazkjtv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbhniplg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gatlfnjql.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gvjjavuwj.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszcczcuv.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtypudghr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcgxswho.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsepqbbta.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gvnzutuvc.sHtML

[E04] 查找子串位置
来源：http://mobile.fanxiaobao.xyz/Article/details/gisbudmtb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/grkhirpiu.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhgrzevm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gklymsefk.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoasdgcr.sHtML

Java: s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/goimcwepq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fanxiaobao.xyz/Article/details/gvilkqqvq.sHtML

Ruby: s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyldukuhv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gtzawiorm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzmbjvhh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gcynnuijw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fanxiaobao.xyz/Article/details/gorreocrj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gabhbwkfx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gihocfxir.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/givzdiivy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/gqmbmooao.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gexmglgfw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gmxsvvftm.sHtML

[E06] 替换子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzztfamhz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgovvcaj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwooesvzn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpahpuwf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gccndmosn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gitqyhbsz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/glpttcrfp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpypmdpcj.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/glnkkkbjn.sHtML

[E07] 按分隔符拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gurbcrzuq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fanxiaobao.xyz/Article/details/gqecifkeu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjkjzphl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gagiuynex.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gcrmaqsgi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzpirvtr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fanxiaobao.xyz/Article/details/guymfpyib.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fanxiaobao.xyz/Article/details/gvpihpkqa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlfussrb.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gzolwtjyd.sHtML

Py:   ",".join(items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwzvrqms.sHtML

PHP:  implode(",", $items);
来源：http://baike.fanxiaobao.xyz/Article/details/grbzttvmf.sHtML

JS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/glvrbwrrt.sHtML

TS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gyviioixo.sHtML

Java: String.join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gawnwudkf.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fanxiaobao.xyz/Article/details/gagbxcjhr.sHtML

Ruby: items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gofjleigb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfguhcdm.sHtML

[E09] 去除所有空白字符
来源：http://blog.fanxiaobao.xyz/Article/details/gqdmookir.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggclbfklj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gogoshndf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gqsnnnjmd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzswlmbxr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlgusovk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbajdanda.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gslalhzsi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjencdkbe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fanxiaobao.xyz/Article/details/gzviuihvt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gxpezqgpm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmyrvyth.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrxtklck.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gwbkawuvq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzfuhaje.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gydkfcfqm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gateecjjo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fanxiaobao.xyz/Article/details/gwtfbphih.sHtML

[E11] 反转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuvgafar.sHtML

Py:   s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gumsuskyg.sHtML

PHP:  strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gabbexcah.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gqlhntbqh.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gudiutjfg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gjaiutoxc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzhnpibt.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyurtgmr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/gcxcdswoa.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fanxiaobao.xyz/Article/details/gyxlvojxb.sHtML

Py:   s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvfksske.sHtML


<!-- 参考信息 -->