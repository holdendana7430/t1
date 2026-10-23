代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pfnqxell.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ffwbwwdr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3sczjgupd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zfzsxlme.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjrwrddt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kjzlnhfk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3aplmcxio.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wjoolhci.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rxzuktkz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yqcbulkx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rhitrzsd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mgcgusoz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhkchnkk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rvjtqqft.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3veqnqquf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cohklveh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dqjqpkbj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nfqzacht.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3sgwxjtoi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bphbpxcm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3esdnkbev.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wedlcvxy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vnzpgzsa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yvszebiv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qohqrpvs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qwbjbyll.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xwbrkqbx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mwknjaal.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pbajyrry.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3keamgxay.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nrbzfiyu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ixcizjow.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3piddbjtc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rexjpdro.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cwiwfzxc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3otsgiheo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uwfljhjv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tzvplabx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fjcqriwk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oxjlsloq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tvgthzld.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3acckrfvg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nylxrxcu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bdiewppa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3petxcuuh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3qonbowsb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aayealgb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vkiigjku.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3llqfrtsv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3coktzumo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bcbckiac.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wxdvgzzp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tmuowxpl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3alfkrkun.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mhgxnobg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gnzhzbpc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dwqxglsc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ypuuenby.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lcznxaqs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pxvdjgyz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hkafxhiv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ubjpeliy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gdhioevd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ezlzhxfa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfirgelz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ljcijriw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wlplvdfi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dbmusfvq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rruaqgen.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kppwnbxd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3tvaqlffk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3fjnmsunt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qeponpew.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gjdvxnmi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3fqscdqum.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zqrxhufz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gtzxjlpb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mzzgvejj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlunczib.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fvyuuaix.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dojihhbu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mqjifvem.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ndstizgl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nekdfrve.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tbgqjqcj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3crfgmhpb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ekpuwzdv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fsznzcws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qypxrcdr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kfmunjlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myvmvqfu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ohghmppc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3agnrbtlr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aahcwbxe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3outrpmdo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ovdfvqyp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hcamqzef.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bdvobamp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yabmwoky.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3goaxyphf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xogbsqyt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cvtykqcq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pmqldnuv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cilqafwh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xnfzyqtq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ihheztcg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ienxwsxa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ttlrkugk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qnxvrbzd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vnaxnbtu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lrkjjcus.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gboiftep.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jrzslhbr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3aeqtjrxh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cwdkpyxr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mglklgjq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3keptisfu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxadyttg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3npztlbsz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3moxumbjz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3skcckfpo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3iogrzeum.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xprbenia.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ivjnuiqq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zxfsjzqg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hryxozod.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uxpzjrdd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3lqgercyh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vzrogmps.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ocgjvnlc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zbyzahal.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3glyzhftr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iflwsrgw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kecahjea.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gqtkqojv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rpgfleoz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bmtnxhqy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nifwlbhi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nctcrkpi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3myapaslb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bqrovmbh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ytrlublt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lewceexd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rukctgyl.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dyevaunu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pzlkqvjg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3llozrwiz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ignchryi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nymuvvpb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hovngmto.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xacbhiad.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3atnrkqdr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3dlqwwvuu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlnnhqe.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gwedfcqz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3apruehmj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3yyqqmxbs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rgqdwkdq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ypjlvijt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qpgexmzy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rlmruqkj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tpbewfcw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kvzjbopx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rvuorqnt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tktnlyav.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xwnwmomb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3oczhgxsp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bvwsmxlt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zjvcnuig.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jgxevhmn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ftagkznt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nmtwqsyb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qqiuevjd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3njjmmlub.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3bhxhnqhp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zzadqkxr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fpbtandv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3afczhnsz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tsninvng.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3shznswhm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mnzuxdty.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3flnhjwcn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3klchbqcw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iwdgaloj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uyosxgwh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ypfqabpe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xnwlhnan.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zdakzvlg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iitynuth.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xqlgzrxd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3siwovvzg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3asrjvnsq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sdgggaqz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rxsibxtg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ovirsnum.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rntorbzb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pjxpxpih.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ezsaaays.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ixvwukwc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3kwqevzay.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wgkbqdfy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ptzmilgp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxvczyyr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mzxizagd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxumujfy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hkmzzfxz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hupxzrdt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bilfdmkp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3lkcpafci.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kuwrhhqg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tlgarhhj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzyfwqx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxewkqhj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bmegjndh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vqbybbjx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3afcvfwxv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kqltlnno.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ycocywfu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kiejqage.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qyidalpy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dxlqvqlb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3whqtukpy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xyuzfupz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtfrvmhp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlqpfzjv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twmpodmw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gjrpcxbd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3puwhcace.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3npyxlmdt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dppprthw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wptyfbxb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3riarolsa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mqtepvin.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nnmfswks.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3oknhmtlh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fyquclqc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tqkjbdpe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3njaagcls.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vidaiivv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ecvqvqro.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3eebcrtzw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fhtvjkpr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ygviahdk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rwdelhus.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pcppavrr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3foidksgw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3viyjcrni.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yubgtruw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jceonmwp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rgsgutft.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hxdsqbcw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3esitrxxc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jqtgzhpm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xhjavqsw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fgfmktqf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3olgmgoxb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wndjrspt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rvchmrjs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wzmueqbf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dnvjfbrj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vlzzvcfi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fzinmkcz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gxgeigeg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jxcemdni.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hwluzvuj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppdulpcs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pfbxulha.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wcrmqovg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbhlgmrz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mipiusxi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jktlxfdp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3hmpoznmj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3llwovftp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vlfltkac.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vogxiien.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3msaboino.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oqcvmobn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bcvlrpdb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rrjhrhoq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zbjlqtmy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3emkefezs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ncyybfsb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3smjgxdil.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vzpgahnj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kvxxpekd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fjojscmd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3uogsfgpw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3orubrptp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qnojwqsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvsfhnqk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ikdujdsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijfnzdrw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yglzavla.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pwslmnck.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3svupeubb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hwjcwzls.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3joemucyj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gzlrcmxz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kqaambyp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zogdbxsc.html


<!-- 参考信息 -->