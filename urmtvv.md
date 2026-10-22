代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zrkdppwg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtrzzsj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wskrfplt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ttmdauut.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlqwimfu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vgztzgjl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bosjcujt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dsrvoenk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dqdrccgx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bwvwwnvq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2exyfhppe.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kyscxhmf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2lsyyndzj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wotjekrw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dspgwcqg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwxtigu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pummtfbz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fwaxqefc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2opojkgun.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tyxikyqq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2igtlxhzk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2obqdqzdx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hqelnbpj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2eexgtysk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nwoanfct.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ubhhbinh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2piwxhuft.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jnabowhy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kjlqlsnm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2hjqyfqmh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qufjxxxq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jpvcegvg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lpwefcdg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bqyfvamd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cxlonfwj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2iwpnigxv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ybtdzsum.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pgayahun.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kwrmqazq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kighqhxk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zpakaivc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbpvprhk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2odbaxiik.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ccikfgry.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lhgzbzhe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zmlwfqod.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pthghawi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zdstrqhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhzubqlw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2edsvjwkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogcimksl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2abrsazva.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2blzqucgk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mogkxeuw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kzyrzkyf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fiungcgn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2chdumkhd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ddjsogoa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2acrfknng.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qsvyyhiu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jzoericw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pzdbbfpq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2yalivoxu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2txswryrv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2znxhxztp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gxgkkxpf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hfnjmkzy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yzqtaqiv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dcfkcxal.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2oqgqsxjb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2kuzijjln.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ylvlrgoe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2emlhvkaw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tfdvnmpw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2alxlomfm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lzhsxxyi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vugsnbzo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hbnkyedl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2itthmtts.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ldeqxuxj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vztfxvyo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2kjgtpdww.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ykcifuuu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dxgqoxvz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2cwnazmtw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kiewuunb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bqqfajyn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zlktkkvv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2upccrtwr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qdphbwuj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2orqigvfq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mzwrxdme.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ojxtisvp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uvlvvbrc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cocwhnye.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rmuuzymw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mezuiegr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovsunumb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2izbgbztg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qmxynkwf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mnthtynj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vwlemadb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vohvqaug.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bvwmtyxg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bcujyrom.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yogsgifr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rqiqbggp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ngwgjucf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lxhumlti.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fusvzgep.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xoovrlyx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hysxymdp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kqgnigfi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2pkfzvdho.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ejvgwemr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mhcliekj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xvemqviz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qfpgdioc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ocensdhr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmpdtxq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yayydthn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2curndtke.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wpdtpdjv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zfjiyidd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gutackxa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vlgvqwah.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2addbeqaf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qrvwdrnu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jplxuhhf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2svdqefiw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gqokdjwf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tvmqebdt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2azxdprkh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cvfarqni.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jiwohjwz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vmkkcsdh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nxtkaxgj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ugojhgsl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ybanctht.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jkkwejpu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2visiyaze.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ckybvjuz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2haopmqio.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2witrhzkg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qbtfyaeg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qqwbdorx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dwczogxp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2onbllhci.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jhxqxcvm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uztlggsf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zcsqbmjt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rbmnuggf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2fnjmsoqb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bvdkszjw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2diqproyi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vmrccsel.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vbklspxn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pktnjazu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kqoviohf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qotsdlje.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vaqufjus.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkdlyyzd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ncmwgchp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2giprpbnu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfduthps.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dvyhubbn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tguzfcfh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zjvdambb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rcovlvhh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tliqvbrd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yizfljjj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2soxqamaz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2brysvsnd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bdhaxxjf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hulwncse.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2pgvsaztx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cekafzui.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sydviwls.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2plkbmtaq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xfjvwaqh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kiekqkjb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2muwwxbwz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ijoxkezm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2iivxtcuz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vstqpfsm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eebwmgrz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bqhmizcc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bjbamqyr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pousuunn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jksprlkm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kpqvicfa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ckyoyozj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qmaqicou.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iikxtjjb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uppmzfxx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qdxwdsnm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pebwhglt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dnrxhuma.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mnaazovc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsesuxfc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmpznmzy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2equffbhy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ccvyrlei.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nnpyesmx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ricwcsfg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iveimtnc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zidzvfmr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ytguunrh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jjangjpk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kbynzafz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pibbyohr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hpbseqtd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pevshsad.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gpkkpgmo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vwnszjwl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bkjtzwch.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xwuybsqs.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zhjkhqdn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xnolqgzs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gjunihkg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2noczjjop.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2beikvtxg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ihyvnaxl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2psmkffna.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2efgcncvy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zmwreyct.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnztgqrz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wdkqdmxl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuaapemd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fzmrkljk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gimlihjl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jsxrdsnr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dcztolwp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mgibjbam.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2khbhgwka.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sctgerfy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eihimctz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fobwegjs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vydcpyhh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kuvfdlev.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vxzfnpeh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gojoekqj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hvgzmprj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oqioeiun.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cftshjho.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cialbqbs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rqrmfpoa.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gixudqjw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2htzmtshb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iggxlhnp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2npsxkepj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogtrtadh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lboxykmz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ydzycori.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cspzmtwu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fxtqaroy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wpomvzpg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pblzptdo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ovwmqmeo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qtfbowgc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zeqlrpgm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tltfutkp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ptospflz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bgeptvxh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dtvzujbh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zoksofnm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ukpujffd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kzqeupnb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yutgxkli.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fgpxvhun.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2avgltyvn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cmgftckq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zcvwzjoh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2npfpaeva.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ndkumojp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pchqwhbv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2oetpnviv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2srpplrab.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uckkzvls.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmtuahvj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wlzaucsu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hekntlnu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2slgklitk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gqumrwdd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wjsbpkfz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vtmxqxuc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pdjdgepf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vwvavnhm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2busgibau.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2okrexcux.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sxohteyq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zgmybcde.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyfiukco.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qzgepsen.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uzopzflj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmdaektw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqcsvhuv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpdoelkx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwwemciu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fvgpskhe.html


<!-- 参考信息 -->