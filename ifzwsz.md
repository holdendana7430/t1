代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qnjdvtjv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ajcehfxe.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3alrljiow.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3apudqxzl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rpzuhdww.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rusmovwb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ysdgqzww.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bvtpzxzh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nfppoynr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vhdkkivo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3obwnwwid.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vfvfcpqu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pedwsahg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xwjlfecg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3blqbxajq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yipgoigf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wlojnpex.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3otncywbg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zbxhemyf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xnswbubr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yzgufkjv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpnoqxmo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jevevmhj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jghefebw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ousohfyf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3szttelfc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3twycayfi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vcvppivn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3lpyozbcq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nrjzpguj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kshcconl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zdotphxl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zyyanapd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gvglyqqo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gicpxezu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3knubdtir.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ckrwjkng.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lijjggdm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wqaqqunl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ymsmtsil.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3oiiuximw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ulxkaclb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qewjtzoy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rjkiezfr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mxnptolx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lglyjrfs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvpiplbi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rtcknxxp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wfbaioaq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fakfwlcy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lvhgbpyi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3einacdpr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3lgwyrxbo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mgmqkclw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3elmblimo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ucljisze.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3yaicwjku.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3psesacbm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qvsdddhl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mpdktfmq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3babfoztz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3okqelhmq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lyzajsgj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ibdprush.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzojtyyn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3yzusylmz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3kfxkuobn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3acjvsqjn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xelawndh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rxbctrpx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ksrcfurf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xmwunjge.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hwifgljl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3nclrivts.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vxubhafm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3bqihoosk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3btdysllx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtgjbgws.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ylanviqd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qgiqvmde.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3duzqlzzn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjooegry.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3llztvzsz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lkjklaar.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fqivmvsr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3leseuksv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wsohynym.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3opgmcvcc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3koowxrmz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ubsepiif.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nvoehkxg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nvlpcqtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptmtrvjr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3agkxcpzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uovdtfcv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iwoaybab.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hpgtiqec.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tupuxabz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iogmezrm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hpzbqnyl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3omhmqvsq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3utltsllv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3udjnlsbk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wqxzagyo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3sxssibdr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tdjpcida.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3erdaeurb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrxqglho.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wvorwjov.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xiertsnb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vnrtfice.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3enzggezs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hhxjnjxe.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oyshubtd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vopksjtv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ofxnehok.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ndacealj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dzwwzypw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jgfyhtge.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rlswchtz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yjiggras.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3vztnfnoo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lfizgkji.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ixpilqkz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gxtbnysz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3exxumfgm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mxsltgko.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fxzpatbz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3junexcxv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rcjuosgy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dbmoasvf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xylhofqm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jktegpfz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tunpeifg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hnrfhkpn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jhtnaxvp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3duhqzolw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3oddaqpmt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3sjxlmtnk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sachsepm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gjaptbju.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxmaesso.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bqknlfix.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nhkidpkj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vunktuyu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aiscznro.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hwibobmr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dioizjxn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ejqajkhe.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ffbhbvqf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jacttlyb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xwumdrdk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cjygrgfp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xmxzlxkq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vwkbwrqh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vhbjruqp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xcakjiej.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqzvkpw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3oojbffrj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vvbrxzvi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wntrsrtb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xkwomznp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3chdykvpm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pffpvavz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ltcnqwbs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fmydqyfs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3umoscpjh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3srbxfooi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpxkithv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3miuvnwge.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zmqpgbgl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hkicsxwd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vfzvrrdr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3drljawjr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3nejvagda.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3felaodyl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fizwtykk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oivknlbe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3xpeylrca.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vkvtbvbm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xualsbdb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fhkpqbgk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hktsvkoy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3oizdsylp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dvadeaen.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3crhbwcrp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3usggbhax.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqkigqrx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vavxfkpo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iswlsyhf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uudolqhp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dxahvwib.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lsmnaiyu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dmwhmexj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kfvzoegk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pnkwbpbh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zyipwyas.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vyluhrpb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rkoqgpqw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3snpajjtp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bmljbfcj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ggraromy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pqrnlglz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ccfvhtoh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3jualfscs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3oltrtpkv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ilncssfv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sufmqxaj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnocpxax.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fvrdkkvk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3gnbtlquj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vuetjtwo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xulkmpaa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3bwnyebte.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3iqiflyak.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mzsewxti.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hdbfadzt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ikzloekd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qslyhzfq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qnsrkwqs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3txvvwqua.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3npckgavc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wwojckrj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cfzpiayh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uaqmxxvl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3dhydsbbk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rxheqrcr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wkqvvaaf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvgrcpki.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdeaohkv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hpfjvkug.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zetosfqp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ihndhezv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tzosaepe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nacqtmvi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bsoyjvue.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cqxkhtxj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3opfoiytb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kjxiqsto.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lyuddvpv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tnkernqa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xjcdgcva.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wbnnyhck.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dcawseyo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jupmyusq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fedwhpoe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jxeufmdt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3erwexxga.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xtfkoxuh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3lrioklns.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lddnrlve.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nvwbzjao.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wtdtftrq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fcpvozuy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ciyagqji.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3odpljicq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mjhdwrse.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xlsqnhcr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mclmivkg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gfayiboq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jpcelmoi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ncehcapf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tdibxbdl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ffnqwupo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xzknvfdv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3caoiitqu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wfzfrbtw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3clcsmjew.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jicvjihp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qklyqalw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxgrsoia.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jscnybiv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3prebrjzz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3gtkjvgxt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgzytrqg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jmiqxlgy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vjmuupay.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qgbcjshk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3njbzldoc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ueevjfdp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vvwtlirc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vonczvos.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3njodlbmz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ibbruirf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dsmfrhtt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3yaotamnd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kueusimx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mjryrtxx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rqyvckha.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tzemycsj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3psaxdpyx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hcgefxtu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kinnvecd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvaodkof.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cmzyjgvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucjkyujo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lyjxffgn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vvyzmcku.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nvcjdepr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fywjfmdz.html


<!-- 参考信息 -->