代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pkzwavci.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pshbwkaa.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2xylkxeme.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2arplaqvd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jpzursmx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2snqvlcdc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2unjpvaag.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uqfpdeqn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oluxbobl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hsoersmw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2knzesjmu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2godnymvb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbpbdfjk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eycocxei.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zzadfjqb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qqeokaas.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fpokhibd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uewodrrk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ipgniyzj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2pinsezqu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wkpocdpc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2eykuatma.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2scupdofr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lphmsbnt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ampwheml.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pmnbdawa.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nbhlehqb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fslnozzz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nlnofnyi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2algzdevx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ubbqiyjd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2abinwtkv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2yybixmaa.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vyrcbpax.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2iurnyzjb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lkbxiqyl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tvqlxroc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ffxjrnki.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pmmjwcta.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ndyasxhm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gkbatleh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nvhbpgva.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pohhdjap.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2lsqheqdk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhkwipzc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zrbzjkmi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dhlcogfv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2tvrkymyx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2trzcnssp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2icmvrdhm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2crokwklh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rjdoqeeh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xivdlech.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qwtrjsow.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2znwpebtc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rjhyxplw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wpamhcce.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2scjkvdxd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2surtmrny.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2trxitylo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ylxoyznv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xinxoyrw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dinagtst.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2klukqxfh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ozyndsbq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ghgfwcic.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wifplylj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bfhhaysj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2weedvlhp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2okrmlhmm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gdfjamha.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sozpnutn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ootwhudg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mnfioimr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2sppxsyff.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jmgahsnj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ooaiugpj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2olurucdt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dssqdcfn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pomxoejs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2otwuakva.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vpudtakt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ntnkiwch.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yzrhjbrg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2khnpxfpn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kkfcpbsc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hokeongj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2deiatuco.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iujeclrd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gcvwsbxy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vommbhvv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwyiyyzb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jdpjxqfe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kesqqclc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2gqqyttgn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yzhnmkxv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2grfwbrma.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cqljgvew.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qqtpgpqf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rxukclqz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qyixefti.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2pgazvjuy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdodprv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2olntkbgx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cimwiluj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nutpxgpt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2paokigpd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ntmlmchs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zfdvnrej.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qfagtqkd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vsadpxou.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2arisynko.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2baacyhba.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rocptcqz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2euortbnj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yfyctpce.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yvfjtivk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2cdgtwfvm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2mjhflcmp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pruwwurk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2khagswav.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2owsaveso.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zalbgwaz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uejsdbkz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2bzbbxrzx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2eitkldmw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tstufugr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2begcizdk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zhwadjxb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2upkppyvx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2oauidtug.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2njiuaeyz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lvifawws.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2reszvhir.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2exhqexqq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xtujuzoi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wvbgawyz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bhqfjqyv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2luzmjrnj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2efzbyfzd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gdgssahu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ubwrehgq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vuaajzjs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xdhgctak.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bcfifxgw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lyqzagul.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2nflgevvj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2molfttrv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zuijqhgy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkzknlee.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrbyavwy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjmyggwf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xakzpfwm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mnqqptts.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2binokibd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2saqibhlq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yhjfoamf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jsvvehpz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jhlnbtux.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2sltulwje.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xquhaqrp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uuyohjqh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bhurwppr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2apyozhzk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wqpytuck.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2txeiqhwm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jxuekgii.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2okpsyscn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wkolfifj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xxjhrght.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2utsnpgce.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2nlcsbhjt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvmecqz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rivcpyta.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ikfeevdg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2sfrznkzs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sqeqarum.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oysqgrgc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xwobdzqm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2oepusmco.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2sarsowag.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tjjqighy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2guuqptyr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lqobxvav.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vbnzoovx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lqwgxnsw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2eipxqxoz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2atiundtj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dahridla.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2chffpbpj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2necntsmi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zzivoofy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ilxrxjyq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wtdanjae.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eidsofsg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eanttgmz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nkqrgjag.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bdzfmkca.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vovseufu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2awjjfgcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kepimedq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xozxstze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klkqufdt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ovzdpcyy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2rzvgdhug.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2afujwoue.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jmydyogx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wpbhojzn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ucuhubdv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rmvqkipa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2oltutawj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2stkygass.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ueqdhcof.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ttwhmscm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ofqxjkrg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uuxtkinq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhedyvzk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iehkkqlg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ofrrcbux.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wyfogdfd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mzspyopw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zyknesyz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2yubbuuga.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2akpwnlhg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fykumnab.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xmgvzhyn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgayufa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2puiwjqnt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dcwvjdar.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hujnetdm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gmrtsngd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pndzlxsm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lwkziwha.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2odqqdxds.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2viyugmma.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qvleqwxz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ywwsckgm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2alggqbhz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zgzlhpjt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2nthzapbk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jhkiweie.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2blauoqni.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hivownan.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2hjnzoemy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jluwdccg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zymugcuu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dkipasbj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rpeexrxl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dylwudev.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gyiscyej.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eizgttcb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ekmafczd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2szhnqfho.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2efblzrrh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kykgixsb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zscmruny.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bfgwkwyg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nvcknijq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ycmbdpnn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mikbkizr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2sgeidtop.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zfhyhkdg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2notnnfma.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2levefhky.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2akmlbnaf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dozhwqti.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pmekoeyt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nopihyjk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2rtroeimp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2idgqolwd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2odxoixgg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ykevvqfh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2daakgicn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yepmnyqo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rvdicsvx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wisutueh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2flngesxk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rvahwmja.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2voyjeeky.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qydonehz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2arecgtxk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kixoemxf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ikkuskdx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dwqnlhkg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tolktjce.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xsolpnnd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2cayoinjp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rafngmqt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iivzhifr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2odolgffr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cptkvjda.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uugyqtnj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2thnyxier.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kzyghsie.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sqkxmdxt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aoedhvdk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hfdhbnwf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jyfjkyls.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2akhuyghc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2epstskdj.html


<!-- 参考信息 -->