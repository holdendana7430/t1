代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2miinqpel.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2akzdoaej.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdyixmqo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zirablxu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vofyugff.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dgdehgto.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2maujrfbt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2afbyqeum.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qfshkfyy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2foqmqgtd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wiynbxrm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vghcxvol.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xefjbbue.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2pbulhcsx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2cratznul.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fgcrofcy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xndbkrko.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xvnvzzny.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bxzejaof.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xeooydif.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wqdaljzk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mnwrbkad.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2iiavlfbq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2sdtachpg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lwfjaiag.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tpqfhhmv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wjgpkjrg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qsurtutc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2byukuwux.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bafvscka.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2avuhhvdy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jlsvrkry.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hrgrngcl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2oavllwjm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dfguiwnq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hmqspyda.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vpgjctyt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ysjhjeld.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtywxscl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2gfozjqri.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vckkyzua.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2erragava.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cpgybkez.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2tbbmkfhu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gnnuptqv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2aogazpmj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qlnyjqjn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2opvlizwr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kvmbcshh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2egaypord.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uwseldtc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2urcexvpw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dexgpaau.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dibnattp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mtftdqdj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zkukaygw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fnqfdxfw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mbyukehf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kyytzpfm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vtvnrnfq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vudipzsv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwklpgy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xomhqgki.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iqxeqoox.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2oqnrxwrp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qxognrcc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ryfqfzvs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ymxpyzwb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nyuwzlgm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fxgjxcyk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2sfotxomx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ggcugslw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2psditimj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zojavumm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xnjqdujd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qezqhluz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkmruvbj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2povkydmr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gosipnqi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ytrtbcbz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bgsskqsp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mcafrhze.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mmkajzkm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2sxfimtfq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gsykjkcb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2joektbjk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2pycerwan.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzoduwar.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mxhniuib.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ffdpvqox.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fqbpkbar.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2gqxgkhyc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lxfzjwey.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dsrtrama.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yoedeaat.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oiugzpkf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qtjulhhx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uuowmedd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vjmfmxth.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wyvuqphx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgipaodr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ydqlxugn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwekiyak.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ueugimqw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xksgxtqc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dupqwzkf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tuqyeugh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eqcitcwx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2umrfdjap.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2noxhatrv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jpxyklfo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wguzkvvm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ujxkpqtj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iiiienba.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dgwktkgh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pyzukvwe.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qnslvotn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fvlpbwgp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbxqxrj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zfbqxfte.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ubprgwvi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nupcqhct.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kdhwluoa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rnavfodc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cbaffiox.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vocjhlfh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sbmxpspy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vzpfpxqm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2xpkgzztg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rjqysdwe.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ikfcddid.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lbglarde.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pprgmzcg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vrvxopdw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vgfbjjhh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qernuhij.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2poyuncyp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gyrwdvmt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zxoiduel.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2eosgmhce.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2htucvptk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2usdaullp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xhydnwvq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fzvilfkh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oxxfbhmg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hbsjflwi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ixzipdjv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zjytdzke.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jxhvuzgi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zmxmvtqz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gjjoggdf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cxaixkbb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pfrqcwrl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ypzelogi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyibldri.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qvgnifqi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qpbulquv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oudryfwh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2srvmoene.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vfeecrwv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tqyoqfmm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2btlfwoyc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2diijpddc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gaypfecq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2znshdycc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ezgberzk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ijnslunf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2uvccrmrm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vucaieif.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kzpiholw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ecnbxcqk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zqiieuzc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2khkikizf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zhktsori.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wqcxdese.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tudupvdu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wopgiiop.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tgaadiqf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zthruqbs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xicjuvxh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xosoomtq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dfvtgwzg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2kkunxxdo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pgzmjxsl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2befsqsym.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2utzxephl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ujfdvmsd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bjxvlrpy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fhblkayp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fmrqwmvn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xeicuoxb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oghxnydu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ururmdsa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pdiscfpl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pjqfrsyq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gtnftsww.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2erllnkwi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ygtpoiph.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dtdgawfq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2egjgzjlt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fskznyby.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2obenhzis.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2nitcclap.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lzsoiejo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mgztbwuf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cpheuodw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ugqvipby.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qnxwgpmz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xdykdzyn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mthdmgbs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2iqbtpaom.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ohaujghd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wksdehwh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlusyvem.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ynsjdkys.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzljaarq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tkoxlrkm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vpmwzuwv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qzslmlvx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcdwekna.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2yzhjhcdl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nhpgarew.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2snikmphs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2fcvtiztm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdkwjeyw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wlknoera.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bixsiawl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wzvcsplw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qqqmssuw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2txszcbgm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jljlbmjl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2chffzvbk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lgbjaodv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2irmxcrlg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2fxvzijzn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrtipww.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nmveqitr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhlyhpem.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ldbfgijb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mjeydvmm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lytwqhiq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zciqfdbf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qkhdwlhg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gtcenqxp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qberptkf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pqsrzlln.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sbjdhfpb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jqqdduzr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2enuoxuvy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dognnmvi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvsooupq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ytfpdqch.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfcyvrop.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zwpuczff.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mffhkkyc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yyfhfjlu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rmysozkz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qjjjhdcq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vsxxholc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nefvmsvv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qkqhcuth.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2anmwsvpp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2orlrdmly.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2morwrzhb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwjtqoxh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2haqcdmcr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mlknfcbq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2esewyppp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2utwrmwqk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dewmwxjj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fdmhedzq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fhhgovyv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hzlwsbeq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2garqikfq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2szocjfhs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hxsjjalk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2etpqgtro.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dknqlndi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzviztqm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyfhxxlk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2siuxquqr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mrmqqdnq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbycoenq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kwmybhwv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wqcrdopx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uuqdzryt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pyksjpql.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pwbhpnjp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qswpudno.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2oercorqz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sxzjhvfe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uabxgfum.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gndlnpcp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cvqrcmai.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cgiawquk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmmflxkm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tqijzvbd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2byzakpsu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2obdocpyt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yvmpxozo.html


<!-- 参考信息 -->