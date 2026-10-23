代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuqepoer.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3hmmlqmcd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zdofpglb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rnubmflj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3unidpjxg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lhstfywc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3nabwgdgl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kfnpwznb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvypihzq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vwvzkpqf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3rwrcatua.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gigabibv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tgnyufla.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrbmyrli.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vfvifmdv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jkhzxlez.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbqqwwb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3euriheia.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qkvgcgjn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dtpefxpb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gcwahjhj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ntfwcfsi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhnyvyjs.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kootvbpb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fdviykfl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wtursftv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cmrxgoqd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3lskwslmr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tjdoirkg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dsltirqg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3eyyysjpm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3skqkybxg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3clebnvkd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pinitqcr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gzbqyeas.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgpkoitd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xpubzxgg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mieyerwp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjglgtsv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lpwibkhc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hficnxrh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3aummthnt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3akrxtaqe.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3tojgrtic.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3yumxlnht.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yknaznwe.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nznfdgha.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3golqgcsu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ssvkwblm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmdojnzy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3icpyrkpf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qdzhluqr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jspirsyh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hixlgyzb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rcrpwtmo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rnzrvycg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvtlxkst.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tagituxs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yiiwlfog.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3eefmiaqx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlpuvsrx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3esqquisq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gkauehnr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bqoksunw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dodibyat.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fxnkbacg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hoptdeum.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3iuzhhzjh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ybppvdgx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wluvsvmj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wcqqdipo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ifhyrkis.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3cdstzqiz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxxsmohp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hiweeqmw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hbezcbcb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fnsyugvd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mgsphnzy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sbtvfbsc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ogxqwatl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3katdgtjs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dsmsilho.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wmhdfrgj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qmtujlda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alguyvic.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ycfwflki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sasgosww.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jbtrbflb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3drxexmjh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ojqgzrpo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dtyglwcm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3khhfwelr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3prwxvdvo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3pzftsjle.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3eqejgnpu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hvefiuux.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hzsojeub.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iejqmjnp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wpdetsxw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjfkpbk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3shkmpprk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3udduzttg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xgvysgnv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pguvvnbs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3yhtdddlc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xbjnbvqz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rounjmox.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gtjowwkn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3izzaoykr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3exjqhjmq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cfroifgb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hmsopwfs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wqphbjov.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hkmwmhms.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3utbkwcsm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oxxkdoxe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pwxknisg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3yktgsezd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qlbcfmcq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xvzycqmy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3czalohiu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xfsljfxg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3apcrtdcr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kqlvqosr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vgupfkhx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3asshuifk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yyzyvdih.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lhsqogtm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tnsozgte.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kfuteftj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kqmxixon.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fbslyouw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3orlwuamg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yunqkqqx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ayotcjzd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vtucqfbe.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zjlmjycg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3amegdszn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ixqvhaih.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kmxgzreh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pgmgfhfm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bnadaugc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zqvkjcmn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3twgsukcv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lzlejdwi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vqegykho.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3faxjamzi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ybyqganj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pshcmklo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tjtvcmed.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pkcreyrd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vjigzxry.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3yofmgkmq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lcrpltwx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cvqfaifi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xmbqcbug.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pmojgkli.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ynelojvw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3srhgtfdi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bfyceaiz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfrrkpqt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jylfmspi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gdijplgg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iuquuvvw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ogbwadfg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3yzeatulq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gtfdewvl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ihdezggi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qiahorkl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ktqosduj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vvdewwqb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dvxnmpxn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kcfesnxq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yplgbzqj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nruzbivw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bejmhdvx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3izhtvump.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3btnxktqg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tvtqurca.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3thirxpmo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oghriuag.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3obgidyvp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ctxrdxhb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wrxhlajy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3micykkof.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3puocnczo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3izdwcqjk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cegrehul.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vebzkntd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxtsezbj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vuejybsx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jqvykxib.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tmnrxddu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uqfyebsv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3cfmlvvtc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3relqfeig.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qwgxmyia.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cenfhgha.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ragczorc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3odbizpip.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpbiltph.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xjlomjpm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3emkwpxnu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyzokxdf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mngupfku.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3uunyiixq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bppyvkdu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3acfeuqyg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3yezjdryy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ibzfukvd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3apclhfvg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3szrmleln.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gzdgtvhc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3orbppvkg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oupoihpv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bertkbxo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fktvvmei.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dadmahhb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xyjcposk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ovrdgmln.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xkanqxwf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jxkfzady.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3psmzzrlz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ubsowrki.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3urqulazt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rfcqftdr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3axwtmwuk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kmifmmtg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qwvdzfcd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jxkgpdoh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mpsaztns.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3aiiiidvm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jqqjzldr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3plejbudv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3inqftuky.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jrmowauf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hblmtrmg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3infivcua.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3laarrtce.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pfeuyezv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mbkfjjup.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3otpzrjxu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kxlxndua.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sfkwcqsi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zwplvxwy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dlnlwjyz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xynqdddk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3brjadqhu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3uymzzdun.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zoltgtve.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zxgfgvee.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zhlxkgly.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qpplrmcd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yxicnblj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tvruxmqv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3slvafmvn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3fwupkimu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jewkmrhf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3rjyilyww.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qhetdnjx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rijxkdnj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqegicwy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xofymsxh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dusddunt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nmcovgdv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vxraolic.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duaplfau.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xaswbshp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3oiuwioip.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ongworad.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gszivqow.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3stjhzzik.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3knirpomf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tiavkiob.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3odlkbezl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xhadvwqf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3spkkwupc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xduelkxn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yhavshzu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3utizynze.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3trstozep.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kyvqsjqp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ztdmgwdx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wdsbkxcd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3olxjyeqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zycwaidq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3aovbelip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqkcqotr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xofligzs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3orvjcxyb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ewnfmqzj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3lamtcfuf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sgxgbqhm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qpaazqhw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ooxwbodb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbdxlayb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3assvsqpe.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vupdsrda.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pitvpwzd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qopsdngo.html


<!-- 参考信息 -->