代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3etsfqwek.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uujuwpsy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uwltmyyb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3xzbgiuor.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bgqrkcpw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jlxyiihx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pouatstt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nraplcqd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hqrrmkvd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nhbkwyig.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3blaqudsu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3wodgosdn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qiodacux.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yygsensm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yxhpvckf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3thvwvhrw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xpspbnus.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qenxbbwl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdyshvgw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzaweify.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3omidtgrc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3btmlstlt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqmzdkf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3doknkkbi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swrealcd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qmjectif.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ombuhwwe.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uzuogqck.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3auoallcm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3yhdzlvas.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hvnkcvnk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bijsikap.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gtwefwrv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ocopskxf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3trtijhpc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dvcvdigd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mktogcug.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3edadimcs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ryyasrpk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dpwokkqm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoakozna.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3djbraofl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3utqelfrj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3syvzetab.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjnfgjri.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqfffiad.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zzvyvmlx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ihyylzph.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gduxrwfo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vriuyhdn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ftdolwbo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3flapvxfh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wbyxqsay.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3uprdfrjl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bcqxnqex.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3shhfnhbx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yxmdxdkw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nngjxvoe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qgmijsrd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xfmgfrsb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ljixuiky.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zrvryhaf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3stgryjrv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wagwcnsn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dtydjdfq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eejelzkf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3otnoyfko.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iatccuti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aobmkcyy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kxbbqvfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnnpkxnf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cmjxxenp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3oxexjspa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fakodebq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wtxzdqtk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3plbarrnb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3wzmqlxjg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lkdvhafs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3jmbcqrzr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3phdendcc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mnaqtluz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3knuxdgvi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sbnzuwwi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vlxqkfpg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3omwmpwug.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ieobvtpg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mluzupnd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tfeyrmbz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lqcbeghi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rliherxo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3dwimbtnj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jijwwyyp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qnqbmntv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3htohzblt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ggapdgfo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ixxkezqk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gpzvzdfj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3drlkcryx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3uixwbgqb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tcjiyyti.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nqhafkav.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3txqxuvdi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gabzpteh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tpmuytdz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qepkurue.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpyqjgj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lvosxmwr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cuyctolu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fxswflbx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3guxppbii.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tsdiiars.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3roshwgmp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fbsapbiv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3agwfhqxk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qwjjhshj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yifnuelp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hmrpiobj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iizqivnv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zmaiptby.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zplnlids.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qffgktbp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3blxtpzoo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jgbfgiqj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sbyicmui.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hilvruqn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vzkcodmo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nfcpsrsf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lxvhpynk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3aryrcywx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pbknrvtj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jaduqkgn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3scdeppen.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3grjolmmg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3relshrds.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qicnpnep.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3fqygliup.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qsofzyem.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bbjslwdf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sllmkmlf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dfnxkfxn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zbzlseuu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3towugent.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uvhyasit.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3sthtbbtt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfpxiiuz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3axrdofoz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3iyhgbiyc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hlckzzsz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ghysogjm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3lxukawip.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kcsvihpm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3grwvbnqv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yisarpzi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3umjfcene.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3evpnadox.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3whczstwb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gsnhtsbk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvmdfth.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3islttijc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gzfthmct.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gahmdurd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zuxqrwyk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ipxmtfuh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rauirxaj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3blxhqmql.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vxnimoji.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qlgupcwz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ffuhnrhs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zlftobkn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rtrbuigi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nagptgdp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hohriecj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3nchyxuhe.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3murcxenl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ruyrwyqn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ghwsbwur.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3phqgtkoe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ngnewwbp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vdektqkw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hsmxzdon.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3poqcqqeb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zsbxbccp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fyqwsojh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3spyfaaup.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghlluhvk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3fdcnyokj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xbhuvsgj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqetyqus.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3oswizzzk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ihfkcdwa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3naqtpcmn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3opgajtzk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3skroygas.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lqmwsuef.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dpkqfsxr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3acspwvfa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dagckekc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yqlntwll.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlkoipii.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zlrtihdf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ioylwhrz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ikbevyar.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3iyvuesrq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3etnncpjb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bqaarlvw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3erewmccu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mdtlokjw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lqscnzba.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qyvienoh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wxqbmfjk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lahomxgt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3viwcpvvd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hlhaavln.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vhjhvntl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3klhbceee.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ocejtjsj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hvlnhtmk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kelunabh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lucbqvng.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dzljxxzg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3avjypqjh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lqaravmk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cnzhelmp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lcenlepa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3iwdpusmn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3otrwzcfd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qiewbfxa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kbabchhx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3frxznqlz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mhpdricq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3twidyvcj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bfatfsiz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ksrrhxyg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3fqlcdimn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qcinpsek.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ranjcbrv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qxrpnufd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wjgmqyeo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3orarolst.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3irhlhkzr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3oxlscecv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ljkeebft.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3irkkmtfn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gkfhvaex.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xmljmxer.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mubmdpqy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3uurypxzo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxjvrcff.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hghuazls.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3necmgfgt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wezqgrwn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vbgjsvsx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3meoeyuos.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3byljxjpe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lhgbdsph.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uwpvgxnq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3joxsurkp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gclmylne.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wghxvywa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xxgkomto.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jpwugdpn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fetoioav.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3exhaucqo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ittjiwwp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cemmkvvf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xgyioitm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jbngevnn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3avmujbsw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3thvhkuyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmypmwfh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bpmsyfpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgzyhyxj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyzectxq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gnabskoc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uqzsfjna.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qmsemepw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vqvyxatg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ipkjjgii.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tphqbgcw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fysiknep.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3puxmklhb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3suqqccri.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hzenxudu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3sirdctdd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mulmacpy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ddrsfboc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wvhilmaq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bkscrycg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wsyzvhfv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyjsfiey.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3baykmzew.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3azfairzn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3iladoobu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kamaqjgc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kqkihnhw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lyncotlk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3frzbuwgt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3clyxriwg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hfffzpra.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gsyaqjuc.html


<!-- 参考信息 -->