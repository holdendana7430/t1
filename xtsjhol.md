代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gfvlsgfvn.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gzslnrcwr.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gfdrdnxgu.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gdektdvwk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/ggiorqyad.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gnumdoydw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/guvifasis.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gkrxzojaj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gjfnhsxpi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gmpvjspci.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gicjevpms.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gaghqqmmn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gqhdihoyp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/grhodnfao.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gebciiixd.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gunboasfq.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gcbtmktac.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/glishmmww.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gqvbltkpb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/guovnoxsn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gqejxypbu.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gudwtrdtw.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfgsekliu.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gydvipdlq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gblbzkkeq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfpmhzifm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/grtkanemu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gdxbtbxqn.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/glaryebts.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gfekrtxdx.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/giqcnrczw.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gnjrqrssq.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gwdrnyjdc.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/grilcwndf.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gzhjvatzp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/ghwbvahef.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/grrvcxued.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gbejaswbm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/glhgbuwry.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gewucsoib.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gbyhylcwn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gfxhznlwt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gurzkooth.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gnnqnbczs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/geaylkffz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/ggzparamy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gptlvizkg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/glfbthhgd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gtwrrdnnl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/geelkyrgv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/grwuxpyip.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gyiaowedk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gomcoejbl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gerewfkem.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gzvzcrmtc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/ghcnahegp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gcruxeqae.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gsbojcwkz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gcjumjfaz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gceajnxda.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gzycnhezj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gaoklmqch.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gfrcxmnmj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gesfihnsl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gssbxmjkw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfdfraaxq.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gxqbtydbi.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gxojsbjhq.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gpgienqnn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gvwxgqcsi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gqjffxkmg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gwxtnxxvq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gzgtlally.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gmrybaxnj.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gykevncpb.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gyzcwjsis.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/ghuihttxt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gqfxrwhca.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gzmgwjszm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/geepyjbpm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzbjpkdea.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/ghnqnqkws.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gcysmfwjm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gmtpmsjxp.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gogkxwyke.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gpixemmmz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/glgbcytjd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/giiumlxbm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gbsgsvxyx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gnetdgkoe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gmtbydudp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/ggpydrskg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gojrmtcmb.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gpuoezuiu.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gnstjpffd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsmkniyeq.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gcvpenkmb.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gmgxkodbr.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gaqzranue.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/ggbahnvev.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gigraclxn.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gowwajqpb.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gptmjbspo.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gmnjmxrmh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/glygezcmv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfylrpsvw.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gbztwfykj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/guewblzps.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gupeyfism.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gonznatxl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gbcbueirt.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gdpzenwqu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gctwbugea.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gtvnpzrsp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdprurxon.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grxvlaoke.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gmzuvplwq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gajnlifkd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gsjjuyajg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdefbdcsz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/giwvaoemh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gnzzfidlg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfxwjtewi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gizxkbfrs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gcveymiha.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/grzaasejl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gaonehlrj.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gozbiyoip.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/glypbqxwb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gndvebtst.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/ginrgldmc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggqxqnawb.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gawsijvoi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gzdiffsiq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gevufkuaa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gpevvuxhn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gryyiovom.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gpcdpihnd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gylxbqwni.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdhgvzuap.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkxqspzyx.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gpfmdzrgi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gmltjfudi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gtakrejzh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gfzavlmgt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gtocpgioy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gfdybtswg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gbclwdeyn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gnymhppqk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/giercrjdj.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gybwalqoj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gbnhlhmkj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gfiqxeoem.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gqzbgztvc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gvxzavvzo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gbdszmygs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gyyrryjox.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gzwxotppg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gnvparkwq.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/grekbudrs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gctojkfeo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gsilexgsh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gdookavea.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gyligcaan.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gjsehrvcj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gtpbkikrv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmcddpli.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gauettaqw.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gkmmrpzyw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/galpfmwui.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxmotazuv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdxesjusf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmdenubld.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/ggufdgvam.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gebictbzs.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjvdmuaql.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glwvoxufn.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/ggossnqgz.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmmwannug.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggstzkrtw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsukfghio.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqusaaqwe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gperbdour.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwuevdigp.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glklwnatc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsjbpppcf.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/grslnrmbn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gxoyhxtei.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjmpbmyju.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gkpshfian.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gdwjbkjsb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gcjmoedko.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gloeocjkk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gtuttbkcf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gcwfnxfyv.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/glmlkwvkr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/glgmadjmy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/giicbadej.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gymnrwgbs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gwankzlvc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gwqmkauqo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/glaxguytr.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gaglrvswr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gitqmdfch.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gulfiphol.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyqqbvtjm.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gscqjafnn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gzmaamhrg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gxsivhygj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gkcmwwmuy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/goontxrxj.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyeskaunl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/goimryids.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gngutudaf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfwskpytg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghqqawyts.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmrtghcjl.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geubynprj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/glkhkzczx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gppjqvwbu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvnmjdwqz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gauywalhd.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/garyfejfr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gzjqyckbc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gbatemktp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfxzmzbfj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggnxiwcqy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gwceswjaj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gbodnuzyk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gsyrfdmga.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gbwtbatua.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gimyypsol.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/ghgejrlka.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gpeiwvfzl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gesxqodus.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gtbaxvily.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/ghynlcdmj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gatfkxeip.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gglaxwrdy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gtiwxlhjg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtorzbuxs.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gnbbvirfv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjbyzwhuj.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/geofbmhvs.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gbsrtgqdo.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gobrtejld.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/goruwckqw.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gegiovwxi.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/goeblgntx.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gftuofqod.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gprzlptkk.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gnqnyfzqo.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gswkqrrdu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gduiwdtjc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gwigmjtws.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/guvnacgtw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gehksomvm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdsxcneda.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gyhzvroat.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gtopvgbwh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gloidjwyv.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gwwxolufp.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gblsarioq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/ggggdehfj.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gboynigxw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gncawohfz.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/glfskakim.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gcigurojf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/grunxpucd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqgcdtuwc.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gcdxlwixi.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gnkatgpta.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gijywiwbs.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gcttdpvpg.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gtyisbniy.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gsigfyeyr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gxmxrhmga.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gdykvwjcy.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gsnkdlhry.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/grkwmrevv.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gpflsogsr.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gxriiakmw.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gzhrpjgav.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjmyvmztf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtntsiofe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gramjcwaf.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gadicspcg.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gxjypqusb.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gtmlhwkof.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gvrfobros.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvxtwjttu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gsxxmdila.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdagbhrrt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdavyaepz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gwsklkpcn.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gyutrasjm.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gizbefksq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gvenznhjy.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/guaoonnwt.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gtzfdrrcs.sHtML


<!-- 参考信息 -->