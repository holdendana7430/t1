代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zafluxxo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pfzidnyj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fnjggnnj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zvgahfvj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hrzautsr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3shjaynmp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3leulxarn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3thnhembx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uaxuvhog.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kqfsjvlt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qizedcui.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3azpukrjl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3isqjesyz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zpvufbgg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ircbdtkz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mtqoddtr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uqlqhsng.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ytwpbcwj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pbzkojhr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kyrfdtxq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3eoprroao.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lekvwtdp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jflrxion.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vonmkoup.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xrnlauct.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqodmoqg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3heclfqqz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ggwpnndd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ukrdpetr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gflonypx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wenwmzoz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cvzudgtc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3aawzplkm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bcjvknbe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcwovwme.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqmiasuf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eamtctfr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ooiohqtu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jrwsnlat.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iciyacht.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3nizknqca.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ogsxkvvr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xltpeeks.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3euuodswc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nopoemnf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3srballsw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jhlmktvj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3knvknyxf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ahupotof.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qwhtdsui.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqqeyjhb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ssuivdun.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pbvpksvd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3niaszbho.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xvjxphnr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3schepkpn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3luacilew.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltrmntjg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ogdhneqr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3umzdjips.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zimnbjuy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3advqzunj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3shjdpzwh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ygxdtxyc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3sewewuwi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jnobggtf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3yidazzem.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ijrbttdf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vpwivugf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wfjbnaog.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gcdxzmay.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmnhulfp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wrzlcmxu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bouxpxna.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rtdbuwcb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cwueqatv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pgcmrnvx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vkkzpbms.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3mhgujkhy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3akonmsgu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kvlepsut.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pmivovhy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vxvjrtsi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtmufrxy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yayggpri.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rfebcetf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3unacrwzw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uktomltq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfpovua.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nexzdxwn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vutqbltk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wbzbfwhx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ptnvsglc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3elyeqvsy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ixogdeyh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gexsfopt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3vlwbhxca.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ghoqseqw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wbmbhaen.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dipuoswx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3flkqjlio.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3krhhcapd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3eocqnugv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rriiotis.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wcoxieix.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bnzuhtmu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zbyteyyi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lfmpkoeg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eyujaofb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3eglcownf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yjprlcbv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fcladnmv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3oelpmhfu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lamsvknn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dsfnhpjo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3koebnxua.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3darfazbd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3feyhoblp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jvzwmcpt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wqmfbxbl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xwmpkrch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucpookuv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xwmmerbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inklqrol.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vsmsgaee.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lwtwwhrm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hdadmpgj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3sxsgtzdu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lftvonif.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ohayhykg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3oydkywgo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnaeftta.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vzrmsmnq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3giyxaoch.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ozcqbdpr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3iljzsdxr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mphqnfbh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hjwqmjwe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rcozhulu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hdpsdihh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ghymlxuz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ksrcfuee.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mhmoxbua.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3czgjlcar.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xrbzpids.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qqdxnmop.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zufdvuvx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dpxrpurw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3exdxrmta.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nybgjkoy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eebfopzm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ewxekfsz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zryycizd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3owmxovsr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kcdxdzse.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lbeyrtwx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qpwlgfiz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qkhstekw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3evznopqx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3krbwtklx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rucosjgt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mjtqopbc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qrkkqxnp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkjxeswi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jywmasxs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fxhsferw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xdkzpmty.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcywktqv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkzuvfqn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vylrslqm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iorqrukc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jskhnmgj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdbvefgd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pfzjuupm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fhrpsqio.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipenyeds.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bainhzxu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dmswuzfn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3epoellwn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ypyuxhfg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yrjtohgi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3smskdths.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bkfgtpmo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ycnsoprk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3izlueqwg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gaenzaex.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pufzbuqy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3iwnbkdqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hpebsvvq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hfexbepp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vjfnetbg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ptxyzcbe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ikbjrreh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gcxqzomc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wqngtkjr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wehpauwf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3efqegocz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lnmvcjdr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dyfacqht.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lkbgrxur.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fjviemta.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rnyzzxoc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3raakmhpb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3urunekee.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ivhqgycu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tzspwthr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkvkncil.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qmucknoy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avimdgsz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynvkwcob.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3acitoqsp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kegfjvzn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svhpqjhr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohrllckl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqeoxahk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tufeyqea.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xqqxnrzk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjpcosfx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yeohyghv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xlphqqsn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nmlibkmd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xmgunzjn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ojwdtqam.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wrltbpyn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ybmmqgcf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tpjeoinw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ukifcizb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3lnjgciqi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3lxtomkio.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ayixwpmf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3exssryic.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mjdhkmld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cizognvl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qlvyguzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chlczypw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kkwieglc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3esihymlt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pfipuisz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vbznsjcy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3diszlysm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hphlxqgb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zjocspvh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gthhajlp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ormznwvn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpfwjujc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ihrcoqbs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpgeshsi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ccihlzrg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xynxfjkh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tomchdef.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3roljouxj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qkebfjzq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiaccrgv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sxfywqbe.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pnuhfqaw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3roajaqkd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gauyvpsd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hzueclzf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cllwmsre.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mtrratxm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gzsdjhdz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3utjfnuwm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wigzywmi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pkdxlmmz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqaisigs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaofujef.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aikvmbxj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lltxovci.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rdnegwch.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ojdndopl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zbjgkncm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mzbjxfxr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yybuoijy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3byoxvrlz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3szftlruf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lawmrjxx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gfwgkwao.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uemsmawg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wacbfywa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xjukmspc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3srnrzmhq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xpwcxnow.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qozbifnw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uinxdxmf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qywncpqw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mteocijc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rjyacfcw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jtcyjytq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qmkqdymc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3fryadrkz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bdzfyajq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pzxqvliv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3axydsitm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ciivuzaw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uzorehqz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ssaipygh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3udwoador.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ppvxkefv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3aumldvmi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3uhjwfbqz.html


<!-- 参考信息 -->