代发 wailian999

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gjsjkzrsj.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/givdawgzi.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gquowdtqh.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gezzidmqw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gfhkklisn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gucciaiph.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gunedvhia.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gvpplafdq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gyszjdgnr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gbornmlfy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gpoucycmf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/ghasepkbf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gzwbvfykt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gnfrbgcit.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/geachykoi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gnmmpngoi.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gjulcbzfa.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gmjcadmcj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gqirmtqlt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/ggwigyhkc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gtmwplbwl.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gryetqbce.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gbiqurhfa.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/giodabfcq.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gvxgftich.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzuvsnkqt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gaurdfyny.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gbjvsvcyx.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/grmwzzgen.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gbqcofqoq.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/giadlqhcd.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gzlofmwsa.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/grgfibnqd.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gexbhvdpn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gikpsyiih.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gfffkrlea.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gwnaytogl.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gupevykhm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/ggxpmcikh.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gphytudmz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gxenxkvys.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gnfgxguzb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gekoyzqkh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gtcoxwglc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gnortxkoe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gnxaklytw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gyrzeuyqh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gppxkztto.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gfyjhsnnr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gvtolfuvh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/ggwakahzo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gbdaayuqh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gsehdoabb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gvjrjwjlw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gujonvhxm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gtelatwqk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/glzxoqplq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gajkcsteb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gtregitiu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gnmbirguk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gqetbxjve.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gdjhfecst.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gfguakibv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/ghxdxsujh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gqpnvcvgv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gidnlfvbo.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gzaxnnctl.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gacmqmhwu.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/ghnmijtva.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gwczarqvu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gwiafgvfp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gmoigganz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gvzuftvfh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/grfqduedn.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gomoqvnwm.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gbefmddgy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gcsdppcvc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gflzvvrci.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gtwaqlphb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gppphrnkf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/grsvflcij.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gtvrdheep.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gtxpzohrv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gkqaddabj.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gbviskkmg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/grbtupvfl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gbcgfgxgw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gcxwnbjap.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gkbnkdzbc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ggxvammzz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gfwzwmvmq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gkuvdzrvp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/grnrutzxf.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gyqjuxmfz.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gcnxxqkxd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwntjbrdc.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gynnxvxof.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gfzrdwpdh.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gdqmgdqlw.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/graagzicp.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gmrjlezea.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gcrwhjalg.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gfdlgcfgt.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gxcqtoibd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gpqogvvtw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gcikojncx.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gmqzhfwlk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gdhilkcbn.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gfpyjvkhm.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/grgutmfyb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gsbpzmmzd.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gvpmzkhap.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/glrxmeqtx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbabjlbft.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggchbzxna.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gvpjovkcv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gudbxmtqi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gdikzdhvi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkdxryfuf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gxchwmgts.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/guqnsfkep.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gkendwtvx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gfkdpcozf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gfnmnamtt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gnxjzglgf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/giumacivw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gtxymzick.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/glnoyabck.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/geikxzwbi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfmfhoryu.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/godgrbgvf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmvqghlfa.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gqgrlmexa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gksokvfgc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjdtdykxf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gcfuracue.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/glmiphreb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gbsmjxdmf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gepljmkrt.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmobzpbsf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gccqhahbv.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gnvyzuooc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/grpljysjf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gdifdsxbu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gvyyujsdt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gyteqjbix.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gfoqcmsnt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gdvoovedr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gylnwqynm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gqkutkidh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gfywfkdhc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gasvtrqgi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gftbysnsz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/govdfuuvt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gqwqxkjaf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gdqexqeey.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gsoickjdc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gqrzwjztg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/ghygavhgt.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gwjegecoz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gozotdgip.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/ghzhclaft.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gmvigrdrv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gfpfmxlze.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gjpuszqec.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gqijlwxvh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/goffbbxmf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gagkpjobq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gnidkdpqw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gwvqbrxpp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsfszheny.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyysmwyox.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkepshxij.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gwaudcqye.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gmrvwibqa.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfqgzidqa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpumatcax.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gnejxneby.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxauzexlh.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gubjklime.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxylgnlfv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goddllesf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gqxpxdnnj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcwskucvr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gngnuxmab.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggeepnvac.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gjvrqgshx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gtsqunmpo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtrhczidl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gtdfsannz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gvssrxtfe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gwxxbzsqw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gwnfmkbht.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gswlsoasw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gldkdlafp.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gjqblvesp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gzxjssfxf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gvulhqcou.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/grmiqerac.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gzgjpwplz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gijsxtzmn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/geydmlfng.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grkjtytzq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gejddxhfk.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gcecovaym.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwlblakat.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxplhywqf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gnneryfny.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gfdteuxig.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/grrlfkxoy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/geyukwhil.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfueirmpn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gpiljffqo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gbfkfqzij.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggllzwnrw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gqibdcxpd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqoqxgdhd.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gweawhozh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gntqvnfkn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghdexiejv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfcsygegf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goimscfun.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gjpggfwbx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gggwhhlla.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/giktqnsss.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbamzzmxc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gqewhplic.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gbmqzfndw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gwsbyshus.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnfuhwhum.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/goagmlrnr.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gmclfzhoc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gxwymjwzw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gspdwugqw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gzkxuctfr.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gzrqsgcmi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gfiddeftm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gynueuwyh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/grwutdvbg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gyrlfbopy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqukkvoxe.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gooedpfjy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkggrwpsv.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gatazbtst.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gmlmjhnnw.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmluwiokl.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/glgluwtuy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gvwwwilky.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gnfgjetrz.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gdegtbzoz.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/grnglzbor.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/geabhtucs.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gswfvaaox.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/ggtgubuxe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gxvpyvmlq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gfdzlocpc.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gwdwamtct.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gdeldyomf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gwnyyymjp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gmxyigfmp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gibvpzipz.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gbqbxuyqk.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gmrtyufse.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gpaamwjfw.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gcaffljdu.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqlwsqzdb.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gmrbpzjuq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/glcynkhku.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gnkowekho.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/glrxpnyaz.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/ggfywkict.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gnyizwbtd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/goaaagfmv.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gftowcvco.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gopsewqcs.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/geftvdyzo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gwpspoaxv.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gkwkhbegy.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/grfmzwlym.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gaefpbdxo.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/ghwfceogv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gppwwnyjk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gzkuhgdrj.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gipmzigwh.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gyvbzgght.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gscsnbirz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gafzmpurq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcchofxqh.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gpackwplt.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/glllxwpjk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfwcssiea.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gdfxveuji.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gjcttttto.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gofpalvlj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/guxcfzund.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gfgjhdvun.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gotspcpci.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gxracinby.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gwoawdnwc.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/ggqjytlvk.sHtML


<!-- 参考信息 -->