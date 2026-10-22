代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yuwzpdjq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2yzfvsvwj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2aiphbnec.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hmpayfdc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2htbgzwpi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2trijgxip.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2axnddpgf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gkxwxbfh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oyjrlnye.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lnshbdtd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ajnpzejm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tvlrndos.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ykjthali.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pvoouqco.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qiyghktu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yalmoiiq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nbcfgcqn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fyncskcc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tkxmncoq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dapavfzu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fkylmwlt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oxrvcnrp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qswvqfgm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ihwpxnyf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dlwyoshd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mkmjdryr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2juipgaol.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ejkzuifq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vwevpwky.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fcqvpyie.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hrvjopqn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gydmlfds.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2gafzehdf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xrvoctzf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cthmnhnp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2izcqoeyv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ohamrris.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fcisosvx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vociexrh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nmytauqt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2idjswnen.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2baxznxrd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sxgbpgty.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jrfgzhbf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lddwyajg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2huqrcoaf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lqbrlymt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2juwwokym.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vlazgyrg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yjiyvlhx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hnjmggfr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gvkolzqm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2byttmmqc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvryjwmn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tsfnooxx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nwnczgcn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fxvuoyzr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmkwzot.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eezadfzt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2acjrpwwo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpwzdkqc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xovncmvn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajydcrck.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ppbzixss.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2edxcntwn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2aexywpwh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wpfowdku.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kuthiaqw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nfuhnswe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkzcyyo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2gpooyyfv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ynohdndx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2likuuvji.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxtmjly.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2icllmdqe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jywtngza.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bdaeleuf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2cqyjyhbz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2acurhzmv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2aozhymih.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ywpuhyak.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2solhivik.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2mjruouhk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tsghhewo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bbpxftrd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nonuwxis.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qndgoang.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pncwxmob.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xpehgedi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rmoytobl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2otiuarlh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmydebjg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bjfgxali.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tliuoxli.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kjbaisog.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2szleclue.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2efkcmuhb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hmxeuifq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ackgwcad.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2usqroiin.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kxtjttin.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ukzyonkt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2crtyayxf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ptvirbwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mowdwtde.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2sljzgzmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyvtrgnm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dgfdrbfs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ioabddwt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hyljuegu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pvxtprsn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gbovrmiz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2wcntqvjs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2irguuubj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hcwpnlpg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2glxatcdn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kvvzhqqh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yinrrpjh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2twdzcynn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2inphbibi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sweuxpjf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xhjveqwu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxgtkks.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mrvmcvft.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vcchbtmc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vxiuapla.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zgfdzpjt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jbwvxkif.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vbkfkxcb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fqcwfdos.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ohzwefpl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2obpqxztg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2waxzrshj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2snkutqel.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2iewdvbvv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2timucsam.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2umzidced.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jdgbnxhq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yzukwhau.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gxtdhlqq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2behjdofa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xtiebvdm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yazzahxu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2yuiycnsl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zdvxfhqz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xywkqhzo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uxcdvmmm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2alpyonaa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nrhwxafh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2sdgdpdke.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnvgkxwi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oouyyfoh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rmknbyjn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdbnebl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2krqgjmet.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wexcwhei.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vmohgcik.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pqzjgsha.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2klcruclx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oxidnjlw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2omzpjyzd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bcuwgqrw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qlvbahmz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jwrmgmtl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ezzhvvfa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2shmpzqtg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2uocrieww.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2myopjnui.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fgrqaicm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ncxoytwm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2lbhvbxdi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zkjtruow.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2iorlurqg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ednmwjty.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zgsmmrtd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bcofepwk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cbaeaghd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nuyngbyf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vvnpcgrg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2khlhwnze.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tdwpaura.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sxrtuvnw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yudadiig.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2slcjcnqh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aqqkikgr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lfbbytjv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cofgjghq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qhvapvqx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2lwhozvii.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xjinfyzj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wtonsjzt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aebycwft.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eqwsxsns.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2klglulfr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2owuusbha.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gdvumieb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2oockuzsz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pimbgrny.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vkwkloum.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zakgullg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gwckzgwr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vxobbbax.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lhzfhfit.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aquasvyn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zayrquqv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bkintgfz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ailcilvm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hzgqrbnw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rizcmauj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nwdrjmqs.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dfmqcipz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ovtkxqsv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kgitzfag.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2isfjsmet.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2hwxmlujf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zqninrlt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fhlhxrji.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ofddmwul.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cgazixnx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rdyydpny.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpdpibnm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wzrfqypf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jwitvrmc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sqybxbeg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tftdnxti.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2beiyfijd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2mqqlqcqv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dysmzjlc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmbmohue.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vycjudqj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2otcvgyfo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rzgnqirn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2odksybwr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2owbiwygl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2cltzzhed.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2erdawpqo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sidtycwo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cdesxdzl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ugmkmxjp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tglkuvxg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uimrqswv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2apmvokip.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2znaoqmeg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bzsjnzdc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pmtkdhxc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jctfmvtv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2beqkmcdk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ddganxff.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vpadfvky.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2cyvdzznf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2szusmjvm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2tbquewmz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wgbxvwnr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hgtxtbct.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dyzsnkzc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2psswguca.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jkwdvspj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jkmoaldi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xuzwhvqq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2dprkahfh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uhfbjpoo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ihcsrsej.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2evvgagqw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2omhazjzg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wfirhqtk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2klghyndt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2girfvbsw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2axgulisx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2svofaoxg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vwirszvl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zqhhbxzm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ltrwgotm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dedvahjx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nbftenih.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2reltbdfv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bmeczdho.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zcoerncz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ydpaygyu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2elwxzksm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fntrzosk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ggfsbvgj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2faoulkiz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2asmlprng.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zpqigflo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jjecjiam.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2eqyhuadx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ofemhlkv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2azyjnlgf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lexaqtzc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mjlnkbur.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pbecmwjs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bbacvxpt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jembnsgh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vkdokywp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ofxxyfcv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bumtaubo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2asmvayfl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kglgjedi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tqawfoes.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qikhwycz.html


<!-- 参考信息 -->