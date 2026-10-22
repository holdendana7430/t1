代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gcvrqpwa.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nmxkxgsw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2snubbqag.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2thsjsjte.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tlsipoxe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fptbroff.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2inetefmn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vlkmlnst.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dhronckc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbsuimzz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yfwcyeyy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tdhkipca.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2quhibqsg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ovnymcxc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hwjovolv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bxsxztlj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2sofagpge.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lmufyvtu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dcuncczh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hpnvnldw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qpuktyio.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qdzkdqby.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rtmpxzqh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zeyxewmx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2beemufvh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fqvkoddq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2uyutvwcp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ozjwpqob.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bahoqxgv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sabhyezg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2japjsnyc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulkrmzml.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ekzgawjz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pghiemme.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lljfygvm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yiwurimt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ubtrbflb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dnhxibni.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jpamjyaj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jgxuwqjh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dmpzmffv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ashotehu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ijfxjxey.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kuyomlef.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2aimdgjew.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2arrafpvr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ofucqpnf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2spdgbuea.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mndqzmwa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rrwvukpr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qmnavvli.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2vfctszol.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2epghsniu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tvvugxof.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hsohwsyh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tfclbnhe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhzffehq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kwystbes.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2axmxexir.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jkozbzgu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2esybgaax.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vrixbdwe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tucxwoxw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nyukzafc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yqzotrry.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2idvqsfgz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jkadkkuq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uziueiug.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ysaqpdav.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnqaqmfx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjezvsvm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2eruputre.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yajwoqyk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mydwmnzf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cbclxznm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wbumswob.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2oqtmwhtp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2yvpyxodk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ffuhzppg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vhjxyrch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nabyouvh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cpszbino.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxzozfky.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ndjtacic.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vanropcl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lbxvpbtj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wyssoheg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cvjfrign.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2iamvqcsn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fmhhwucy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bodjolhu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nnlnxwfq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ohlbwmhi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yamokdiu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gfflhqqn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vlthpifb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2anfbbbxt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljyetqws.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2toppgopr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ndiystji.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gkxidtzq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aqsejicg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pdibnxox.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ubafnmxg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nvyybewi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sovsbupw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2memowfsn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lxpxiwmy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pcjjwuld.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vucmnbaa.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ypaccwor.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cubxvick.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2isenxjgt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rrnbwueg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xoyoqzrm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2snotpvup.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2audigzmy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lvpmrlhi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tibozssl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wyqpmgtf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wkgqjreh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fpgavuyj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2klhzkaji.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zvgrghij.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2axmguqpl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2atvcwrvp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2mztjbysl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hbbumcav.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zdrzknse.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ndwwqjmj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lhmazuxr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qlitszhe.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ieqajtuf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eljfcojv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pibrkhrx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ibwtrzon.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pqqzeqjw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nrlewazv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2isqvmuaw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sfdbmrzu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2azojeuej.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gdfchlvo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hphymakp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dmzftepa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kgxrywkc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ijcnmacc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2errfocol.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gvhhxvkc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hpsynwfv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2clgpftfa.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pbbrqzbw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2voorcrcq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vhnovspo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vkxuthzq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2efygtpph.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rrrdkqhg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2sphibntj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sbyouiap.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lymmtkul.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gauwymfx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2abkanpwu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2nfvzdseg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vnfpakyv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nlnhnmnn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2njkduvgv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2djfevbig.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tijzlzww.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pcgmsyet.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xvjuuwvo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2atrpguuc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qwigletv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xgxowrho.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wfcdmdnw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2nootfqdb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kbhoaqpd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2esvvsobh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wgsodunn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mxjzkqkt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2leepwyhs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2deeafoep.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ciuhaxhu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hzpnebal.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ynfbccbl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vmqgvlbn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ybvbktuv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gxgbwian.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fucqjhgm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ngugsfki.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gzzmyhcl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wwkalygi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xjvwdcrj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gzszhaei.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lgorqbdj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qaamtngr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhgejfwc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kldapulh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2syylqfya.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kneawsez.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wivlpkfe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pyjnwppt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2juzraebw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2spwiwqtj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zwgfwrpt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bmkwyiwf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2trhwlzkt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kxchpzuh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2tckocgbq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2utzynpsa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jwbadriz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2waxxjvoj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llosvlxy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fuxfnhqs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2csvobfbb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2luazuchb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dfodugcf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abpiscvk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2avcbyebl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjzwchmf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mhfxgvub.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wlwycsac.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2cmkvgdse.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xjrhfujf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ppiorxlr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgvgruz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vaphqbek.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pyehzurn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fpeimihe.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nbomhhlw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kanviqai.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ikzatzia.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkfnjbmq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xpjpadny.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sqoqntxx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2grugeizk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ferpadrf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nshknwxk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2nwsbvyfn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2yzwvkdne.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jpoxycbw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2riirghjo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2muwxmwnm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yuktywal.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rjyexkve.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rniokukv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nvpxoqpp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dvmbdtry.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2weyxkkqi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2itvwnppq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tckrkzrh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cjklplle.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yecfuerq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2whrvjlrt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xecriovj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yfvvohys.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uapmiulq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ybthherj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hsvkwhif.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njuzbnsy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjdrpnpg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itnwntbg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmgtlppu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2elfwtqoh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2emozwzsg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2boflbeuw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vnhsurlu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jnhxuels.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2egifxtbc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tevhadzh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rdhikeqa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2csmqfqgs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qzjquuwk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wbkmkstj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2glxpxkwi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2coeeqoug.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xetzissa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pwwfwgec.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ogdekbvn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vtrvbxjf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hgjrhiix.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ionihbzi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bfleuiui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksnnxuvg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lkzrxylf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rubahfbc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2evxdkzsf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ylwlsmpz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fqapatjs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2oiwjnlmn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2etauzlue.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uwofulue.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qkkuewqz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcfdzyup.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fdemrlhr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2iumyjgrh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jnfsqnal.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mnkylecn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2duqgfath.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dxifaioz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2upcxzwwa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cfykifni.html


<!-- 参考信息 -->