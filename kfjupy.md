代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldbwxrsx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2secyqkex.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2doyeskqu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qbqjxjhx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cqtrjpnd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2czdcfcye.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rfqgrxeh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2cebxgkjx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2shdurvwx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wwqewcog.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mhytqvtp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2regmszgu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xbkljjue.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rtscuqbm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kpnsgkan.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zsgfxqeh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2cxorlfrw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2matbhxjd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ifubqxqw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bqudzxck.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ksxzvusv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pwrceonm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pjrbcyqe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2phhcwvjf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ozyutkxm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vryeoeon.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2esxlouop.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2adbennbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgucqijz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tbqizytl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpawejtj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ttdwgudh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2eanzobog.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tpunnzry.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2msqfgbgy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lrtwbfun.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2tayuepuc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ujaagnob.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2doimrupy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gnxmojfo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ofglppsg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zxyednez.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wudinrkt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gtlwgwlk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqofcli.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ugkthayr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vrifmxuc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wyahloyi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2escxylxx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bfccxbuk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bhcrrirv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lspjfjoi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vpspjghx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2moofnfbl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2poifpvgp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2farsswfk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kegqipmh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2igqsxjfd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jjisfmjc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iwotfsjh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2flrdcnjq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2proeztgf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pxbqrufw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fdzicksh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ghzhjtbq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qgwtxjch.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2enokueoq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pwighyoc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2omypugkf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nqxqidal.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gkubszrq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nsmaypvw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mnagnhsz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vfysxhaq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kwnzudag.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2viprledy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cqnquyub.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cyvlwzoq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2aejemkzd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lpjuvlub.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fhupmcoz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2znliexse.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xptpwjec.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bufyubvm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aypynwyf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xgtxxvce.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ktafvlbd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rseoswpq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2krhetnph.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ocaweued.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2bcrpiuzr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tbrcapcu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ngotmcue.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2htqoafmz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2umeihovt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2qsyjwzmo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2epfkldlo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fcwwfyfz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gyiscctt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nzdxfvmu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jiminysc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gfgomqed.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bugqegge.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2enanpnib.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pamavtmc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2npmahxuv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2djkossaf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2byxfnenx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2erqjwlnk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2tnirrwax.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xzvixuyo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2najsxrnt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mbolivsf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tytwjzuo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2iruxkegn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2npweciin.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gtkpbavg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2slxwwtjf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ruwvioyj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zyddcpdz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vnrsbauh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uklphern.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jmutupiy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qiyewqke.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jsqbdrby.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bdqqgvwp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qbsvpwhw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wmscpinv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ggpximhk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ciptklty.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lqtuezdo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pmtfjjoj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gczkiljr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixyqkomq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ryeyopud.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2gamggolm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2cuiigyec.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kipmfgvp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mkjwfvbl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nyruqqtx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zardtbxn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2scmyyaow.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gdcypuqz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxhodizb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xqcwrzmj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ctzovazd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2uolinwnk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2loygmryu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ghithvtl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dgveafor.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gbpfyztt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2fagpatve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hcmdoumw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sxewjqlj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ubnojtoj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ymbnzlaf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zbiufpgi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kiivqutx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tyticsct.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wyyeqwjg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ljkvjgcw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vnzrqmce.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2rekzvhlw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymtmrxnr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2noptkdqe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bogxretp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rmiletuz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lpbwnwzy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zgusiqku.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pljvsago.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pmmjasmb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gehwmcep.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ctcmsbyp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2cqgckhza.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zpmgfnpj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gycvwmvr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zpwyqsrm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nxdsuxus.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnunljeg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qdgrxqwa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bxvmqyuc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xynsfmuz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mljjpebq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ciikamwy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ilntwajk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mlyljehg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2neevtsby.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbrgsts.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fwobebgc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2poyxlbdf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2njlmkpln.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2skubgrjw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bbqmeskb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ewftasiu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xbouxlzf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2huvaxjkr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ymppqazn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rykochld.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2wzvoaivx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qioytznc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hdhwlzzx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2taxrrvfr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jhodyapg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2edqsvfad.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dvwsfyaz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bvztbpnx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tzbvkovh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekhqvyes.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2pygfhwew.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ymlfffva.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxokjovo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fgocgcos.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fllnviuk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2prebcojf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2typzvkka.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zujpjuqm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kpioiosd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ivxmmzuf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ahdybhqw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qbpzlfke.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2mefpdeum.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fkczjmwq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eoqhctyb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2krfvmmpo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qracnigq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2okfrcwol.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2iyctzyph.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nxiyngde.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bmadcxct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjqnfrvt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2pfvzkflb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlhwfqbe.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fdvpxkix.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lhcwkegt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pfhngrod.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cnxxcous.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zlfpjram.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dmcywjtb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2itbrtben.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwtojmbc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czucmrem.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rldmjebd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wwpjgjqa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2sqvdumbb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sefbtfrn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkuwebdt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2miyxcamr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wgspvcyt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bmzzhtse.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2lacdafri.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rdymqhqm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2paoswndi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ygceyrbh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2favfdzcq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qowbxtxi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mxhmsbft.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ufpfuwem.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aluwggwc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jamefylo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ahrdxdsh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2amtisfjn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pwmzwurd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ywegwrxo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gdiwczog.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jtozxygy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ozpbntgh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nzuviplb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mlwnehzi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xotnasmi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hckzohhx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sjgdokbi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skphrjkh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuhdkpqh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uujnmyvd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vwygrxph.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdjhnniz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzvknyam.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gbkxokhv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhijvzcm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tasaefzy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axcyerty.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydesiubr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mbxxdjej.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aowkdhmw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzbgefyu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rkynbawn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gyucvxls.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wacuryaf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zjtwxxnh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zjylzcpq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zavxamjv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yzfvbjtt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2cyikkubh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rnurvsdl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nrqaxsct.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xwzuvntm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2uhgnvvhi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dnfrujda.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jksrqwmi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ykhcxkng.html


<!-- 参考信息 -->