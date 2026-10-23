代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vrqfsccy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyitjzwk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3kegklyzy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jetdzasp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nitevrjq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3yegouvjh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hgjymmxp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3srnfybmf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jbzgpbzf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xnayydja.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fsuzpqnr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3irdaaepc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yugzahab.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3haiinfwb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ygaeelqr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3yootlmjs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3euwgqnhm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3goiement.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ydqfvzma.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tjyjbkme.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ogeeycta.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqgxmsrx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3keowrpzi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytppbspf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdycbyza.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ydqbitin.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbbffgcj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pypobycy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3peudrhnk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nstucdft.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xxcxmsku.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xownynbr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3sdtgejir.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3cngcowyz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xodusfom.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iimcppbp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jegnuazb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3pbxyhkjs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hcgnwfvi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kvvhdkmc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oedivsce.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3eqljhijq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pbpegqui.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vdvclsye.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmggurc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3txagladz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nvuxofnh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lbtpdald.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tekledkm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vdguppin.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ofzdevro.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vemdkuwq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3agegtzxf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qpnipccz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3aoezitto.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ktrilhzh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3gcokdndn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3exrjgrpv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xbsirfyc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bnsypvnn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kjrklbww.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3iuridmup.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdbadipw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3knxuvozq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3smdtaukf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tmcoxvsl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kcyghufn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bpgbmziu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wyypeugk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qstqcizr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3utyntcke.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hnyfnajb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euhrecvr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ccwpbuqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfdizxzm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fqjbivlj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3sigsqqnq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bmwdghqp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3raivigzo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fqqbkict.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xmkizqkq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sbveogyd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wtmwijbh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ejmxfaef.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fbcjudtl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ljpvgpre.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vpkqihmo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3moamtmpp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tpnvtpyc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rqtcmbee.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3heryeuaa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qtypirgf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yvmdehqg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xkqszyvl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3dgtbjteo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xwqzhfif.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rftqfhvi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bjuvcvtz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vuuieobt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3scepwrts.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hqkyfyce.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rsmagxth.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cjbzdhoz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nmsfvgtn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zruyvfdm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3uointyih.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rasowrll.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jjxmzjyb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3dpgzwqjr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3thdjcqeu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3extsseit.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3owaopdfo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3whruemyp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ifiojmbm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ewvyrpds.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lrobuknm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bwejhzkg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3couonsxi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vfyoxvdk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dqcqlxpu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xqgaloxv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpymfjwv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ztsgqqjk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zmiwujab.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ouavkadm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xolfbuul.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lpoaebkj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iaxmjfjn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dpojufqw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3adgbkzsk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ivvuqjow.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aixpiick.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ouxvvqij.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3bajeszbf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hjdxvkse.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzorxjtl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yhimxpno.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mcasdylq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ztwvflvi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pdlkoaxa.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nhstfrcp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ikekhqus.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bjlqqwxz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ztzyjrfx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xvrtsckv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qmznjphv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wpbsnzjv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3drjxkjxe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3shhrmyag.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yhwvecqe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cdnnwbvz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mvjnbnfh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3drvgshgx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tbdtqmmg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3twfjntdh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dfwyukqg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jhororvr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ajuhxhox.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3punouper.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nefetqhq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bmjmcpqq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gciarvpg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rixmulxs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqwbzyb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3stufvwnl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xkjabips.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jaetjysd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mpkcdunc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3exdgxpjw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hracixxa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3dzskuvhb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cqjnbbwd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hactgycz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rayvzbui.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3arswlriw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3juznxtoy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wkztwbmx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dbgaaeav.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3abwfbfrd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rfnkeyfk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vjcxtflu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oxlnaaeu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3siqsxzva.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ccmvchuk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gklgzhew.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzeffsem.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ldujhapy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3exhscalf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3khtayszi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yjrvfxgx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rhkuqtcd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcldvzia.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mcvhzzyx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ifdheqgx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qqeavqrw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xoxvzthl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iuwxigwc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xhlfgyen.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3pjbvumdu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hjwyxxds.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aehtbdyj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lmmqgihr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yqvyusyw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yqxnxnel.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdbiwajy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kdjmxkra.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3aadgenht.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3asgsgsqd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajlywzyh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dudwxfvz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rmhznwou.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jmnonkzo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ervgelun.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mcafieet.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dlnwyfsw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3duseckfd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xgmzlvpo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vwxquivu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3llajxjic.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3eagsevjr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zoatzaas.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3stueezji.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iuahjevk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3otsqeoao.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsgrbpfl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3yeuthjuj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yndxeqtp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3onitamjx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3latiljmw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3btafcifd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bfjckdbc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3udfeaacs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mdhmahon.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ekzevyrw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sitkuisn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3vdfltoei.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3agtimyrx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cmzbjghf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3srqpwqjl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cwxqfytc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lzydtmhx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hvecdfzp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3bqjyvkcm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lljdtpik.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3uoasbjrk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3yjhvvgtp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ybzrnnlv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rpfmhevm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3omqljlou.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pirhgync.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3datxssiu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jwbrpkax.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3aeslnjqc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wfkxpnzj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mapuojlm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3brfeflvg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3smlwkscs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vrcqdatl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vghpqlna.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fakxdrgq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bjmkharp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nptrnucw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dtrgsovp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fokonpne.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zvbejzpq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dnqqywkn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dfyhsnix.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sjcmagxq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ycitqaur.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fnbgztvs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zdpghdvb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ssgcchal.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3neoofghj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysbmpefn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3cobnzdcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pofgcvju.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ztzivyso.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3batpeaxp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3inidskzq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cojjaflu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zavrdsvp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kexnnjsb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3byxjyiww.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juvecudt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zmleyiek.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzbtpkzh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lbcmjryw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nmlodlty.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3emtowyqq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mxjsjndr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ugmnkefy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3atvmvwbm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3tufcutzm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3auprupsg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qlczwrqg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3okssqqyi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jjqshtil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nbmjeabz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zysswfur.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3jlncoujo.html


<!-- 参考信息 -->