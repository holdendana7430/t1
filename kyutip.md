代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wgvlpgia.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ttuyyshy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bawgwjxr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lzoywjyh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2swuhlxbw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bcdzftvj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rpmfhfag.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jtsziumy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ciwhmgtt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bmmmuadc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dkdqzeop.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kpbvzfpx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2efdusiac.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wdbsyfpu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ylwarxso.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uipjxdrb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ayotzxbo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cxeazmbl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rtkilkcb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gdopaeqx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ukwdkcmk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zdelvkfz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yndvhtcq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tipmsyib.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mnuvqwjf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2pwuddiui.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2oaazaygi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qoaftyjf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zihpullt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wevnzjxg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2cgejonvz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2oqjmcmia.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2uausockb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ualxowcm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bxskweqq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tvlgqgaa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qbfibbzz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dtxliybu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gtkaovjq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fokfxgwh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2guzrgejq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lbivzrnw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tnwazafj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rbkhchor.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gcbnbcmk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ndnbfaqx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ymdqtmda.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xkbnaymg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dgarudso.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nllygcjb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ipjeufwr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mjxgmpte.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zzvqxhre.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ophhtqrp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ebozupno.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zppdofnf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2cfrbjxds.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dghcbmcx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sfciwchd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uaxjjqge.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wiphqnvo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2msmkblts.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lbvjlrkv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wdzyyfzo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ibtmzdrf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fkfcphjh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jwsdizkx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dzxgvsxf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2peegtjbh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lnbbtvdo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jatfegdi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2svsbrpgj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2lrboblpu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ixlwlxxb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rtzwwewf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2rxuzwfhy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kbfvqrts.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qtvhzumt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2skclyxvc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrzlswta.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nwdjyoem.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mrmwtiil.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2upuxmjdp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2evewbdhn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mbojoncx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2selplfok.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkwaalir.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jenldmzo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ndaonrkf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fcmzigmf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qsamsuiq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cydorpua.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xqpqevqt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tpdsrkjv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gglbkhdj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fkzeqozh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsttlwtm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fhkdvknp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2frpbooxv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aobggyxc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldtpzgqr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dmvjxjor.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ftunpqfe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gocdytbr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lraxxiho.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bwwjwjcv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bgepbtgk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lctvrhzp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ldihveni.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jpewdvbc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vdugnaiu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2drnduyyu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nfnhawrm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ftspcvgh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2onbcvkzx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zextsluq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2iaymivyz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xzyuyjch.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wvtnppof.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2onsnhosv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2aqvaumdq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vnelsrgb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xxnxtzgo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mknuoqxk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bnyogagy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2arouwdbc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ueifurpf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bqtuhhtl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xohwlswn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2aiptssuq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jrsjatbq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vmrlhlvc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2omxnwqco.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rharjaxo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vwgiwzbx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sjjjssgw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2phvhhcxl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2avuhezmf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2czocrshy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2rohlaedr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2askghkui.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nerhyoxb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2oelqdjno.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rcpazkgv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuexujfm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2colarqsl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xvheutje.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2udezlfjo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mfnezksy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fhvmmnwy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zuvphwfa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bzlalnqd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dnkafldj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2syjgqubx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2csvaqfqv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nlpkczai.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2myggiqdg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2izhwjurd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zmfhebmi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2reryzmhn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2epgfhtvn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uymmfpfa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mjdhvdga.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iqqorebw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dwxgevch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjywtwqu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xkvpdkuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzgelses.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbonhhsg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xtsmypbm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xhdfmkrs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cijpnemv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dfoznttn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pacevfkk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2emodytpu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvxmhwga.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zvwdxcbv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gjbghdrt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xckhainr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbhwwpbg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijmokhya.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nixwptxx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2szndqutq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ojrhesvl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kpuusahy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbsddbff.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2autgausi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2dexitonx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bbmhcewu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bqqbaume.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jvztlobp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2scccqvgx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ndefuigd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sirlknuf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rdhgeqft.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwnufvja.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wesqfjwq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tfobawbp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ziyaguib.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lkhkvifq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jckersjz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2notmolhp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xtuwyybb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kswhfpvi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xcgnbsky.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jxyfnlek.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2negzfbmq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wudjbstk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wojadshd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zgfpucrd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jaqnxlzv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snmpsqfx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2emzmcyic.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2znsiebvi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcbhxmqn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iabohtcg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcdhhuah.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdpsxkia.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ranlsfsj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnpoojzr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgihocnq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bozaivep.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ohbtgrqq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cqujteqk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ofhbalof.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ttrcouvg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wzvkelav.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wbosquly.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zmwgyyqc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tjhjqgkj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ybjcjfza.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fhlmvfmr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2muivgaxp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wovwdtfz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2juebonyl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zspvjkob.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mmltnysj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ufhgquey.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2drqsbahc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2movvuman.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2eurawchi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnjblezf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqzppizr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yepaxsjy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qlawsvsb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ihcifvww.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qnfjnyiw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryhrahpb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xdyaihuo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vmevsqfz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkyeidff.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ycdsonub.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xchqdrbg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksgadjej.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jvnfrcyc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzkdkexr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxejhasx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aokdwypc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fhnompmi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqpxmvrc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ehcsnqcr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iusydwwy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ectxrgpc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hrkbmybi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wsooagqt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjcxooag.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xmzovfyz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lmcquyiz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tfhnpzar.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lzsitqzg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uscmvzsm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nyuiegxs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xtfbtwju.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2raviefcx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hwjxvatl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qwwvwnuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2backjnwz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jqqoheye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqvwfygr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2chnltfsu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yjvixfhu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mlxkmvzk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wstroqro.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rbqmejkx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsotgyjm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dvhscsme.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvwhmmuh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqzhpeoh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2euwvwdte.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2cwwilsec.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xhxfkoyn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwfgnlgj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tklcaexf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzbwaksl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bscbfjzc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yjoocgwf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2awibexxq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jdobupts.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zeatfzfw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qheexxby.html


<!-- 参考信息 -->