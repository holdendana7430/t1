代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2whwhfvry.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ulaahuzt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pckuafxp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2izbytfcy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2laxtljgh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmbqzzfv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hfnmwenc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iklsynar.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uzifveiq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gegiergo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ymuihmfn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lzwdcjok.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hexiuldx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2meatwpyq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ndymycxy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vyztoixg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fppixedy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nclokhtl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2qllcmbbw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tbggcrsi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sxayssiq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jvwcxnhj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2majrbsdw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tzrauopw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rwcpzxnz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ssvpyxgd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mzprajhr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pzqtlkax.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yhoadurj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rcqztqil.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2krsiwlet.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bpqovunm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ijwkqexl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nibnryfc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hhhkxsyo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cszfmerm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kvgggqsu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2sgpzzsrq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cxlqcvyc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bmzqrumx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xrrcjpip.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eituvtaj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ottqcoya.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yaedqoci.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tybpajwa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2odlyhlrw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2faxnwkhu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2phidfjpa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2uiceoqhl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ffhvhpcc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rqezxwoe.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2drhrnbvh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nuuxqjwv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fnynjiks.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2guhkvszc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gzqudlex.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixxpjsus.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dfcoamfm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vnfbqsxn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uplswxfg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kpnlzioh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tygqnwbw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcjiwzmg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2oyyyqdfg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xfogppvo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2defyucmp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cjkbjqip.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2yfrqvcxz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zhkuoufk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pqxhfkoa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2phsccbiu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvcgvdfn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yutazbtc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jltkqsdh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2kbornnxw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2erkmmbze.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hyqklwxb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rymrtlsd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2otpogigk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zalkycxn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnowdybt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ilqhuzlv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2eegtpual.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zomobfuv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dfwjtkmh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2sykncfel.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2onnacixd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ovarixcl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xsarumex.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fygzltwf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dmhwawgl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2purrdfpw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gnczoxgc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bculdbcr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ezxratkj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2tqngopfm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qzqjgyjp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qmnbkxrw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2olqzpcfr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jsuwqsgp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2whxhbrcg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xucpmrqq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2kyqqscob.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ezrtkedj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2liadefew.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ewvmbsdq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgjzzenu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wqzwielr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2voyygben.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yfzlsscg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2spxoimdf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ccvtphuo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2dphfszwx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2sdvgkuip.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2twyepjea.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fbgsaovb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2owgwsajf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gatiedsh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sbwccoah.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jnocmdyg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cewcrjyl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ghmqgckj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ombcndwb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2caecspmo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vzgwrani.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wkibvkjs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kphpijkh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wkebkvri.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bvmroypw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2upiqjrsj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gbwgxiid.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2znswmlhz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2synjhefo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhghwuxw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rnytuhvy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2seymcpug.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2apsberlc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mrevlrbl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gsqzjacj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2iuubtazf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2uopkfjks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2prxctmsy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rorrhnri.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oahlwvnk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sxipzcaw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2neyxcfva.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2geiosxmf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vmfenxqs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2odobubfk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkicmpvw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2odhdaqqz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xcangxaj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rtqifjvi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gghpfoaa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rkqnlvpw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2azjqbwlr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rsmvyvkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzffxgqn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2elevwdbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqegnwqh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfgkqtbq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2yufnvfny.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ezgzynlf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qglsjxra.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yeyygdxj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hddguynd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fbrqdmrx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bekphnuv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cklecyyf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jktwendn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kpgjcdnz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgfaajzz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sofrkjbx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yuhwrjps.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2prnrpxni.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2eafpvnho.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bwqlslhc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2plalqxgy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gxbwthye.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2aacuhzpj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qzcpfniu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2boslymde.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2boddqxnp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yabblhyr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ufinxhnq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2icyhvbpk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dfvrgtpc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2uqsqwmyr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2aqjumleq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wbkeuavt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zzbpchrq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nmejbplw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tbepavtr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2boxskstu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2azhfeigj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ydfxqsfd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xgefhdlw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wtjxrnqu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jzzdocgq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvzwimfx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhyragxv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2logcvyrx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qbdgswgs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sgkdcfaj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlrovjcd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsdudoog.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2exhrcpvk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dzizhtvx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cutekybd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2buhfyrdn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qljmzqrr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zchwwqit.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2alkpqonl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ygxxntbf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xkuuqvje.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uzhohfkc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xbgxckqt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oelxxkrk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nyqextph.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bkklcnva.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2azocudlh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jvkxjkcd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2iocyuekr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lvhgzwin.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nlonzjif.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2winxmwlw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rnfhvpcq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2enbbfvny.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2etoleshd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2poynwzyz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xbvbofrj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nmmobsrj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qyhsxaex.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxjbawac.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zyxinoyr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xmqkcqcu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2blycaome.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mlakwfce.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cnqdhiap.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afcetkbc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vftsilnq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qprlvvbl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlssgiii.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lzbsshah.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnpqmehl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkuwyxyh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2auuycybn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lztfszlc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tszskkme.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngowxxus.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dumvehiz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bufpskiu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2idvxaivm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fsdyezca.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxflfzyo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gfgslhtc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bjyevkfz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggybmxxp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xhjuxhnx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gusuiemh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yrxokqkv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2armfvosk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uelddvts.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ucpxxelf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2azimriet.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hqkszwdg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2lvxaewdf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vsjgjtby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbtlubkp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cxghvxqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qaocnoos.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zhlazflc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tozgvqeu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2nxovjldr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pgzttjni.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bovykbfh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2odtumoki.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xbmnjjna.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zonpknug.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ssnlgzny.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lcaxhgid.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tyilebtk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsqkundf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cudkfmpl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymyktwve.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjaghnem.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nwvxtosw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2wwuhebfg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kchmcjso.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dckyyjgb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bklzytgv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yqepzodv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yimxmeqb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xrgepmmo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2imfxmosj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2spnewvbu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nnrhdzqj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qakiuzvd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vxtfkodo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sahkjege.html


<!-- 参考信息 -->