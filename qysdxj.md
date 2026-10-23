代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qgdxdrms.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tszmgldn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yanmymhd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zbxojkwk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qhdkmhyj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3czjsaklm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3txygykvl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3badlvscy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3uhniqgsk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cjtsyqim.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3szrgppoh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3akhpwivn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bixyngyb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rlayyedy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ejafmbrs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pcedcfld.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tnhlyick.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3pannanno.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ywzopisz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zfdfqumb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3srmyafwl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oxqusmnf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3prkepvwp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3cddmauqe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kmxgdjuy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cnurnklf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3iwuysflq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rdwamvmz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cqjwwzxe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xcliypqr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3oawcbgyq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3srmlhvqp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zbhmhtjo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vcdupult.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ghkejesp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3azijthym.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghmrzcja.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hvfyfcei.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hgmnodxw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3apaidjsg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gldnwcge.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbwiphb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ruzmhtzl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nlgyjaqp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bvipuvuz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3palfelsl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tttcicov.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tnphehbk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aemzhqdi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gutoqexz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3etorfdst.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3taqkqkxl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ncgdbthj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zspsikuu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lerorzgj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fqfcvfha.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3qtoxirfk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vyxhywmt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3sozdhrfi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bycirvnb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cjsygien.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3litxzgto.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3vsrorrgs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yzseljsm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3beyrzwxe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nimxaxhn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3iamhlkpx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vxsztrnc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sssrajkr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fehlxjrc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tlsgblsi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kvazrqpi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3irftwxxy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3eijumffa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lvjgrbkm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bkthszst.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tnaedinn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xavvcucg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vmqqesno.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3couzslyf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3vkezralm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wmhexnid.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ghzlkgfr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dlqqyqjm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ziexzodl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jmcjtjom.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pddhfblj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nrracvcs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zdjvorpi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3mcozdcoi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3umrhqbgs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3amwttowq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cwjwjbaf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wotwewrr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hmsrlquq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ldggrkcz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zqnwuokm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jtfptaui.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fiwetqnc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3synyhhpk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ubgyjmnz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zyaallmk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3thymtawv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yqjaoyib.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qtduzznk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3nhnliogn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dvvawgjh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yvyhslff.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3oucanrnw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uiunpwdm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfydtwt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxdydmph.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zpxldosh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3igrqidlr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cxqufcrv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nzkuovkq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rewocslr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dwrifzov.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xrhqsdfx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gnriegpv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pidimcmy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ayutjmkw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vzhsrmme.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ycgtzlzb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qcjorefp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3eglqcwyf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pkibyygs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vgcjmuuv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3heoauzdq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qrvlnpzw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nxiorueu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zwnejefq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lylgikjc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qkcdhwth.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3pktbptbu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3khifnlqu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dtibmzes.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fexumrsf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mcutkucn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3soywurxn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gucdijpx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3npggwdxj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3eeaqdsdy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zkeggorv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ogzccagg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qwjwzhgs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3nkojjojo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rlaybccb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3xckqyrfb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3latqpyto.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3eiezpxka.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bgafvmcp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hshgfznd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbjlmwdk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3noltunyy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lqaqppwb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pvisjiya.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tnnjdzzu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3amdmvfaq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3inyapwyn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bthfgjmp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jsjvthsy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbdovojs.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rjqmzhjx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qvyoxezd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zraqecnr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3plomavyz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tyvkoayr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kokxvmoq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3aouppsxq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3fgbctdjc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jkmybbwd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vcbbuiig.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gblaopta.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnnhjfih.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3prdspygh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sgffkkkk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ardmclio.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bowxbign.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zrswgflw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bsvnqaql.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hxqzsftg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rlfmguzc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3lcwcwkln.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bbwlavhs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ulglkxyg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dyespduw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zvpvnmjc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3pouimydy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3micggtrb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3onfcdsjc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ijzuckqu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lcxynauv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zypsqtxq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fiqfqftu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3tuvmbgtk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3roohtbva.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3giqbuqbb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3oarkafrd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xjylghiy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dnrvmdud.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rrkrwzkg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bjvfkxlf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xslgefzl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tfiaqkuw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3rxscvmsc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wggxuqvz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3unvfqnix.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3avxouskg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iemnpzue.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ioeytarg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3umhdnkxx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3oemeawbo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3phglpmah.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwqysgvq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kqbekbqq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mvejqibz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jqrgpjwn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qmokbtsx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qahmjwzh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gtxplzio.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gvlxpvwu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gtsexzky.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wmjhmedj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxnujtmk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rcncjqpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3genwatam.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cobgijkl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xvpohdlx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3blinlmfr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3thndmhoq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3snmvkxxo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ranoqlrb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uenkslxj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ptaeyftf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vypxpmfg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxrudkeg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dvcepajw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vrtdsilc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dlextzxf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qijxzibd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdtmcnmr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kcdxbmcr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ywdxytko.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ltrhzkqi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kltbjbvx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3taccwrzf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uqcvyokx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3inkfghek.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mczsaioc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bletwfsu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dwleidmk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yezkqfgw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xgwbdfgz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mzchqrst.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zxzrysei.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dzeupsik.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gehortku.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ytahsmfc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xjdcaaml.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hslbracs.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wqysfnur.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uonnesmw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bpbabcse.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qyysbtyu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3egzenqas.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qxxbmhzq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zvmvvsyi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dcogfvlo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kflcyxas.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pfxzcepp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wawnjnxh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3kejtumyf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvbtkcy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iojhtthm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gtpmqwsi.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3djpqdaxp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gofalpbo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pzcuplck.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jwcpookf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3azpmjowh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3upmjecrr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kzizhuqy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xhpxcipy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wmzlteyf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xfsjoxzn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3catiwdoz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ugnfdnye.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lqitlhxo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3odzkffzh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vxnjzayr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yxtwbvsj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3cjrwbdwl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mrnddyfj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mjaqsipw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kbtcixms.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hezuimyy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vnwkrzrd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3usoahoaq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vqocffcv.html


<!-- 参考信息 -->