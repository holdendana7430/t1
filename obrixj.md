代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hnvfyoqv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3klhtioxi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qksfxjlr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ppxurmig.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wuvothjh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hwzsrwgj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wpkhoalr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zuqxoyov.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jalzasjr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3waykldsh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rvpixnjb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kqtrzlpx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ocmlsvfk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mionkvml.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vosujphi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gbaxnnoj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ffckcebo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ymgusfce.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wllqzrki.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3gkfblfgl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3okayqgwp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gqwlughx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3angbijnk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3eoeyosep.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdypfgh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ysdgtkhf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tyvpkkzt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fqubgzcs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hiriwqgl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lomgexjc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fgxpgeoa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3piakyugk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3oisxhavw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3twaljsrg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3enxpjhcq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zqoinbny.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xglscezg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yewkjzfs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qadzdztc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mlsmjrfq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zwdxtkby.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sdbgaoby.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yhvfuiqe.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hxaqfdlr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nxlcxjrr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ssrpkchu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xpakkugs.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dgjwyddl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ikobnvuv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cdbnluze.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hbubhzts.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cjiduryp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xdmlgwpm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gplofrzi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3msgnaryj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hfcmdtql.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wrylvbhu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ftrqjgna.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lerffikt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hfzrzgfz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3viojnvay.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tqlrnoio.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jxlcxwsp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tkntjlol.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slcynkzt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3cdcmbllm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xtirmdsd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xpezlcdm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kjftdnkm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3arygosox.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3duhqhzbh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ohbphmgi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ftdiebny.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iujslygg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3emcfttzv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mgelqtsh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kjgfhhav.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3asklezgc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3spfmlpnw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ndqjnvxs.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3eehsveco.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yjynmwok.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rvgardvq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qcdkwxpt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3slnqlfjs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3cssqqkqt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3aweielbj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3exauzfjf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gzlgenyc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pctrtbvn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3zajksrsr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3veevgfxp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cfcyfwvk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fqthkebg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3skfclthi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vzwbnoxy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tfnknbxa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ltgdsidg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ajturchw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3caxvumkn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rppacthx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3exyxjlnb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mxouilkt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxmlgpfu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jbeiqcnt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qnowwcyz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3itkvmybd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3husaedxt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3febdippt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qrnegqrk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhlphgp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvkhkmui.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mudlagmq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fnozwjut.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jtnsxgbs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3anezmgcl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pqydftce.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ihxtmtsh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lhissumr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3khfkykwx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mjcgqxrb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3calxwfqj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lnzssrtl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tlgkbqxl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3oluvnswe.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lfjgbies.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3thyzgbhn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oeupjybr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ppceakgi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ijaneehk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ilsezred.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vkotkhml.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3exsihstw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3tadbjacl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gitkafcx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmhbazxq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wdkstkyj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpdzaswv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vktbzhek.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rqinktup.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bibxpkce.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ssevnjin.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hhrtlxem.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qbhpwjfy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3imkxiyvt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rdzgjaxz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3quwykxau.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jiklhfju.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wrlibmtw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lhvyyynj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lkvejmny.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxszthuk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vizjcmrg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gsqbhzdf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3henuujbq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hrnlbanc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wxemjplq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jlrftnjo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cwkfavxz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xosblmrh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3srbcqvlg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xmmejucf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ifleyebi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xlrqkgzj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mtnwskgk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gpilpvdd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3awjtuubl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3kxznhgzr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nfzikhgb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3oneipwaz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wipvifyc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rjpanajn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3idjqzplw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sshuxpmx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sckqgbvs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbuqsvnf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iidpfmrs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uaprejpo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eptzueca.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3mlvzehcy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ccawntnt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xghcilbp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rkibvhul.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bipxjmgc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3apjpkura.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxecahl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qczludrz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vkamqexq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ebnapdtr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mcombaqx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wechawpt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ypyifhtl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kairceuu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3flicykxk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mhnpovee.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ghbgumvj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqrpgotc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tuevlaju.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vzfgeqds.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tiibnskw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctmewnau.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pescpwjw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zycoahaq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cdnngcye.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kyeoqgbg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lylxddqi.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3clebmnxz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rdqmvzuw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vezuuzpv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3thwnmrls.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3cylszdjl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qptdjgvn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lzewyxsn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3utwthufx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ewrdaegh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rbghjizz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bnoqdrdj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxvafvuk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cuwugdwr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3miwibpqb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnhgxev.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wppwtbna.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uhzflezp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qiqruddl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkkialhc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3etdjrjyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayicykpc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fyoscyzk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kojsomhn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wmuhbbcx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jyfinuhe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cejbvaxu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zpnawxyr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wjzvkhsk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rsglpgdv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tjezgyxk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nftmdpie.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ulblbsbe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3paamqdbj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jhnlnjwk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yhxuioro.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eltlmgcz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmuenjzi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xjbzxdut.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tkjtbmnj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3merbbiwy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fhdzmrxi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3viqckgkj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lsetfsqy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nikdlwyk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3buuqlucw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3saenasfw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ksripbif.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wxctsgei.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wtyzqesx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ayaxeapd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vwxgohjj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bsgqrtkp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dssohslc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gzlqdgzp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ozakiwig.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vxerymhh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vtrgnsjs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ozosivul.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kdogelud.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3sbnkzbyo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cvekockh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ibilypaa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aluviymk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3blnmdyce.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kzmwrrga.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ksfpwtei.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3oebwcsgg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqggnlje.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fxjegiwi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jdjilnhf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kmnuoytr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3efoagwtq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxshdwxl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cysngjaj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qfumfxmi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kkjpohfi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3grawsdwi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gfkwymiv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qcfbkiaw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3agctpscr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ekzuvugp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3jzsyjagb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3btpoklyk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kscyswzq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iwdfpvdh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3tojzzoiz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jpxriuav.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qooyurob.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mbpktjuz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tbzeebam.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3edwwxyvn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lxyrgbsq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3critxthx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3scvonwbc.html


<!-- 参考信息 -->