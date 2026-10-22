代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wnceopbn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ujaotrtj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ukdewbob.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wkaaaaim.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dloeuhuk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldxymucj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tawpkwel.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2azamytbi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ycuagzow.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvnwyeim.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hqfrtqtu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hndockmt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vsnzqpbg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2curebapk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ggznyfev.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2chhjswyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qaihcpqb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gcgqwioa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcyofzop.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iojnbwot.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ieoprina.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nrpdpdgj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bloyciev.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jxxmdkse.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rncvuucq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bcfwryln.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2buqigesh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2exkalrbn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2irvvtmtd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ybonjxvk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2samjgwhu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2plyldxsf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qucrcomy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eillmfwk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wtmwzcwe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ecqfxwej.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vydbkstu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gqmswzof.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2eecehycr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2teqhlcgw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2utfjjloe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tneeffam.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbxzcpv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ghtfbzsv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2iaxdllsn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ejazbguk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2uvhxwmwr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ekjneohu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lsrqfkot.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zgcvesyl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qdzjbjaa.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zirehinc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2jqtludqq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aqnlrdef.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dzuxpdib.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2iggmykjh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jrmlskfv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nsmyisvk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bglcseir.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2oddsciej.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2byzoqlcg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hhrlcsus.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jijdpbxc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2khwxpdgs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2iqpqwdgo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2grzdhfub.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rvmhcrpx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dlcdmgsj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kqtwlqpw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xlvcihjv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2esxqfnur.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gxcbiwgi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jjthiruo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pbmtafql.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2datsyhwp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jlksqabp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rbgqxsrk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qkgfkmuy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pmrnieis.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgtdoapx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2paqcmoia.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2juyrdqgh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2esqjonoz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2cnxwhgne.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hamvebxo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tlwaztpn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dxhnnvib.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzusiuq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bfxbjmal.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uammrhyj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ytxqrcrb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ffivajrf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wbgeesgt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmcvahbo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pvmzjefr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ffihwjsq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hvkpwqmp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2bbgtkdqi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ungvezbd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ftllzbsr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2oqmjddah.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2edxzzjts.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2nipypova.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lvldogmr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2detclzdx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wqfdblhu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mbruguhm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mqiwdplm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ztftoacz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ydrtpsul.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2emsfocjq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sornwvgt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2blmelbjf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aotpfgpn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lzzbanto.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ycyrmukw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yxcdljdh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hrdanpjp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2spdcqgor.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fqdjgcod.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jfogakbq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oojurmln.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2joivgyea.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cxfcgieq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xutlxmpp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tmauyvvh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fpjuztge.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lhjyceha.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2euiezxnn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vuzeqyev.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2azkxjtva.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jsguaerc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhrvrnar.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xgtjaexs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tmlnobym.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wghassvr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2feozvsyv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lofmlkau.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rahmikpz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zkeikkaz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2uxvmtfka.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ylgubhte.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bgzmudke.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xnegqlye.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vuqqpcus.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wiwymvqt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2phddkysr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jzqowepq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ahhamknu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pgwclfrl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2klnibrlv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2syddntke.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pngpjlbj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psievvmb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ddqkcywl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ovvhkiww.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2sbzfyvfs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bviohenc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cucpbxox.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ztdujtwm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2opgpevnk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ihtruhuh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hljnacpn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xfyhxqel.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gdkatdzx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eaayfroh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lkcelmpq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ctjpihbm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2laedutgr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gouewfnz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rdeaicex.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2grcllfxd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ujjazqfz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2sgrsvtss.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rndffkru.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rmznhvsv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2resevqea.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2quxqwjan.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mwsiwclj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2kyurlcaf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xjxchbvp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yxporeix.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vmfnillb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbyvbjdx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wgsokqge.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dokmfxkw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vnalobxw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fulqrjzd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kdpxzttl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dwulmpud.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hwycuuwm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2holjkgqw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wewbbguk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wckxhtfk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xufoucei.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2eamqnled.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fkhyebvk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jhjvjtnz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdxyylqv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2igssseeu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2adninjtj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xkcxriyc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2miagnyqn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cqokxmit.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ycyrkbfo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2oownnuju.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2umgqqxzr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xuxkmzmr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hbvvvxhz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2chdnrlkf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bypoczxx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qzbojuog.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jzwshonc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dkvengcv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rycijyhx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ioreoivv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qgzevmbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prffkhks.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ebehsrrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afrqrfrv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mrqavgvt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kohnhvlv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2clyrhcsu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kbctwwxe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hositxmq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ifnaiaxv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2gnjiqljg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbafschx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yyhnhbve.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ecrxzehp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nzrpcpvn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2trrnwyef.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxrguwsp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rcmtribg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2njqynmib.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2oorotdoe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ddanzhit.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qazdlakt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2fzjpcawz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pncbhkpb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ttmxpecx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2btprhyvk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ttohyync.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kizwnrbz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ghylecwi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qzfbldxe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pkuiavwr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nnyopnqb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2avqfzsgq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fzvrjjtg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fdrvmtnf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2duzjdzzn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ykkuvuxi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rgdjjnuq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lvyyklfj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fdaozdqt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kgzrtldk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gyheslkc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fcmuooai.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufcorjju.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vefmwyav.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2axhksqlq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2enpcyapo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eumpzkvv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnzjhlqk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qnbprdzg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbwakmns.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iwldppcs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmagroit.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbjvbsrp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fcecpfhc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smqehypn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxqrlqga.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wdugbhih.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pptznjtu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lsjhscjl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2naawirae.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sugloegk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2guchqdok.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2awdrakzk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ntllvtzr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bvtiplpx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2afdwjgrk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2caqgvdgq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lpulywur.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihprqwll.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2csozdoqu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2giqagggh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bwcglblj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jgenfspm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tvhfckxq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mqiasbgb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rctidwhs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbvjdpzm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lyltvxkj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qhqgejkg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vklbbctm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rztqkloe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zhucfhbx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmftxfrc.html


<!-- 参考信息 -->