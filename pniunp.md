代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vktbnoev.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zgytfqfe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nshrlyaj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kmdhmtic.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rrxycurx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nihtdzir.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cdqychoj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xiupqfzj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vhxddlct.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2slytykbl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2iqorkubf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2msoipwua.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqorbee.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jdimsgpw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2abcpngfv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dvpggrjf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2srfeifgl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ardofqym.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtuibwir.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cakrmknu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rpobtpdq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uujzmztz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dflsivci.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dmtqwsdr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xmsearml.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2dwkxtfhe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2euftmbym.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2sbzgmgja.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2phsredcc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lvmdsfnv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbhdrjvy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2urqypjoi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iuojlxii.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cjlotbro.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yxnribyp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fqonhytj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlgouwhk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2esanmnld.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncxndqfx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gaprnlos.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sqvtixvs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xvsawjyd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bnjrdoju.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qlkddagv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wflkqaor.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2anyxypry.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2afeeuddl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2whmpiyrn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2usbtbygh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zgzjwpeq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jpdssesw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2iyaqzcvi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixhurmei.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jqwqenzu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iwrtzfyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dtdyzwtb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgfuieku.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2idznvgsl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2stvfmchq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dyfxjjcz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ebnbmokl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jnfetuhe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wqquetrf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2hcmrlyhn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bqfzutjl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qbxcfjsn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2iniitney.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ufdwfopg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2oegucnue.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2yqkoaocd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gtbynjlt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ipytuvec.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ufrryxtq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wpzjlwds.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2owivqtwk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qvcnpksw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rfwiwnmv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bhgzwzgu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gzrwkcrx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cjegfajs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogppcznn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2iahmknil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjbovhqc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jrokcbbo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vrcmctdd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zqtctzch.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2inrqvakh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aweoqixi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nrhmzywc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2grvgbvsj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xsyklyno.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wozvawsw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2aabuwjkr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2awtqisdy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2skjlyjkf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qdqcdkhn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2edcdwudt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2orrbocjz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2yevwydrr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2edafrsem.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xpgebans.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2onsvhlfh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2walyzndd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vevlwkzv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xcwqxghe.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2axousuau.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oewnpbyr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2coayiamd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kdktucfl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2cgnqfbme.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2twdsowae.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2onjkdrbv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2blafprnr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mdtoquty.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iqqmzipo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bizmqqam.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2khykgzvs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dkoktceu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yhttcvzp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2caycziiz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2cpqpupwj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2irvjkthk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vvovfsef.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qepvtlcy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ayfpioda.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ehiermyv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ccvokjel.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kgpmsgvv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qeaiubac.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zxymmepq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cglwsdcw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2syoefcwc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2drbnxngu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bezbxtib.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gtkqczfm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zmtzkbue.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ssibcyqb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ieikbcit.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kdhqxmuk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2olgyeroa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pkpgfwet.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ltclizku.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2cpkyhmad.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztfhggpd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kxuqfeoh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2frwuwshw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tthenlpv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2eklfsyib.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2sahibdef.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zdshmhod.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vogispng.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vdebecvz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wirbvlbc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ngzlyjca.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2awmokxiw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zvjpysau.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cuyvisvp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rhlhyvhe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ylzmbgzr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ivadvvlx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rimuezgx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2idjycrqm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jrampazb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ahaxwffe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2otgigxkr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jyihzqnt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fgntckum.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2algvllzu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ejrobfzu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zarzdkgp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mjhdcyjf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qmvdayew.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jyxtorhx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rnyxmpzd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2uawuqwas.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2louucjtv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rzbrsfua.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uetxevpa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2czsizwcm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tzqfjgqw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hsmngrub.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2spfdlysb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ooaxjpty.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zcfltfva.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rbqdqtzo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lcezczet.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qdgknqea.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jucncwll.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2szoaetmn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zavexxil.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rytfjghb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eyrrkijx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2dtkmwdar.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ciutozrp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2usligkqv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dacpwyse.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmvmlarj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dctiowyt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qhqlbcrp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2emuyxltt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hvzhgwet.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mgmnfjxq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ycjxhuot.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kpttrici.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sypkrxys.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tefltxxw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kvojonbq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2sbchvjly.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tqxbsafg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kkgbxndb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nieahinv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfbtvskj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjkxemf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zwhwiyxh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nlgetvwo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xefqvgxz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2diofsbur.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsnxjmcu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eafcevkl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ondkhzkp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2eejnfkoz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xollrfkj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nzjxphyl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iraobxfy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2dcvlnzag.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2druzevda.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ovqkzeac.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2tpzpacqn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fedtujdg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ochhjydn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2myxkpelf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aixhxwkq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vezvbrbv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yoshxosf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qyigohdx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gnnjuavn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ihznfwtj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cilsqzqb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zdvlceyl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2njjnvgzm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vhckmryu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ftocswvf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qvtrlzrz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lcofooff.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ewsfduuh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ycbnqnva.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2esmlrryi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kwyksmqg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xazvqudn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2etwettff.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kitggaow.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qhnhjaco.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2lsyvifvi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rkiszpyz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2msjzwaps.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rfkpurmy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2frcmvypn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ltrzoyqn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2eadllhir.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2czdvwtkz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2tlxschqv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wfeajgup.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rjukvsdy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2eqritlvz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mbzltglm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uhwvyctg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lffaojix.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ligrxljj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ygafdsik.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2glsbikcn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2afqxmzbt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rnhjnhco.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2jqpaphkp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hpvxlhgf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2todcykfe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hhnsiqdh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hctfrtae.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gztjjeca.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bltcxwkz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2erqasysi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2apqmcdtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpbfusgv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nirmlcyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgoqzoym.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2nqlliycx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bvvcutrj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eykeriix.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2meqqwhoe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mrcorous.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ejhqhpfd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2uzxgsnzb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wcliwqyl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ikchclty.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2khxcushw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ekcasisy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xeagjozz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hukrivfp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mbngazfp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zyqjzlxu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2eqzykpdo.html


<!-- 参考信息 -->