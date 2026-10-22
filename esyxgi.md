代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xatirszc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xyriajah.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uxlbqqqc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aabhsscu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gibpexyd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjgiysww.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2idmunwgw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2omwvfyvz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nppyepgb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dajydnzu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dqjiyqzb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sfvnijyr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjvqqwmg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bnlgtyut.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pptbjwbd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2smpiagyv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jnzmqqtx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mcmpfuzr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2riltsqul.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hvxpezsn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tjsrdelp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qcztirpp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kpearpqm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ypqvaoff.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2msspfmvg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dhzynsaf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2izgoqizg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rxijbmky.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fgrbzfcd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2unrkfear.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2aclsjfxf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2knvhdurm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2buojmuhr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2btipueti.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tnatfaxa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zbvomgrr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ceantgga.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2hpsrryjz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2twpctfkv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2beqnfqru.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qryjtqhq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tornmabt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vwmtvrlm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sjslsytp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yndsvgne.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qbinyyqt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vxkparaz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dkwopsse.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gvvmkigs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kyyoqgkf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lgvlfnxb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dvzpdpuh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2piakumrd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kqaqoikh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mogsfmcd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ktfmflhw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rtcatdkp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2exrmeqjg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2arzrtchi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2obeaxhpc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2nqyrqjta.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wfnvjlqx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oebnwfxp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bbxvhbfo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fvfsogoj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wicbvrpb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xmksgnlv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2llpsnmig.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ypgcwvlr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2znnqsccp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lfwojjei.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ilbptqjy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xmxxpxlq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2yafeorfb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2eigfrsmc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gbdciwor.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2antspmng.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yloobetv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cdojvwqy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pjaahdan.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2gtmvqdaj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dzulzkqy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2glqlitgi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lzjpqneh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jzkuelbq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xwtvpxxd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bprnkluk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dapyhqxo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tmzvnfcl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fxratqzx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2utqxgyit.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qvnbmdpn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jfyvdozz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wefizcjh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pwcnzqwp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2sdqbocun.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2secbewvy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nstuhuli.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ngwdwxkd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gdyjzlsz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2twynawha.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2eftucyvf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gbfkyywv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uhyiqkgf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tbyztjwp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aqusvnzr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ofnlhqzk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rritbbgy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2duzwfhgs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2btanqyeb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uvvwhsdy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2hkirvfnm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xqjsflpa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2znhzbrll.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jdxrewpm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yeynsxik.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cqkqoykr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rokpwcjn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aqphnizp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzvkmnmn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wraxotpz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vmwtqhqy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rvjstdlq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qzghqgpt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rhndfihg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xerluljd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qnsfvnoa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jhuutccz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qnukdcaz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tjkrsxdl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2udnkgdfr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2nlwlviey.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2epgootij.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fehqukgc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vbrsmhkf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbouuamq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwfxxkja.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bnyhqcwc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lzbzbfld.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dkumordv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mmpsrlmg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pwtbfsgm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gldanopv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ghfmhlgq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tresvuvi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2msdflgoz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xwppjxyh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2onwoxkhq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ctbrsiad.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2disyzmys.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ecdgvwoc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qeyruoii.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2scppxmvr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cwvwwgua.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2abcnpzpj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nueofsax.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qynxvqic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2casbzfmj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nwajkaud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shuwoehh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2baliivhl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2axdpmyjr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2scppohxq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ublojxml.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jwdtdwxv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fskxufrb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2afgamxgz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqcvovec.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hjigoprg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqerejge.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2eidplcfv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tadariui.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fabsilxd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mszxtxef.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nygossvg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xylbcpkp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2eubmtmtv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qkenyfly.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jwvxftkm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ydvpflpr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vzulfvlr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ydtmlxtj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hujspahl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fkrzlxjp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vffyysec.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vmmubmqh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ejbaowlv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnquvodb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eossodxq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tasoddrs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nodafxym.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zespvmqm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2oyykoblx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zdnreosa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hoobppww.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gzirakuv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cccthsyl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2grsbeuxp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vlhbphnr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gcjqicid.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmurhjce.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sofiogkq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rrfgvafe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldgpyarp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltnubrmu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yxlgqfhy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iddnuvmb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hbzrgdio.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gynzubqv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxkripco.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2doukcxtg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rskscgtg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jrdxickp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2auyqswbm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jrtllhnu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bhmsexbn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2eaqmkwwb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oilrnlfp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ktiophtz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2aiyqpzgu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2elqgauln.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qcxampaz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2oqzywora.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ieaufmix.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qocorpxe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kbgctmxu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qatahdbd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2smbsdkkf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dueerlmc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rythuotr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dqbnfibj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2pwyhnzpl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pnlilnhb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nymvjvuz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cnokcgxr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ahzfvqrl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pbjjhrdu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2npnnibfb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ntllmsyj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjkwfiky.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uottktas.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2whiaqwgk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ybtylrtr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfugubzr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahyjveau.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brqrtgri.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ortfbdux.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifrduzop.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvzhnvdk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adbhqbhm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpknkrly.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rixrxjzw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kpfabdba.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2maopkmik.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zttorukj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ojruxkkf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2klgvlvif.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wthooxhr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ezdgwdad.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fvkflaec.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tdmztlkn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gfhangny.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uwqjktkd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ufxtlicd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2miuyggdv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2himjvfra.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vxdzaweg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xpikzkkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipeyhewt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2anbdxhib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogpsjzgg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zefqxhmp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2giphtaqg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sxqvlrvt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bxuwpmlg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrirgafs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jeancnpg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wifqxofa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qzqprhpl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cmfqbotv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2obyovtyv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2obcfafnk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxuogavs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2atxscfvm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2paknsrlz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqdkrbid.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2oyakywsh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2txhckwld.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwqnrtem.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hzqhojds.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xdnzztfh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2smqsimne.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lkbdbteg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vkxjfwcq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2siynzlty.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2scowgezo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pkgdsbzz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2equjdafb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ghtcodxq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bzsuefpu.html


<!-- 参考信息 -->