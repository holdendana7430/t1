代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2unpkklkq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sczabebu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2frniptml.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cnbfsdlr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yogasyuk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pgtrsbpd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qgrrguaj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hrqvrfem.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gioeyymf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2cnyhobmf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ymrodwrp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gvfyyrdc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ushrfluu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2osykdrya.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bioshoyq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jpzahpxe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zqfjrghh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2srhchwvn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ndqqislr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2twijtzjv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ifxltdxp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vmrbdavc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vprzapgh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2doojvhmc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dfwcrvzc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2khjjliqt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iazsxbtt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hrfolynf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpmiangm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lffbthga.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ajcwkpno.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2oeqtnxha.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kteyogjd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2gbnbvtqw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qncddace.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ginbykwo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2euhwqscv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqiujru.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bonoiygn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dxkgdqka.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xclhbzzp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2zaeezvla.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zgtgzkne.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fvwzwkmj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dqefakkd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2sfjctqdb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2idywglal.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lavwigjd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lbshjymx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qhvtfsca.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tjbsktuw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tvgwmici.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxyehnvm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bductuif.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2edlmieip.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hjqehbpw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fqrsbqqv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kvdyxpvq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2uobolpww.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jwsgccsy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ruohboyy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gixxnoda.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2usekweqw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xbtjebve.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zugakovd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqssbfob.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2njjonjti.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bdnizhkw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lmonushd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kahxgzgs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mvoozvui.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kbohomnk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jypfjiit.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nkepycfa.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iaansilb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dbdnirle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mernfcan.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2apniyvnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esjexcks.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vdtyibih.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nxcjwdlc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yrrxygep.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pbhzedmi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2leuqgqgo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ixygdfkh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nxmrsolu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zzcwoacr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iktiafwk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nnwctrkx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lygcgscu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xrfbdjta.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pzzpxifp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2eqnaihhs.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jxhthbaj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xeplzacp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gfldlhes.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mpvktyif.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fkvltxei.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jxlvakzg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pabyyxue.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2baeqrhmu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhhxseq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yuunflha.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wqpmtfta.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2arkuwwxe.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zetvwzpg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dybazars.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ctygohzt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2nozfriot.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ngbxhogo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ditiothx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dmedvekw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gaicvaeg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cmeggpok.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jonyzpdj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2tssrwxhd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ezjaggqd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zofhkalv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bwvczyux.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2elcjhvtz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pnyqxnkj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jpvgrhho.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bccxppxm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ycmlberv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2msjfktej.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sbktyehj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gkdqaspc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sqafkegw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fdkbsunj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rfbyxgtl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zsnjyxka.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ihsxcihr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fgqzttxt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ftwbpjjx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2boodsozt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fcsedddi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2sfqrdlec.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mruvdaud.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2itoddpqc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eiiexpsn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pbantnlr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wlndbwwu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tlvbyrmt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jgpujoia.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2oypynxvn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pzqwjkey.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2afershes.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2swjtppcd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cycpoxrv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ifdjcscp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2igeuzvcp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vgbsbfzx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pxocvneb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ywuczqdr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cqpgznju.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dsizavlh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2spftviky.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2siaaiuje.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fgtsjlpy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uvaqdzrz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fvntgrxr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zzhrfkzi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ewtzmvtw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rkmumukv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dhcqfyom.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wvxkzvqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tpvsyrcq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2immbkcjj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rdbpyzcg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2trvkrnzn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sgsijzlk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zazzcpcf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xpsbjgxi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tsnncosl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lcssutfr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hyclgjth.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dzxxbrcu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wqmuvigv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2tinoadnf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2btojxkfw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2roxvqhdn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oddhvfiw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2iqiafuta.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ihvcftoa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2dgvumhxs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2boewixut.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cenqvvqa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wrteyprf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vbkqidst.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2eabymweh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qenaureh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhneeki.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2edkejpkj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fdgffwqm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nxxlsmie.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljmqtmcm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zddwrwrj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ewosrvtv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2itowhdro.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2hihdhtyy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wuoeggbq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zszkymlu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2klarxwzq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hgbzyond.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vxjniztb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2onjvpxxl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqvidfkk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bmklnswb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2fygrllos.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xhzgborn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2owloeien.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzppwpge.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2juvowprx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmjqecao.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ghzdbxsj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tiyukcsm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zbxcimti.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tfqkjzbc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qckvmzxw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xperbilg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zcumziww.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2sbdzxqgd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ijvtkorn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nhrnpztd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wucaxzfv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hoyjctyz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ukeqnyup.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpswcegr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wozjbvsw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ihdattiq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2egnbfxpp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xcrkcdts.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xfkhghaq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2uhskgvoo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2hyuzcggx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xqoejcjn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qjyuwkfh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2myukbpbc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mtiuybnr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dlsmrnuh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2blnvlkvl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wggrhvgf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2dilmgllb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xuzqrqrj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2juydhhwj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lojqilzu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2svyhntex.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2komwiqfq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2eapurtom.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dnjzmbkm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ssvlrhaa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2sobshxlg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2cpfuoezf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqggxlha.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxeupeyz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hgzrawzf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlyezyko.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nsezlcaa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqpdwdvb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2pjzrchnw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2slqtkyia.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bnptgalc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2afigvbxk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xkoicqtn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2punvymys.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mdbvwtvq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2csdpdcvo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oswxqtcd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kxnsvhpg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qsufllrc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cjznkfgv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qkbyujkk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tycdzyth.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bsfbccfl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ttvexnpt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ugriqsas.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2awbpbrde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auicvagk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tkeqjbbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzqibdne.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2slbxuxhb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bkaqqpfy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jcqbfcsh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qxflbpcn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2esxudstl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mdyrrrdr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hvkmknpe.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbcnmaxe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tdrdxqhl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xczqwbzs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2igsxnfig.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiebibeg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pxuvzxod.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2shzzlylu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qnpuwjhb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wcfnkzcj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ntdspxhp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2seznpfqn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2sqdtdkbk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fxxqsftj.html


<!-- 参考信息 -->