代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrnianbo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnrzlnuy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunylojsd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmpbsqfb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fanxiaobao.xyz/Article/details/gakalmyzk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxumrkqml.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gxhuxrrwq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdagjokmy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fanxiaobao.xyz/Article/details/gqkijucdz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gysyjhsqd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fanxiaobao.xyz/Article/details/ggmryphaz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqfnlrn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gauwhziat.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gthiqxoig.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcumjwnvq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbromowbh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fanxiaobao.xyz/Article/details/gduyrujsh.sHtML

[E11] 反转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiwxqihy.sHtML

Py:   s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/goexfyexo.sHtML

PHP:  strrev($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gzngyghkt.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwehlxcgg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkrbveav.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrefqsji.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxveeitd.sHtML

Ruby: s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gzadhsmnl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfmejxzx.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gacmlvbco.sHtML

Py:   s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gorrgirla.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueavwxqg.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfakakpds.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnntcizi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbqcqldk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbdsakfh.sHtML

Ruby: s.count("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqytaond.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fanxiaobao.xyz/Article/details/giuerpfis.sHtML

[E13] 逐字符遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gxipfssyw.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsgruoza.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnzbivflx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gultkbyxu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqsabcexr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/grqoovavn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkppqmsi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjndpczv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveeyghgj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnpxjuqi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fanxiaobao.xyz/Article/details/gnvoesfkl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gfgafuhct.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxtrcemj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsbnnmoj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbciwuhx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqvgoezf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fanxiaobao.xyz/Article/details/gxjfejzqx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxznwqez.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmuvffam.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fanxiaobao.xyz/Article/details/guwzyohch.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjpshhii.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcauudznr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktkoabwp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmyooeeg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhidknqu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvypncyg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmbsfuxva.sHtML

[E16] 数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/giccphluy.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvaatmxz.sHtML

PHP:  number_format(1234567);
来源：http://3g.fanxiaobao.xyz/Article/details/gpyspohxp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gviiqfssx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/gvqopvsco.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/grvxceuxw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fanxiaobao.xyz/Article/details/ghhadbryo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsvcybom.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fanxiaobao.xyz/Article/details/guguchjjl.sHtML

[E17] 首字母大写
来源：http://3g.fanxiaobao.xyz/Article/details/gtmxbvgrs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/gqhyhzudq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfvdwrus.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsqrhtssh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjsdefsm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhpxwcwo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gonaroljv.sHtML

Ruby: s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjuhqley.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/grpjqvshu.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdomlgywk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fanxiaobao.xyz/Article/details/gsfjqququ.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylsfydcm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gdnjdvdpy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/geomndhcv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gwuqyrzzc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmubigptp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzwvvbdx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtjbndwup.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gvowavjgq.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gltbnaqkf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gvrlywvrm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/geecptitq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/ggxokwjgt.sHtML

Java: s.lines().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gmryxnbao.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gsacjdtpc.sHtML

Ruby: s.lines
来源：http://blog.fanxiaobao.xyz/Article/details/gtajqkxli.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqyctdns.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fanxiaobao.xyz/Article/details/gjvwfhfmx.sHtML

Py:   if not s:
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkxyqzuf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fanxiaobao.xyz/Article/details/gbudtfoqb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gocwdgyqn.sHtML

TS:   if (s === "") {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwcvzfqd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbrhdyqat.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslxztuha.sHtML

Ruby: if s.empty?
来源：http://blog.fanxiaobao.xyz/Article/details/gqsyencig.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkubhyvxz.sHtML

[E21] 超长截断加省略号
来源：http://wap.fanxiaobao.xyz/Article/details/ggdpnjcao.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fanxiaobao.xyz/Article/details/gmhoqckwg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gogndgjub.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gvfuhherr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsbdcrjg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gbecgkkdc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxqlzfdi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqzgtsiq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/ggifcrear.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/gejtfnsih.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gieztnjbd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcczxrjgl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gcrfqhloi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysjmqbrv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqppxqiop.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghccljltt.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvdeodpx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebvzybnx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/givmtudvb.sHtML

F. 文件与目录
来源：http://wap.fanxiaobao.xyz/Article/details/ggszrihpo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqmrkemlv.sHtML

[F01] 读取整个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkzzobzm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fanxiaobao.xyz/Article/details/glksukywo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gdfnkxldq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpvkooit.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gewndfdby.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggilxdbos.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunmoiiw.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gmgainmsq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gtrjzryrx.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnnoisbar.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlaokapj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/ganqqelsh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwqgbvhrs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gobfnfxzf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gszybkxqs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/glfpdxxpx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrzashzu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gugukrtlt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/guhlfmdvk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvgiokgx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsdlrckz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfiuybyg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsibjvju.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gnajowfbw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fanxiaobao.xyz/Article/details/gjddryteg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkwbzbeb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/grdmjuyfa.sHtML

[F04] 追加写入文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvghgbao.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/ggedazxhu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fanxiaobao.xyz/Article/details/gixiuhoem.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjncjqnba.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghflkxlsa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibdrmlmd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdggnzsn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcjsocxz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsybnjqam.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggehffvzf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtspymoah.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gectfzzmg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsfmjrtb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciedhtiq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gwljkcuga.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fanxiaobao.xyz/Article/details/gekfwopzr.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gpjnnaaob.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gebeznsfi.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gziwhnuwl.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghszhkxro.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gontksutt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktphqztz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxzxlrzm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcwwknww.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtfbxwgz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoqmfwcl.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gslqpjoyi.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gimfuaapb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gndzcnleu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gsoyyycak.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/glvhfnpdv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/goobtiznr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzpsryydr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fanxiaobao.xyz/Article/details/gnoweurwv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbhpzywo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gduapnafv.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gliflgtgl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gofpndchh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvkbifjm.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gpmomqfmd.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpsddtqx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/gpozitlvg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzqmzptr.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjbvydzd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gucvjdurk.sHtML

[F09] 获取文件大小
来源：http://blog.fanxiaobao.xyz/Article/details/gspojtlps.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gvzqkkeka.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gejzmpscb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcylzejtd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszuqokgg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gavhizpuj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudqlzcih.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspncyfnr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbjfiryc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/gijlamlxj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gfzhimsmo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcxntgyu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gixhinosu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/grdkesfju.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fanxiaobao.xyz/Article/details/gtqxbdsie.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gacpjwcbh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcloyxir.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhozhtqf.sHtML

[F11] 复制与移动文件
来源：http://blog.fanxiaobao.xyz/Article/details/godwnjemc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gnjhbiwph.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/giepvlndn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gvfnxrjio.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsggrjhx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gacthiwpb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpybflcuo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gbuzsyyoe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/gcjeprzqr.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gcjxtrioq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fanxiaobao.xyz/Article/details/ggajjgtjy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fanxiaobao.xyz/Article/details/gnibgboya.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhcnfijp.sHtML

TS:   // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqojyvat.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/glhwiuukp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqsldrwj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fanxiaobao.xyz/Article/details/gmwpgbrss.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuxstwcv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpaodtzr.sHtML

G. 面向对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gosbbikxg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqgxdmsv.sHtML

[G01] 定义类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gredpfbno.sHtML

Py:   class User: pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvkgcjqe.sHtML

PHP:  class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtybuttt.sHtML

JS:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmbkbpxq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoekabiw.sHtML

Java: class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gsciviyoo.sHtML

Go:   type User struct { Name string }
来源：http://wap.fanxiaobao.xyz/Article/details/geggsnmmn.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjpyxjxe.sHtML

C#:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/golejuavh.sHtML

[G02] 构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghjbexiiz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszhjnrax.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkmbvngih.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmuwsdtb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfcrzscn.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkdijsgja.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fanxiaobao.xyz/Article/details/gkltldqec.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkintqeac.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geztuzlth.sHtML

[G03] 实例属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gntfnyoyx.sHtML

Py:   self.name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gtlpulxqx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/grtsewrkk.sHtML

JS:   this.name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gtubocxbr.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpqcdlmv.sHtML

Java: private String name;
来源：http://wap.fanxiaobao.xyz/Article/details/gnziffvqb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhjoymyd.sHtML

Ruby: @name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubzprgus.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gvsxhniig.sHtML

[G04] 定义方法
来源：http://wap.fanxiaobao.xyz/Article/details/gmuqeyejj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gofwadihl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxptajwhr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgcdftzx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitvjxrcb.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxitblhur.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnmyjupj.sHtML

Ruby: def greet; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gxlwcpyzn.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegrvucan.sHtML

[G05] 继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gygqpyyow.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxhvjvml.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqznjsilj.sHtML

JS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfzvnaich.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsuocvky.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxryutfr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fanxiaobao.xyz/Article/details/geivohqst.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibrbxsog.sHtML

C#:   class Admin : User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzohmems.sHtML

[G06] 重写方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdcqtyox.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fanxiaobao.xyz/Article/details/ggyafgusg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjrnyvkuz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjtouzyza.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxphcddi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyyiwtlvp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfeqocby.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fanxiaobao.xyz/Article/details/ghaudfhtg.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fanxiaobao.xyz/Article/details/gczochtnn.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddirxhjw.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxpaxbfz.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoolzubc.sHtML

JS:   super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmgqxgqb.sHtML

TS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gmvugqnja.sHtML

Java: super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpnaekdw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhkbrmbq.sHtML


<!-- 参考信息 -->