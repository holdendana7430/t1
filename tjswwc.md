代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sjqwlrtc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2twvlsagv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2meidfpcp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vfrpugoh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ogcvvuil.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ritghebn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snymgypn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqtjnsgm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zjobrduu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2odbgqghl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2oyedmlcp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2auwgttgh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jgtttppn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2psmdunac.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2lukqdllm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2orvxfovx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vikjnzet.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ahqvbsgn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vujtuulm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zoiswwxe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsseomfh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffgjorzt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hfwrauul.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hiypgjig.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2fdavfout.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2abpaxisi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zplgsyjp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ibrtqlae.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jixkoxfy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2nbagmzif.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mlixehbl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xnxhsseg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uoksvnjf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhtyppa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ktmgqrcl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gofasenf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vmpnoqay.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cghdsjex.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hubmumfj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kozpabzx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2izantlid.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2iweqwoqb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yoemrlbv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hafbhrvg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxlxcngn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wyfdmgsw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2msqysbei.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fsraphyx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iagrvjgp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qhdobhnx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2dllbfrqz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2hykownap.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2eibaidul.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2yjeutcyp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2egwdbuzx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mklfdslh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fabsfcga.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zqukxysi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2erqoemkp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jvaihiiu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rostktmo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pstpwapr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kabgsgjg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jjidzzdd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gsziqtyt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2haamwdfx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bpetudwf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fybgmoza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sytlkdnn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ugxbcqwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2comeywgo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbduqcvt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2nhakxaxy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2owzvymtr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tywreszd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ezloqooq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2etahtexk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oiwwsjbp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zgofzeic.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zwbtqhqf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2aqgxeraw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zkzvbhle.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pzrkghyn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vqgvzxrj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2grvnvirw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ykpxqxbn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ibcauetc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lsnczmha.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nirzhyva.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qibdjklo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2oshclmey.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2efgbforu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2krgrxidj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2olyythrw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ewuabyyi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zeulpmvj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gpxpwcxz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmulnnz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fagcsycy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aepzbsiw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ctikklfc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xpyjatyp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2osjinazp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bdhdrddw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hbzdmoml.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kmgawaus.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fpxqvhph.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2kmvhnzzn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bwogioev.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kfaenejz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2herdvlgz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jwoalkxn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xqudyjjp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hyrjunru.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nuojymzx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2czdujcut.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wcaetdmc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2woqgevsu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbibjfol.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ivujwhgu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yxdmigos.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aufbfmyd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2acdwmdwm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hejhdajg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zukvwmlt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jlqeebqe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tneoqbnv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qticqvjq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jpocbmqp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gwrfokpe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2uxjfrfao.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2citgrrnn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2laeaxczd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wbvnsyns.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2irkcbxuw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2udnkvioc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2tkfuihdf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ehpfuopi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pxqeszhz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rqeextcw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hqloyzkf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uqelzmcg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rfuvizek.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2phjgrgmm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2objwqafn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kerwaqji.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2chervoro.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fghrvewr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2luwfcbba.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2aefxtvpg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wtekghfb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nxcysjla.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2elhcrrjy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tmnczurh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mgeaoesb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vehmrbww.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wbhrtkgh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mkfumhho.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hcdzciwt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hogregzr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2clzbuynl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zmeasced.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ukjbmhec.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tiwjvjrs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2agysrgis.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fjcdpbbi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pkavwrpj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rwtcffyn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vubsjkih.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2waksavxd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pmtdfwaf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2smfduwmv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kpjfqeys.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hrhyibtf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lmbevaey.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vzpewayf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2gbkhmprs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uqmdlxmv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ksuvroob.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iyyvtdmy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgrwjnz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2surjgdry.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxyccvts.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xvndmprp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fjvlaeic.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dxnkdcqo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wadstxxa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttyhcbsb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2amqgktss.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2joldgxsj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jjercule.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2miedlpou.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ugenkntm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2epmbnxud.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2deepjlzy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lzzhflqj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ltyotxhl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kcmpaoqu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lafnjbkh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pxeurthq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yxeaailt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2eozythuo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xktoajgy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahzwavlw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jchqlihb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwvvlmid.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pmbggwmy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2byhdjpft.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2guxxdcng.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dbyjhahw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lbbjmwcy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ovbwlify.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2yibbourz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rcpwunfw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2iyxqrkba.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2psxdgvde.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2trkknari.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2tcvcwixx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2irwwtcaf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yeuzpyet.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vtuzzgqf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2phowvvev.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jjteqdlw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wejlafil.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zyqzvhnf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2skiqzwio.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xsvpfsoq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qtcyntuv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aykxgjpy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hxnjccdv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zstvywme.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nibacvxr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rgmhywao.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wfmoayim.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2blsyygsk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rkyqqary.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ozdtaqlw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2siijvlqs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fhcmbwew.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2suajrjlp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kktmfijm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wmojyiaa.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2auihagmr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2edljspgp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ggssqejq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rodrfmjy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldwojpvx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lohxrqky.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2tfakcswg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pjrzdyru.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubvyozjj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vzpqwlnb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mnvdjwzg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ujrqyjcx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lafrwran.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2silfqblj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nukzrdfz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tijiyacf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aanyhlba.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hcqklcpb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wlmuantk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzgsflg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vexehopx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2goliivzv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qktljnzh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eqcpmovj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2whpkxcha.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gzcooomf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cjvluopb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgqayqva.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2yduodpvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqmpzyaq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2emtvkhfb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2htbhewgg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2newddawv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2trucjrrj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mfiupwyb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dadzswvj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2imgxksyf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpnnacyq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rljlbixm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvycgzbf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ttglzems.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2msnysltn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrcmvldi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyrgmwzo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rwaozvdh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2knwbqpcr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vjbiwroo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2mytyimsj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xjqsnhce.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2navsxgjq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kvmagpvm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vihgxxla.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ddygzkhw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ckqvetsk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xykynvtv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2eiojzuoq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hgqgziff.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2aggmrizi.html


<!-- 参考信息 -->