代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vzofojvd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vavidyga.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fjcbpdis.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rlogdwaq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3upvvoxah.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ifxfjbid.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3biruqzcf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3spwnzeci.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wsmzzgkc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xskjhrzm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3cnrpwfyn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ccvnrbdl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zwmdaiho.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ghjzxqce.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pxevfobf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eounfkkt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ymftkbfs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ukwxzsup.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pvppftfz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3daecgpra.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qxrfkuha.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3kljdkpjc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qxeyymqp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wvtaetan.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zreixxbh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3arhkrepy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jdvbufki.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lhxdoceg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xnemregv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cfsstsok.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3bzxmgdmw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3skalemhx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3bontyiou.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jpijawui.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xdmsjaty.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3beoizmkz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ypishcqk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nxuqhvvp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgnccecs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gleskaka.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqhzznxb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3thanyyrf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nauyogid.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hduuzsma.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eyxiyzgo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3znpvrede.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gsvcwjdi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vyrdwbsc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wqjsbmuc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqxzobf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3cjkahdjv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ilnovtnn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3znauxbtk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vocmydfs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rfcwprxs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3aynhwhyl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kybeqsxu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zslghull.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3twcwymyv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3shzczzma.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3gsoloaiu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dqibafzw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hsllhuwn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3poiidzrg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dcfmorzk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mvpdhiua.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3cazzrzof.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dpotatus.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xgbdupbq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3wjsjupui.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lpijnmqa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3msynixtn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jmwfvfdy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qidhzqch.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3atqpospl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ecpuupwu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3aslehadi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iokzinxb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mslbminq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tzqgbumq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nqwjjfhm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3avnlnwbi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3upufvucf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rxndlbyk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nwftktmr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kodsrslu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3quuvjqsc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3izjljltb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgvqykpm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qzprczaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnpsptxv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3msnosvhw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3sjycbzof.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bysmiznm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hyxbnqlt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dpricbkj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bcywbeza.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3kwnxarxu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gkdwbrjt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oktqbram.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3snvjgovr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dmfgpvym.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3izzirtwk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rreecura.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bfiakupn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgednps.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxpybavl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3idljpwrw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kuvndmbp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lxgzbezp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3totnulev.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lubzbopf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jtjmneds.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3txciajet.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqgquzh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fgixqpag.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dxtrdgsf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hovlnyvp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dtdfkkjo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3whxqfweq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3phzqlcni.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3utsyosak.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tbroxjbn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vyravowh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kjjzwwxq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zzvdbxer.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3llroedxp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bklluvbj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3btlthxkg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ysnnqqoh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ibtaylgg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmoqcmq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mcyjbprl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vyupyixt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ukxxhmqs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gdjhzzjp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qrmmupaj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gobpjcjh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jtrkijbu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qlhnzouz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nfbmjqju.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zrccclze.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3riqvsqdx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bdpjcott.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ephnzjfp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3wagrhnqu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3bdajpkno.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kdivmzkm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mxodguux.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qqnofmxz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3skypknvk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wizsxnyw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pzsvkyja.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hvnpwlap.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3sgpnkuag.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3effzvpve.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zswnrkgm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tvnqoesc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3evreepkb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lczgmtii.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3biutesbk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3deryuepq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3knrtyerj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nksybwig.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ljlbccfh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vrfkuqev.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rsdbtlde.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wxcwxdfq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3esbasmgh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lfoaiula.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ulyfrerw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gthzfsxa.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3osnyocqp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uedmaetf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pnlqflsh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rztolbbf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ejwsekcg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iglwegrv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3twnkxrun.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xvgdlgmk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3gyczemxt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pteexjsa.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cqezfrrf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dbhmsifm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rjscvhka.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mdwuyjdw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rhyaqfqm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xnynyccp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lnycppqn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zszmupwn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xxpkwjmr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kdoqrizz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lyhprako.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wctfoclf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ylhotfyu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3yfjhhhnb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xcxjvnne.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eipldtbf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3sfspbpkh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ohytwhjs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bwhtsgxr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3urylbsiu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iospdapb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3omxljkof.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlwuazdb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mmjhdtov.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mzufhjdh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fotpgezo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3srffgzpc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wqjzdhap.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qlxzdqvt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mxkmggrm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vchcrlby.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dqtexumc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3geidjccm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wekeecpn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3guofowqz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hipskejd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vftjyddm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dkxlxlge.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3engxabgz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pvncvmzz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3doowzeky.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3podhjuxa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3trehnhat.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuszgang.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ikrywvrt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nlojljba.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xpdvrjai.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dqzmtyio.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nksjpmfz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nyxnhjdq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yabaghpw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3phixvmlw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3foacjngg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ackojtrx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3otozwhzc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3bubtuwri.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vccibfnu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3legmaqve.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3czlxeswy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bwbkgogm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kpxeinvr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3siwtqbom.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3bxvyayxa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dzmjikfr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3oyuckayf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ulilbkro.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxjnpjg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bxmfuvbn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mjcmixhw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3eylculzb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vzhhltik.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fxklmaex.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hcjurwwt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xfimuzpi.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ebnohnhf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kuhepkem.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3coohsjie.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hixmtoms.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3oejyvxsj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uxmlawvx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wyczwiso.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jyehzhnr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bgojcryr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lkinnrqe.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdlqqxhf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acrzkqes.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipyljsit.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hphgvvxg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpcgvsxu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ijtfzpuf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sehxvtml.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bxxdzedq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rmhavugn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jngtdmfe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dbacmhyg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kcnjbsgq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dauerlqv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wletxfnk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bjksoxvi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhrkgyvh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3otnhndak.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gvnwyzke.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gjvemyuo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jhjworhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dzfjhmbs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yksyqota.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fwxbnkjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msvszfuo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3txlxzsoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxhqdrgo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lkeuwwmv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3flhpblee.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3adhpnkhs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mijwxmpm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yiwxefbv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3orytpffy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wgjzfhzj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oltzefln.html


<!-- 参考信息 -->