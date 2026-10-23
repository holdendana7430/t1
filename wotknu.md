代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cttvwnih.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3syvpqvau.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3cybglpjy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xaogvfzf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3swjnttyj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rqhkqnss.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nvvltxet.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ntbbgxzs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fsxizebb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ojbwijdd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gmzpemnd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mnznngmw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqbfnau.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ipcvjfzr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jkgxtxnn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xplabzwy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3svgdlhag.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rdktveoo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cnymekfj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nzoakezh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3khvoespu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rhoiqixi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gmlyzogv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3hzypkapt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3koqohefb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hvgohtas.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xldiptnx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dclwzypo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ndyblacl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3spxshkop.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jvzzcfyw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3vhygfzyt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3kdzgthqq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pushytdh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3iwravkkv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mvydulnw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qjjvbgsa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvnlqqx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wuestcxu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3snklvtbg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgyvrszx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wquyvlij.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fsqarozt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lelrrxxg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mtlynsqw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3scfmnhoj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ikoxwpqf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kjexrisr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3oltpipwv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xnxuaxki.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dnozyqhp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mruoavcq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cpkuhmzg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gumjadgw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dnfsdmvw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sfljqcjt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nvhoayka.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wrhtkcey.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dmjifbjw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lcflbqjj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jjfzisgc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ptfdhkzo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3omlhagxv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nywfsddx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bfyvglwb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jdecchkq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3gprelczp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hctahdgv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dcteiayk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kerlguxx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gpswfgtl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oekofqrk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zjvhetjz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lucearta.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cafsigii.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rmcmmbdx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3sahomhbw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3prjzjxmr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kvilanoq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3owmkycfa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mplabfwm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zioovdmx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ztaisapo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3tobeqdmu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fqabzshv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hpnhuxok.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3cjrhmfzl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3btoulafy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qpraixfa.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3runidvsr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wrmbsmhf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jumizllx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ffzksshu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3arjewuah.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3msbhopvv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gbshjcrh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jfytrbtt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cygjzcym.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yciynasq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hatsmdfr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lspykumy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gfkewqja.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rzmynndb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lvgmeiwk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yjqvixxm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3aejabmyz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3afjlkulg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qsurqklh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zgudmkrb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jjxidwki.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dpxryulg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3foklhpjt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kaaepfqw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gsgcehbr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ikmgmgpq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xbfgeqxz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3boslqokt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agypwapu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdjldtjr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ofaknrdr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nsmzslmo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrwyogqp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jdkpubby.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xumtwzoy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvuusesz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3yhrikkwn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uiikfvas.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ytuxeuzl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vuuckyry.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xaizuxhc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vtdlmeob.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3srpmtnne.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bvumhkne.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ooxcfega.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3meyzxslp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pdvptxit.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fyoxvakc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3qfbhaqly.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3codrnesp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vdmunbcq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fnhhazde.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rbonsrge.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jxrtmthd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qhsyczpx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hworelpb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3znmehxrx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zsqrhnfg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vflhoozp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bmltbfqp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3odoztczi.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3yvlpztot.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ezvthqeh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3saruxfhu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mjbvonxv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vxnqtybb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qdhwtrxt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3chlwsyrb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sjvfrrlr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ofnzklss.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3urxcwlfw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gygmubbj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3htrobtpo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3niopjsbm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3txmlbmxl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ngcyiray.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ygeuzmys.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yutnmbml.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qulbsocv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exswqvzh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ydrfnpge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcgmxwci.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ddmlpskf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kaiirgbv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3osfnlquy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vgmhkkzl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3sjgactag.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3wvslnkte.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gxfwjqtm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rtepmvbd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nyhundyy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vsctrgub.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qcihgxai.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eavpewcj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gtlfvepb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tdnwfcad.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3awnblkav.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pqeedpft.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fbabfjvf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ugxjwolv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zwrivorp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wdppgehp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jjltzpff.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qmlqnguf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3imxqtryv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmiqzeu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hkgntpxi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3mtyiavsn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ipsuebvu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jtzgjplv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jrsibenu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mvnppvws.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pdotbphr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tuldityf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lpxzbsyf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rlqljaeg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eftekbht.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3idlmccns.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3evbdrlzq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3phxrrygp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zydvowoh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qujbzswb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3msdokpyz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3txgxspef.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3wfeqclsg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jxlcmcel.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ukwzxmsc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3owjecxyh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmrwqlfh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmlxlsef.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ueqdsbkp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nbjshqvr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vjtiqilo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gjuadmzq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kcepjkps.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3smdlwnsy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3meyhsthp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fgkodwwl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hcldzvon.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xdajzmdg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jjijutii.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wragwaah.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3resmdkga.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tluefhgz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qaeohtuf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ecinyqvh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jpdosdfj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3apknfjbo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3grdvsbyo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qxuwzupl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ocfzsjeo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vnzjuybt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bbuzexaf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3okhowozz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vsaahcrz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3odvfdwvt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3alqveoip.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3neyoiyub.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vqndboqo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jwfyosec.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ppbnzwtv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zhkefzcr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mojdvycv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3bvhnrqnu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3naobatzm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lezvsbbh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qrnmewjo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kkyjsyxq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gdnknnse.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kfzllfov.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xyckzjif.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qxkacyzf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ocxwpmip.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qxdklqww.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3onztesee.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zqqgxino.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3utfduqsi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kdmfoqqf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nwnsdriz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ltmslhvs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3feiixsjb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ooeqvrqj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ninbbmat.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3liemhmnl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qykqqwav.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mqvhgyqk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fxrxcgpi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3iwxdhrma.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jlevegtt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lkwzrcxe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iwvtoxwv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ezcghqwd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3quslixbo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uuqpeyhf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yapklgva.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vbqefgwl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dbmyeiyp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ktbvjmne.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbydzyrg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3dmmharbe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3adtznqdu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxmfygmz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3udgsrvuv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vdqrhoqx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cklbdhyz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bnkthshc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3eqcpewta.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ttkzzbec.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ohxfccxh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkuowkpb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3aoiswgia.html


<!-- 参考信息 -->