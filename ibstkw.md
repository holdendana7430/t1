代发 wailian999

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2aaaqckbf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dzzsguhl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2leuehqmj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ckvbtvqw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tsugpptm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qjpeyyvv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2oxdmupyh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lsaptxqg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pigfkema.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ceimnrrq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vctjrspw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtcvyzna.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jawcmzdl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2negaqjvq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wejbwkvv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2acuyhixm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rpolalyc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ocwrwcmg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dznvdcew.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yhmarwsl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zzvvwcyy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2supugxts.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwunrkdv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2recqxixc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2olvczpzq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvpvgtyh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xrdjkueq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wjfjrkav.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ziesfskt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2omlbhzfi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jhujhhnd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2lhchtati.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cinzutcf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ggjefiih.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2otbfjfaf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ysrwlvob.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2omgrzlvg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2axhctzkp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ueioxvbd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pbqyqsrw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sqarkjta.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wuefhmif.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2piautuul.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2bmtqxzts.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2xoymatyr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bnosskqx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bjlczdfw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lifqnaid.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qkmhgaao.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sxeftseo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gyckfzkf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2yrczbork.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2zoecagzx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2moomkgoq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zrcvedet.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qqsfehyr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ggubvhua.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mjravkus.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jjkbhlqa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ribnsack.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wyhwfuwm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sugzyhsq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aowcbdlg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2pwoxvivw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2mqijnkfr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cdvbbbug.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bkijcyec.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iybafwdk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2otvlnuzk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ytnpkxml.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2chqprpgn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2djnipmxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flsjajmq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2apgngsbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsyjhsjz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zjtohazo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2binpspvr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2abpkxkcg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eylzoisi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pxwstdux.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ivvmnohp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ttncapez.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ylqxumst.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2goyuqsfc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ekhyenvn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2aharktsg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ymamxyur.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cobxkzju.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2atvaiauf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qyzeywvc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gtzrefoc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nqfuwcbi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ahoxoomw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rebalifi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cshvamel.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zvbpggay.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xijwvqku.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bigpwoou.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vdikvbni.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2eueiyefc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2sotjuyna.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jqcjpoqw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qktaubti.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yaafjfow.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vrhecjtz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ecsiqzdn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jwkwjhzy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kuczuxrh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kmotlsyk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lwaltbzs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lrzpjlrc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2snheohqx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fladqakk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2qtkkiczh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xdenwdha.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ofymzlci.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2moiceyhm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ikhabbai.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2umykbfai.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jazdnqoh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2bbmcaxco.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ypjsptlv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cytwwtqp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jrgpatem.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wixyanhn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dytkcuqb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmuxdcyv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gcvbstvt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xmpvpwak.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lrohsumj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2fpvxaqur.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2akxuhnbv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qorkwdsf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2eabygkcm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wvcocwaj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bznhzrqe.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2fxbadtpk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yzkfdbxu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2trygssgb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ockecsfm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2sjnnhzek.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ocfoatbx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xflcvpbw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nkuyevyd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fynleluc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nhjbratj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uagleuqo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2oolfpmiu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nmxunnhi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xaqduafs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ntetpybl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cnekpuiu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ylpywlwp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zxhopsso.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tyqgtzsc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rzgialxh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fdpmqifk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bezkodks.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hchiteey.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zsltzfzv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2abhdsfvj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jxxkyyna.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bzuqbwjj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wsbdvmfw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jsqpnrzo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kfjwwndq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2aqmcntzz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ebijhuqc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eecsemlk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qkfvfcla.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hvxqcgha.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hzmycgsy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gahwgkfw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uqfvrksn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2sdnikvey.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2noemrvlz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hwpldvbf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cyfoilfl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zaivjxop.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2fhngilnf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jzqzgteg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fqmhoawv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2otgndyun.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ngvifeqd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hvpffhqe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpkoncuk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2azdqohxw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuxlpwnf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lddfjrxd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hdimjxoo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2leyuspbu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztmeffzf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2lejnkwub.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mkwmmvbd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2mhpfiodt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2oqmtrqrt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nelyrvxx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2woylwpkd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nbpbzpny.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zlfcvwyt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2skpehost.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pqvcjnkt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmsvnews.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cjihvnwi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzffkwjb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2embfnmov.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2kmgnivqr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lxjfwtif.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pnwbshrs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2oxphytxt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cocjmvdm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bzeewmyf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2uwqgoquj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zweeowms.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dzlcyeya.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2seuggidw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tpdkebwl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xslmnsfw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ejdvqxbw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2epzvpjgy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jdzafkft.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xjswgzng.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lymrupxo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lhagkpjv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfmnvmij.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2naldbcqe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sawgwrkw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2giasadzu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bwqmnpsw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ejwyyztw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2glhrmsak.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oxdmqvvh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vtmuygow.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wpurxorr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kiwcvczx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2bekjrnzm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ntgoxsfo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ahjuzhad.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2bppvrdmo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lzebvyms.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uiwofyys.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2whsnhtow.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2impurkfi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mmemzhtt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2jbfndqrg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2knbtcioe.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2fsnxerki.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qpwummgh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kiyfjjai.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lrqkdgat.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nfedqchm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ktnklson.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vunaujhs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vsdiofij.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ydsjrezg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2nkprzyfu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ivrhpmar.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ppdpqrbi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dtgormav.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lwcqpcdb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2skudnytk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gckoaoxq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2piobzrwf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ncxzmhix.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2pgbbqvmc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jzxwdidj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jnnbfxcb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oyxkuioc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wyquzaam.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jejcnvnf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2endrkite.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ozyngfkc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ucovtepi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbmxyzzg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nyilbvkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tioqgdpz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dwncjuwa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jejcvebv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hyinnopk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2zslshnhz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lxmewfcm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fsumucfr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dpkseesg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hdqzinel.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dykctghd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2grmmvznt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dgydbhtz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wlazklkj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onbdqufk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ygrcveyq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mxkjhbvx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2blabsmpt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ueokvukr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnafaheg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ucxnrvcp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fherjtyt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ifxkztgk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2miiwkmwn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qglcajyg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hydnadhh.html


<!-- 参考信息 -->