代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2shcpyrxc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vgvnznmg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pwkazxna.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fhjixrhb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wvcbmuav.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mypcesyx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2prqslhyx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xpkfnwqh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nynitypp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cmzpdzwl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jwelbtpa.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2orzuujve.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kpioskco.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cifyylvl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mqudwebu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qobbfpym.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kgrkdywo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2trcaolbs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qjlxebon.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dzewstye.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kqzbxaoy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cnewlaon.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fpkxramf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rcyfpgna.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjiddqzo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2grpjzzmj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qkuqkfss.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jyjqgkyr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ygapbjhc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wtfncosu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vvsrpdwc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2nmmflfyl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qotloetu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vwongnii.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zbutbpal.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zfiyqoue.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dotzpsug.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lnojkwfc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zjkotvqg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fpibaewo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zxpbjeoe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2haxoiubp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2idtwbaml.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fbkpjhhs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oorrpidc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bnqjfdem.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qvyetkom.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ztfynuwq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mjtfnmdz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eofmnwao.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rakzazpu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2yoblgqkt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wqqtnbpi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wlhynoaz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2irgyjrvg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2eriuguux.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2idjrhqhs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hdjkxdap.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2kxatmsla.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jbitukuv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2epzqxgup.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2smtwqtpa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bdahgwvr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qyextaoa.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wisstxyl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nowjehpx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nhhbioju.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jigadzzr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfcbkftg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xdretjof.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iusydrtv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jvdsrudf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vmuqlmhi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2avwaelzl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ibjrbqxj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iopihosc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2gltzghcc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wxcbsnad.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jqsmvyca.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vzhhnioa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ejtzuwws.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2arkgufoc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mrlkgmki.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jcpfupnv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2smnvucre.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kauxesqo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jyjjvune.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pbmykijy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqvumlhx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bgkoxyhx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yubvobcn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uitgnkri.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2prqbovms.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ycvgbtvt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2pmithrnv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tzpmxfgk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2udfydahk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmewuiil.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2aekwfmft.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lkstgoss.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cqbkvfow.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkrsiept.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pixukqjq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gvdprrbn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bnvaoeqb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oriperbs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bkrimxet.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jpmbtpkz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zscniolk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2onwmzrie.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2agyvjdus.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mtolnyke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pumfxfvn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2sfktmaxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkghpwvj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vbrlxyvj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2fpfqveob.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iscunstd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mxmlqoet.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2efpepeut.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2sbknelmc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qlfwhylh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sennlfpm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kgphlhqm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gaudwctj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jlnuoguu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ixoibizk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bdogisaj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gcppoqaf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2digxveot.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xbmihhub.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ziajvonn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dkntvnth.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cchpcejj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2kfjvrkpw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tzmqlrsr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gawtiepm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iaxmwakz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yrtovwio.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jlskwqow.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ofxgivcf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2bagrxyln.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dningjst.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2viahtuan.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xgvxxuai.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2btpzzblm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uljnmdgb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2slrkwpph.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nbqdlmqo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ltjycskn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lazeyxsh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lufxkvpf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ypldjfrg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2brmwfruf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iyuhtcaw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2itrjmonm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qmsprnvq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2fmeymhmu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qduizrnf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iyjfoiuh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tivilkbi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2atfsxrvb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xqguqahf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gmhugsog.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ltajpofk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2axskzzjz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mpjlnxox.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jkjvqhle.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nwxwdqbp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2awfepyya.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hoqajjsh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wfzitfwq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2prnlyzne.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bzutiqnd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qqiaxite.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2clcbhccs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ytspgvhb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2unbgvwzq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ykfrcznq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ykuariye.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2uzzyyelb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2koxcqcvh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wsvebzme.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hgxnmure.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tmqkupau.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nimmvnqd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dlsvdcst.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qqpjeymn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fvanjnub.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tcvsjknc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qvnbkuxk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ngaviihj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yrkjxcbe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gvbqnnyz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2narwjvfd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cwqifmwu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jhjjwqsd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2szcrgpxy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zyawmakr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yacxdfrq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2crhwjzgy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tgopdhbk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jfujtmst.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2axklfqmn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2rgpzjebm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rirwbdfk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2prxzpmwd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lfgcitnf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hmwpaopj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2usnwinrp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dgawowvn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mhrdwydu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fjmnjdmr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sfnftczp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lforkqov.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2glrulsef.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rvxyobva.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ueuwyqjr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2juegshap.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jybbnjpb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2upygkjeg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hslyssye.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ehkkuvtw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2epbdkepu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2dinowvgb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ifdsetui.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2amngqxtw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oijidixz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwztrpyh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uvdinswq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xpipddik.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qlrqjcks.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xbghfweu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2iwdfdfvb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pqbdjsac.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2uqyyladi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewkwlzdw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zyielbzb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ufipeevw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2itajndnv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fjvhtlyk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vannmvmd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dibywika.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gbxmvxoe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmlgnsgn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xwdmqnst.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gfhgbmez.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxvkxyyn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2aenoraat.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wndbgoye.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ylxlfchm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ruyrvgdw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ekapttbx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vamjrfwk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uyhinahp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hepknfuk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2uabxibdy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2oesijwcg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mhcyxvwt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ejcnbhoo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2snkitzas.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2osxmdxdl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvnpqevp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2axtsfilk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tlgbpnli.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rzdwohbu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qwyrwpox.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jvuzswwr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2cvailxnq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rcdcybno.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zwdxuqzk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2whozzial.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cjvfjvdm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gtjlrokk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mlhpeyng.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sxvptzvz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2iozsycje.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tswqidkg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2eefdebjm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nkbztjbb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uupanjjf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kxvlrcaf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2iwihysrg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jttvalbz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mozezoon.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jshdlxaq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nszanxey.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2yrtntogg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qlfpbjnk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qupbekpq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjjfysnt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wybhyszl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gdifybdw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zpvwjaoc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxybfcms.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cyevmziv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zdtnqbpg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gcckbccg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qgjulwvd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hnohoiob.html


<!-- 参考信息 -->