代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2logqczmt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ovupidfc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kusiozuh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2njddgbjn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jmoeaigy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vzxhsnfm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dqlrdxcd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2kvftqqec.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ljglqfsf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2uabruxyb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ixypoyth.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2erxqwvpu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pvlxrahc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mycteqxo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ieypqids.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2tzdoeeya.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gckccuut.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pjlkyqup.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hobdlpva.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2fpbrdley.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2feiwdloj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2txaqamyy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2frhqelxn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fsclikue.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qyuviair.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kcrgixnl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uephzitx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsjfbiro.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wzyylnpy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2febrrlha.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbqiwurn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2yemudosx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zyrnruty.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2idrbavus.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2racjvbcz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ffoawewz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xyblojxk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xzdkftvc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2llgiygms.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2izbicmqc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dnughwzn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2jhrtsfql.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2scejuvxm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gcsjiffm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uubwyxua.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2shpjojsn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hkkyzwtn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wzheymxc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2oyadlwbg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rwlmsblr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hqnavngb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ttssuusk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nbzihvkm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ttlrlmdv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hfacfekk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rxoublds.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mtheqqhi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ptmobehs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ojyrhxes.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zfmblrfn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rlezvonm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xuezisck.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bhlnfegm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rupzgjyp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2duftiixy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hnetkezc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ohzlmcps.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zihsecpq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dgqoanuw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mrutazeo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nkebqcye.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dmxaaisc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qezylayi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ffrlvswa.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oadvzkqf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tyqjnija.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izdxrapg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bfznddxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbfmixke.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2swxgcoog.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wulvgxzw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ppdegxbi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vjrqwwsu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jahutaph.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2owdkjobh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xcwmpcep.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2aihgmzwg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ouibhcaz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qqndpcmn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ojqnntal.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2femtbprw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dvnohggy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sdomviod.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2piexumvv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqyqxoty.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qfbbgxsl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2oqewufak.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ranifppj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2uqzrggau.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wuxuxnob.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2utvqgfgi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vewjwqpl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tlgrhefi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uqdxcyea.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2slcnbojx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2esizztdg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ggrepqqs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ylcxheck.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ncrrxtac.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xdgfuxzg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uraftend.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xfdqiqbs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kzdnelyf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vnsymxyt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2crpfivno.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2sepkyifq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qhcitutm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nbkrolhi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qvlyrrzb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2clnpjomw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2djyajmge.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ydvwcnjl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2daecpwrl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hncfqajs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ujmcboop.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yejhrquq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2yvyhhceg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ufdqagjk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bimeiawf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hkxkybcj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnoeqtqz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ptttycgz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kgfyombk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2okdykvti.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tecykhnr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nsmgrbgz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2wazslrmz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qycieinp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jcsazjno.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gocsecgc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vyvhefvu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2trhefifb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2acbaqegv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2piqykowf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bhrwesjl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2unuaeybc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rnshkfqy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vrzapnaf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2caaevwho.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lscvmxsq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nscirhvd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hkexdeiy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gnjhszll.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zrpfxpsv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ucganqbp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qlpyvujq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zjghgduz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2arfrzuvt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xijcsyio.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bmcvdewn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2sljywozx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2giencjgm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fezazuni.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ckkntssy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2igssfcqy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dfqkkldu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uumgxrsm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ibkfhbmz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vxagepkl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ssymjury.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yaijshaa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nrabfbub.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xorouxwh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lthgeyqj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dxcknurh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2thpbeajx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pvwqpxip.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2szerjeow.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lgzwrnba.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2awfzforc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jtsojkqd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ptqyrumd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xgdnrpue.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nyhwwrdf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lsejbcme.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rfjkbiek.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bzjngzfi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vgovzsoz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kgtkjrjf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2goajpjsb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cqaarhmi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2njhqtqnk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2abtocmin.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dymncwae.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2txkpzveh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahifqmlc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ettwxzav.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nlftcled.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ecrkckkw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2eomckuvw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqsiszrv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kkhztimm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fifdrvri.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hkxwlibx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hmnyzwwg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2roippcne.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nharaznn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xwjifsyl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2idzfegzd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2uuetklep.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2yzjchaxh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uywdsazv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2znnpuznx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2zvmeqysx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sprkqkbm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2khrirdlm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2szanzvul.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qujgildi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wwpwmgvb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2baiykokb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kauymgyc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jqiglpju.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hzautfbx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kwptblrn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2pzszghpu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bpdojbuc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zhjjsxgo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nybvooqy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2uvoghkmx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2atljwmzi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sccyehyf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lzesvtwc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2bgysretf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2irneploj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vmndaayb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nguydvcq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wypzoxbm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yyejhujh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hhrhgqyx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yxymapzh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zmcfwqrn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hpnqnmrd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2afurcdnm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ptpujluz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qfqlmpzc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gsdvrlas.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2anyaojrj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ewoiffjd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vnxmlrwb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2drttyntm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rceereji.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kvgvfmkx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2owroeleq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2noqdvjqn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2envtvpup.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycrpsmvx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vcdfaqpf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vrcfrbjr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2aqcdfrqc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eozqyqjn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lwmscmpf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zgugvlnv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xifkverr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2efxdbalf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oaqdkfiv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2lzydktjb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2anlldgio.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2argqmtxl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2burpflla.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mmizojzk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cvznqkbi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dvmrncag.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ogxpyhhu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ivsqpjqz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hqzqfwtp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hytgdfgg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ubhbddkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdrfjwnt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xbhhtqlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vewzvflq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lhhcxwba.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fcvnkpgr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2upocydpt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hpcznosp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2frublnyd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vbuorcdk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gtsnfcbf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2slridcql.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2areyzdva.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fbmrvxvf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2igymffny.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrqahiuc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ygplogub.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rnlmnpfc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ptunvbjb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cpfkksxo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qmugvwjy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzebovve.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xadfpvaw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2idpvkmnl.html


<!-- 参考信息 -->