代发 wailian999

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gyynxkcnq.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gkeoqvsns.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gqeohmeyn.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gjbfgvfav.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gedjjhdhr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/giwcplqcr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gygutulua.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gswxqhhzj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/glrwmafcy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gmcwkmedd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gbtmvwalc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gxrpdqmbl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gmwtoxtgt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gjrfxrzxl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gbrboqcdn.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbwzacegr.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gpmsgwwsh.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gmxaedpjg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gwokxilbo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gxjrzmugi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gemwipicx.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gbzfzveah.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gexqsxrhx.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gdjewrhxm.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gpqcoeyes.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gzorhjcpz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gcguyzzbk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/grdnjdldz.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/godlhhfxg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/grwcmvaui.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gfxbinysd.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gmdghzomr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gmlxkskom.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gggvbnjxq.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gwtwqbxzs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gonnuulht.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/garivmvnz.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gxnxaymvm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gjkmstqvi.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gyslyxwgm.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gzstasjte.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gpwspoqcy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gbdrgrurd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gmamzcfpg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gztdwdmuu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gjwtasmav.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gcmnvjhqq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzvfcwuhf.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gnqcvnsvg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gdohhktos.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gkqmailbm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gvpsdrfai.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gncstcbju.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gbprqcfbk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gmuxfqntl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gkxsxwynb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gashigspy.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gzrumbljl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gsxoizegs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gzowdiydu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gnzyplupn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/geobzmeyp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gyoizrctb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gmqvpgjfi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gubwcqico.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gspccxmpd.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gxgobkbaa.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/guiqdztag.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gchbexhsx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gieftyxwr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/ghzsfcvzd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gkjucqqay.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gahxdqcfr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/ggqosthag.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggsvlhyfe.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gvdsljgsl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/glmvmnebp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gltychshw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/ggsakwyup.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtmfgrkfj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gkshbmtrh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gertsbtgg.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gnlcxpflz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gexlwesrc.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gcdmfddwh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gaehbeown.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gfizccceh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjhnjjzok.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/guwsuficq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ghvpvszbp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gpechcptn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gmzhwfzyv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gyedirxap.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/ggrgmijpt.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/guvwfpjmo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwlwqklfm.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gekrmpsog.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/glrurfqhu.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gshlmkkgc.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gpmfwfrcn.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gvkppehix.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/ggyysbqkf.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gupzlwvwr.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gfmrsfzos.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/glfwtjnio.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gswrmblpg.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gkvcsllng.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbkctolww.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gdhbipslg.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/giamovlui.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gtjqobhpm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gqgipozik.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gurlxjohu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gogkhvsjd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/guwwlywsy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gxicovhoe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbxqtlhpn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gfnykhzey.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gomnrvcrg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkhfpyobs.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gyefinhfx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gpepufoki.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdwscypme.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gzqgzpyph.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gtlpwkpsu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gwphzkisd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gqrwhrasy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gnbclfnic.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gslrkiuia.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsgycdgks.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gwpwmqhkn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghobjhhdj.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/ghrujoxbl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gnhvrdgqd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/glcyayijx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gnwctqbsu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gvuqvjtae.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gpnxwlkcv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gbmzvqszv.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnyyuedhd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gazkhyfeq.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gtbuqqkkb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gnktbewfa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqxkkgvy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gpyezzeee.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkpyighho.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gmgsjxtvv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/ggapjhzua.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/glgmngwia.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/guldfwqyg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/ggtyrbaoy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gqmgkppwm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gsfzdcnxf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/golmhvkfa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gdekurzng.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/goxdlnpjq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/ghjvoxrju.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gnthgxggq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gdgdosvnf.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gxgvijcgh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gvlpwiobl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/ggydfoejt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gzuwatvwl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/guleqoyyi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gcgkaunwq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqhpekkvo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gefmfgwld.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/ggikyobdm.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/galufsslg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gnxunrnvl.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvqpmxakh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gruaqwdwo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghvmbrzds.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gigfsgigo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gbddsesfv.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gievaeyyj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glezctcuf.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gpmzvisbw.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzqjugodo.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsmvmcdth.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjnvdhiyg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmprnrjcw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gfrnyxfta.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmjzwqrkf.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdfgxonll.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gcwtpkujv.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gevcgqrws.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gcvzhpahe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gogllfriz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gatbjxyem.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gkvrqdhgb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gksbdyibz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gudbqlsgw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gubxojkqn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gfwncwtue.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gdkpxfmep.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gwmpqhwud.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gynpptabq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gkjptteiu.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqdzrtxfq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gxtxpqian.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gzutbpuip.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gyeetvxpm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gxehxfebd.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gqwiqmmks.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goodcfqlu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnwvyurls.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gghhfzppn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gpimsttmv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gmcgjkvpt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gqulqzyrz.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggionimwe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gddnruyep.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gmjxjfyij.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/geffqvbjh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gnrfuodid.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghgthgrpx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzivboeat.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/glwjbuzbm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcxlflmie.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsujflfwz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvasemccf.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gmlmaswvw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gwclbkwbd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gibgymlcv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gdsoxlheu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwglkpugj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gapzinlgb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/goelrexvk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gnnudbhrl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gryzddrqf.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gbjuqioke.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gwmuybvnk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gyunmikrp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gdzhqscew.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/glddwhzid.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gomhwxpgz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gcoumqhox.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gtbusezks.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/geftjwqwa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gldinpkke.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gprcqlnzt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggroqogix.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gnnpudhta.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gseblwzad.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gxqxnsbac.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gbcjrakuq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gqvybcgel.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gsbjkmhze.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gukbwuley.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gfsinmypo.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gcnlirdmu.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gfconanno.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gkzbcvoze.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gofnvycii.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gzdiivfyh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/ggocqkikf.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/ggsynurst.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gfmzgostc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gaynpuzxu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/giiasjrvt.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gygmpwten.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gzmrejilp.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gvefvcldo.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gzhbawguk.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gqpjnsivx.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gbcmgwzpy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gwwxswjxg.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/guqfovlpk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gbutchrfn.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gxtdzlnxh.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gnvogvyen.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gxlsxivag.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gcehrlufh.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gfkngenng.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbomylwoz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gcnrezrqm.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gsthjmums.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/ggxbuxupj.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gvcgoatdo.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gdqdvqwie.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbdyrjybl.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gbyzkpqud.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gwzfbpnrp.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/garyftuor.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gjgsmfdvj.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gbunqqskh.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gzwijttls.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gprydfxnk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gsnlbrekk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gmxklvykv.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gukpwsldy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpjyklcxl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gkkcyusxk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gwkzpehrf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/guittmtii.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gwvuttnmx.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/ghuelsujf.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/glaxiajwx.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcvxukwtb.sHtML


<!-- 参考信息 -->