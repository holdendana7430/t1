代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3beybxuhc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rxivitqm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jrssuknd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3flrxqxah.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zpdnssow.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wqyifoym.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ianconau.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3azvdtuxw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3brppgoiw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uvunqdnl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3owofartk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bkovyknx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hlhuhmuy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yewkryel.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vdpldwia.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yncptokr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xfcrbqfu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kjvftnna.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3prittdpa.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3htiqyozn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mqmffksx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sgqzuwku.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zjdobtoj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3demjkylc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3viucjtfc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lgpylffh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ixnyrmav.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hlpkpbfx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dojvupvm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qhqwrhbk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ndswsrpt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rydvarob.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3knxfcwuk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyfhowbp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnbafbsi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3naqxcfwy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lnxajnah.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ksotnfjh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3giuggony.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wnvvcdbs.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ahcbpgpl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3shvgrpim.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3iumrucmx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xfovbeeh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ezcpdaht.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3edvkfjfb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kollhzdk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3briujgqc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qtucnvpz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fuintfmk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rmfqdqnv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vjavsqvm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfbjjeof.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hkrzhmta.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3chdfxcyt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3otkorsfy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nhyhslok.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cicijzfg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vpblybrt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pimmnaac.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xtaiaixl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3yefbycni.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zaxuedhb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3cpvwaugk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uheccrnl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3cuduepuv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jyhjsovs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbnwthvr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jvpfulhv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tedvpdnn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yvoxshra.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oeqtkijd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hnsiuvqr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xnjaoprd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jquiuprd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qmfxkgoe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wcrvgyld.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3saqcdwgk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jfodbiiy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yclxtbkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfevdsup.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ejcrrsok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqrmicfv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3glsyobbj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ylykhqnt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3kaupxsmp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kytbwgwc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ugimqcqm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lhtxsfxw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3trexoncl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qzehftjl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hezzojbb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mkxuudwn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fpmffibf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3bncsvrgq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vtcycuxv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pyojspsf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmnodwit.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vantxlmj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3joiclahr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xjnqoaru.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3itamgsld.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3kmuabcno.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lrljaius.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rvfggius.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qywiytjv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sjjwlfrn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ffpmiwsd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3csuyyldv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jccwdfiy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mswezbqt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jimcbsob.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3zpwictra.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qovnntdd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jbtagoxw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uqakvqmv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dzlmssrb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mxxpsovz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3elpocizf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3iumaibiv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dasjxxcv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3miveobtw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3evlblpsj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ejrppucf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hpqztljm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3efxzgdtk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3fywmutuu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3duxqctir.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3dlrlbzzq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3remdpwiy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gosnqxct.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3axugxwvn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hksqhrnu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qgcfwiac.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzudqsfu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bqnanowe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3siyutdok.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3udmbjwtb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xwpbldxy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tlewaqiq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zhqyqzzg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3oydqrhxm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3eonqyupp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjztoim.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3cqqdcxrn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hzwqldgw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3qvlocmhk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tboydodo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3sydzooxr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xhlncavf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3almarihk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vsiltysb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lnnxguaq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3eoeruuge.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvvbfsp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kxyxmvss.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bfxvlxmb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ykxdupcp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xzqxfbul.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vjnfvawd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kwutyghm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3upnxisuw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vsmodcke.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fplylgub.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fvdwnbsg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mkwnjcdl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xbbptcxg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jzhqfpga.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pxwzblmp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3otobqwtm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qtgpnreo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fajuirej.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dnmvivsu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gvnkbpxv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uvkdyxye.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qqgfzcsq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3npvhqnqq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zbtezstm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uwoxvkgr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uxzmgbuu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3btdmvtox.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3miptlbrp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qovyeirn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3diddderz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ldzvmxcy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jhwowsmo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nleqbphz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gcqiaywp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3etvbohga.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cglzwtys.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dqlwfdtx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ntcfcqfm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mfztwkso.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wftfsvqs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fciidvzy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hgetcttt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqfmuqn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lckzoopo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dllkiahx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zwojcnwd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3lrtsrido.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qmzfauhk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3fjrpepff.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ouygkurk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hnhtgmpi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ravurpwf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xwyeorzt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wuvyhyrj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3omlfsqpw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yzzwlfxo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fovasclf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zflcrrpd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3uxfkwqqw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qvuyamls.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3muhgyzfr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3lxqvjhfw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tabxfeax.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3pgesngvf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dyljbkwk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zyodbdkd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kxsgxrkk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pqtwsubl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3snflvjtu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uurojedp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3lvmeovps.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3znjrmsyq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3bxfobthq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ydqizbvf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qdfbqijf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wufsxsgs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rvpjlknc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbfpmpvn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vltsvhbh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xujzlubx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ujffauvr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3flxoogcv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rimuoxwo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tzgwroly.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hhkvzcms.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3skcrsfad.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3faejuffw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jxatobji.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uoxndphb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3avfqrqjr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3uajjcqzf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zbdlpeun.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ykmmmiaa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uawulmqf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3retiefpi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nvpquwpw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxjykuku.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ujwuewxy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3uovewfgo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tvlfvkfj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ubkrnyem.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nunplrnq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3iicnsaok.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ovsguldq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwsqduqp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qtfegorm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rtmiuqws.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xplygxtk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vxcolvzn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xjxnourg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lyphilyz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3llfonnon.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uvyxwhoi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qdbqvtdi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pknvgcwi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3syeclsnt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3epfspqnb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ykbneuph.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bqxznvvm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ixbvultz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ezdctldq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yfoqkpau.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fujkeaia.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3empbnpde.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3dvilqhfw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zesqdpxn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lscbtbuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csfyinqi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mjmgajyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3myqrsbqx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3eoxrfgos.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ivneqhlf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xswvlrri.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vsnwymmg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wugngbpq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lzlzqlgu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vcapslwu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wubqhgii.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xwuszzow.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rncjghap.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3mbzwcdjd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3idpsgdgq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbkioqvi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqrrypmf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nbxbcjly.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3saziyxeh.html


<!-- 参考信息 -->