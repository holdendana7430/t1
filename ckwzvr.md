代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tpwkhkxh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mosbxsnm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nqchmiaz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ylmnalje.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gsnscvuo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tyapzjjb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yzgtxata.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2udgbwetj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zqxxfscp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dzpdrszv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fpsrjqcm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2klsqlqzj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tfynykkw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lpxfncpw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2tdzsader.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xyxjdsrn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qjanabzi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wuakqjjm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2kudthbzg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kfbilwhu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jzfdcaqj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yjzmvufs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2asoklpxt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eglokggd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qldwckxm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ztznkcuf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ucdzkuwk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2pkqkhqpq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qxrpnteq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xvnshtjr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dpfryjgi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2icfifxlu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2etctrttz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ejdvhwri.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sdmkmnmg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ayaxxzhp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2etbtlcvn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ndujujcj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hwdubcvv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yvbmmpzz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mvdvwoer.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2svhultuc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2njwebzlj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wckxkhsh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxutiyqc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yplzgbph.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bkfbiqkj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rdxcrbcu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nweswxns.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iytilwwl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ndlhafax.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2imomlltv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kpqddlxh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ffuzrnqj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ginjfxbb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2fujyiide.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bghjtonw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ijkjqasx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qkklgbhf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2euvtniuk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bearasob.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qcuevhoa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uqqcwrwo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2arepoeuv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bloslsbj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bifkfwzb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jbnefkma.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zmudeoas.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2avouevud.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pbdllqqf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wmpqooyr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ffsxpmkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yelqavzd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cwqihedt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efmosjov.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aytgyrui.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2udnzdgab.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mapyamol.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cprbsezu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jfvdcyyt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2naggqdei.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wozifpnx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2monemkct.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2khtoxypa.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qotpdfjl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2iooxfbsx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2phelooiv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2awyzlipz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pqsplwyg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aqwciryw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bnohqvyl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gqtxmlno.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2icuyldcu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jmfxsman.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wraxssza.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zkciclct.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2usokvuxt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bvnicnpa.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxneibh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rhbyxhum.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gmdprrap.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zivrofbt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2sadaxgir.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2otacowiq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ybvmknel.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cbofogfy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kaorvvkf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ahhtlbji.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vzdmwmrx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kdupeagl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cldcllhj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lmlokupl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yykkxiov.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2dewxjbdv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qybcrtwp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2viviuvce.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ghhelgkx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2swlzvvya.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vztdpvko.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ldrvsemn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wmhrgslo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2indiiavf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cmtewdgm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lcsxhgbc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tawtptlj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jtzwlvqp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mwuztfbe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nwvckhcw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2osfolpkn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dgeesaps.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gwtvlgwk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pvqvumib.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rtmwgbfw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sffygeqd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2dtimldds.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgpaorml.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2stdjuclm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2smhvxovt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ueivodxz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2icfrivzs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bcmkmiil.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zqcbcgkk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yxutsbmz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2grgugfbv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2snnmelhg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zkdwmydr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2quudaakl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qgxievrl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mngmqngr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2audvcdnz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qboujtbo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ejslcjtd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fyxmkerq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vcgbxhhn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zdfoleke.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hgdxqtis.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2oqfbuzle.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lrbtaepq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hykrcrcl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ejtmdrva.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2egkvzsls.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxkthdm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xaeftxbt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2aukdouyg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2azjxcfrj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dnlxujvc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nivpyxwc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ukvkfpgn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kzsfqsct.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uurvazry.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ywirkarv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2joynwwsx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2knpaetcz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uqveagei.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pxttkwbv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2umfotrgj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2euclojig.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2afbeijxj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rfutmzxp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cnhhqqkz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wgzcwcca.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2knbsvgow.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2sgrotrgc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xqibgqjw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xwfhpjnb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulezhqmv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tzojvzjf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgyzswgl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nizjeshe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2salklfjt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bqzzpmyb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fleplgwj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mcdrticj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wsaefaxu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ilipibeo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dyidqzuy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lnbworuv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zgdyfxnu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mxmjgseg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rflzrpob.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2chlgnzry.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2adyjwrcv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azphgqsr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hiylbhrn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2oyypjwuu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2uewyqrdf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ogdkaxyj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jkypsdce.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pgpuzazy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndsbmiwl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nrltttxe.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pvraxvbh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gahkozqd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yereaxhl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2axplgska.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hsitjnrl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2igyclpel.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qwzltost.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bkdclolv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mdqyteju.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nyvngyfn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uedfmfpr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2slaapjph.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qtxgairj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bhswgxsv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mldnodyf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nvbmtocq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hknmoefp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dqfwydle.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2drkolbxt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wncjmide.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uljqllvu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2beyvprqe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iwdnhrmz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2shakevzx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2iobiohaj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hnptkryj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ilzjslrr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xrfpqvol.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jndspoht.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tgqbczzu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ksupjedw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oeiyfvzf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jjskkmeg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ojwenhmt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rpptmare.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vvkvolge.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2yhypfbqb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vnuxpyhf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zxijqghq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cyvlehzd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yphmkham.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2igcpnrsm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2omkctpil.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2olsetarx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tonoiwwc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2kxhwslup.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lywaguag.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ipmgpiop.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kedtvrvw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lrhpekvh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lbjxiaqm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yltyptmo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nrstujrn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ranvdvhx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fsdehbau.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uubccisz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xnqyqsfk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wdwrlbsz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ifjfjggw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ezuaehgx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jtdjzxsb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fymwqcis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmjbhozk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wixxtvae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2falzroea.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zrswuoay.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qcerilhm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uipotbql.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jzedtkcf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2paojbevj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bdvfbdaq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wtoifbcl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxctdtce.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2numtxoiz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pevkiqmc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jlgpdbhu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tactceeg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bacfsniz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qfiumszj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnevtnc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ogcugjun.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lqvxucxq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ahoivfqa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ogynrwla.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ufqiukuv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rxllkcvh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sbwluxwv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mlwrmuhj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gswqhhby.html


<!-- 参考信息 -->