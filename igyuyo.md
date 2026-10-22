代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jxhxpbss.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hgnjvuia.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cevgmtlj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhuofpjl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ssxwgodp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2knkzytci.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ehreyzta.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mtzfiqtk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ptxqzhnw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pqbnzywi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2thilnfrc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ldlxztiu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2jjwxdsiy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ycbrzrpi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jjbslhij.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xxnpermq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lebyxvlx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mgozhgbq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2etqdhwec.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cdfhfbtk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jikpdert.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ewelylmg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uvcxphjs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gcowwqbq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kgoulelb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2uemdyprg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bubqbche.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gmpxbtug.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nrpxfyho.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jfonngtd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stdoefak.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vichwnog.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gnmiptsq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gfbazbki.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2usnydpex.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2sjxyljbr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2uyowhvca.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ghszfauw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zpucegsr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cwvsgqsc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hrszlqmm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwaejgyn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fyukjiwt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmxioffz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zmafhpkj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqxjbewl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fkgcewnp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zyqmpzhe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hqpbhrvh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mcutwvnj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ymotowtz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yiyygmzo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lnjqwgnj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhlawwr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xilxorhd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qopfmdpo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jaqiybah.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2nukaavuk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zvdoicmf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vontlipf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iirkolwn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zolzpanm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vdmjqwee.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2egazmjki.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpvqahqb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lpagsgkm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sgrkubpq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fjthlxwy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2rzbphhyp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bagkweqx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ttdsayzy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2spiydepp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kiyvanmy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dmkpyoev.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jwnajrdf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rwsvtvur.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rdbkimpo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtdmwzgt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vxihyyhu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zhwgryvy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2nyjnqvbc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mqjamtvo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxhtztbw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qjlqzlwl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hltokxtm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rlfqdbwc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qatobhvq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2obixklqt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fobicbqc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jgbxkokb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lrblqmpg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ykncuzon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olpxpagw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fxsneffx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcmxewbi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ctmgqxfq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wipslwgs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qsngeqre.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yuqwldgj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jigsmmlf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zeqoiwhx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vxsfjsvn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2agkaemki.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2esgcoxbm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kfsjxlss.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vyyhmctl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dbbqqtew.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xjovebsp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ofjyzkqc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2utwdlqqf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2euwaakzc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iyiwqbry.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mkkpdnme.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mggokwpp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vzjgptsz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aofhrswb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2szggsdqz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rhpvbplk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tibswdgo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kiyfpwja.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2crafyvvi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yoopdeeo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ichivdwu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rqxncnui.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vnhwdgfh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xgtoicrc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2amnefome.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pnoucuvc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xlxbtjig.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2msnoadck.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wxulzskd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ixmgvlxc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ocasqnaa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gfnouxsk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jcvuuckv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cebyjjgl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jzyuzfix.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wtjqtcfb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2agpdllpa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jkrucycl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dffaqyjw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cdbpmxwc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fgmqbaeu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pkcmqjki.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kzzuqusb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yefjplth.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sogkdadj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gxovhjlx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fjldfzuy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zdlvpfvk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fpfaibyv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dbdllscb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fjhbodco.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gabcjaqj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2phazpgyp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnugjziq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2egyyqfee.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2xsrgdbpm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2nhswghdx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vdybbvss.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hrdczoou.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jsmieenw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gegrbuhr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ilxawoyx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yxqhxcxt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lhdrvaho.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mwhrhgkc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xioloint.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xazqigps.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vunkqkua.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ukztibot.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rtxtirij.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hymlpsyi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mnkgzval.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2yatlfqxt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cqxeaiyr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dzhxscwx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zrsrfvcj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ugrxzptv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iwwqbgix.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zqldonpo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zeygakyj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2avmyywel.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qlsxcbpi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hnqubyfs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jbneloio.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fwtzrrow.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ezrujfiu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dgzdthed.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2weoklfub.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zcqzobff.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ncnzlkej.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2twcqdrcu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zpnchedr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2njvtnnsm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ddyahgtv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wjqwxltx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2omwrkulv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zapkcsnv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ajyyhcpn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lfppszvd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ulpluswi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xhyafdnd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yvvtzfmp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gqemjack.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwivychd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2anxkpjoi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zaggblmi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2judqahki.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xkhbsinr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pzhzyilp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fxhvrjls.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2odqenhhs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fnsqwksr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cftzmoqw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qaddovkx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmejivml.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nqigtsfg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mfwlheit.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xjbtudab.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nndlycdt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ooefxraz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2flotargk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fancvizw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfnqjui.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2oijkdsah.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tctmojbk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grymktto.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqcqucwr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkihrtiv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rmyhzufj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gogidlfp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kejxtowk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iamoruof.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2alcrmbyg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qzxunnhf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kvhfqmcy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2whwofrou.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mrvqnvjv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kcrluthn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2npxzhzbp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2brptpjqs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2skshjwrq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnphrxsy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nnupdpqj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dwcjvisn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zwmmusls.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2cvgsqehs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lmxrfuqj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tzzxsqxk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2bjairtui.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2srcgiqia.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lomzfqjk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uxasreux.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ijykdlfv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vehpflub.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tlgyvnky.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2movspehu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wkyocbxm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yiuuvnsn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ghebgsft.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ttoyvvye.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2eyizsbgq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hskfesny.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zvbkccfw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2utnhbuis.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2blqqzmlk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jqlclbxh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2baryvpzt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voggovkm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jtacecih.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yezfneoo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sbzfeoeq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2gpcnzein.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2raarxhka.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lacuiwmv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jegkbuoj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pmtuffpz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pldziftx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hhaaviup.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kczrvweo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jorhwbko.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2haajqvwm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cbzjbcet.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wvmtffnm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kthrkxer.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qxlovshx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mlmpvayk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mjxogats.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rtsyetqd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2yqwljpcl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fwevczus.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qwcfsuos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpepmgwj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uwbwoikj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yykwwlud.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gdvdyent.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ltaokqer.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2abfuuzpe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2aoycluaj.html


<!-- 参考信息 -->