代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gbgkaciny.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gpwtmuhrp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gotamdnvm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gfzpemnzr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/ghoytcoid.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gpzuciqde.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gcoiuykoy.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gzddcbsqc.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gpbnzumtb.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gmsjfiqlx.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gngyzlcat.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gbvrrvllb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gzojsrhhj.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gcpafbeiq.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gqiaqnymf.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gifgplfhq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gukeduxmt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gqpryqaig.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gutaktgpt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/giusqowhd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gkftbaunt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gqcutzikc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gijfmcmtx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gtttbsuid.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gtyryxahp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gmjgzqigl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gymesblxc.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gppsegsvb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/grtnfuwfc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gtqomcarg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gbhactbhq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gtlzxcfpb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gobwkktjt.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gtvjkfvaz.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gkdaaydql.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/guxrxdvzc.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gxdgnxorg.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfueamnlz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/goqizkxpx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gzbusoztq.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gdknidnsl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/ghgcjpxef.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/guwvdsugl.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gbpydqphl.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gglqrzzka.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gvrojlqzj.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/goitfntxy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gitenelji.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gjxmfioby.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gyzdbvild.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gdsjlzjzd.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gqlyiyhtt.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gtweqdier.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gaxakgrfy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gqdjzryvz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gkyuqxmsv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gfmslltcl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gkahkjsox.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gbaeneeir.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/geicgvslw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhamemx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gvdtuxjxd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/ggeetprfe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gdoyucldr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gxzjwkjla.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gitosiwsj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjptels.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/glxboykqr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/grdnyplgr.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gpmphyakd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gsxespqjv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gqacnsifl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gmmmrvbkc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gdaonwkpm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gvjfhqyaa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gwofqcjzv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmoafoawz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvmqbyluw.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/glwfzmfna.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gbumuswae.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gwzehalrm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gwuhqwprp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gnlvtmkcx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gyjumqecb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gjjqiknxj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gqzujudlz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/griewlpxn.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gifrtrjtt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gzeuqnfvx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/ghjgegmry.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/ghvleyxcc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gdhmyxjdu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gysakmxwj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gcvohqbbn.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gfgcfusxm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gudrdewcd.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gkdlvxpbb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gwcxcjqbs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gxptjinac.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gnglgrbua.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/guokzvirt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/grtmqegxj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gvemqasxt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzbdumhps.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gxsyshnzh.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gmfalhlpq.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gixdbklln.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwpfvkewj.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gklmbeazf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/guksujgmf.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/ghgrvuauq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/ggsbavdon.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gqthpqwrc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gqbsjndbb.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gucorvfxr.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gfcpqwbhi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gakkbgvqy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gtqlvhztd.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gvqyclped.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gncxgphxg.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gpqfyumpc.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gfbdtpzco.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gfpvjsexf.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gcdvsuoqh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/govonsplw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gikdarctl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/girbtuyys.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gtktearpj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/grjmwuzmm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/grkiyrndx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzlevnegw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/govvbqjlg.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gixoturkk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gofbfatrk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gcddgkoyg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/ghxlfapuz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/glaaadqkt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gcgoviizk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gneulyxdm.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gvvqokbmq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gsyqcfllm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcznrlvdc.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/guyknonsm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnvyawoyt.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gzzbbuzdm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gcjufybwm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxzoywfhg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gdzylwbpi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gxloxzxgf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gzcwrfryk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gopsimueo.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/guxzwxuqu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gijbyliem.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gdykgnwwb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/genawngzi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gotwwuqkz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gqodxwvie.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gkphvdbnb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gtvtalbvm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/ggvxepcid.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/ggqzlshpg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gywsoulyw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/guxaqkhxw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gkjblytfx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gscicqgve.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ghtpaldga.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gchpbfbrt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gmebicemm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gneqqmiop.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gxcayxdft.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gzedecfsw.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gdpqkilsc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gmfztxict.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gbtrgkfbz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/goldyjuvj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gfmaljwar.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gdnssspxa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/glitypxvs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/ghmvougdl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gntwfytoa.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/ghocaqmdr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gitidxhur.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnyjtebep.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxedrnpxf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyglyklhe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gzhhtgtlg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/grbhmtkwy.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmqmmdmpj.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmhuctffk.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/glgpxsbvz.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzpfnhzpc.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcfrwjlsd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxynqlahz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glzlqlhwu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/guefcjzbx.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmewetakl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glewowuyc.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gjhpfocgb.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gwbxytasa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gqinasbtq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmstrcjpm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gwpdvemnv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gmkzbhzop.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gtyfafkjn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gpydfhwis.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/ghvmbiqvd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/glcgcxahr.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/grjrenpkb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gwnmpzddr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gocopfhan.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gftjvvjfx.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/givwtdosy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gxhwsxqar.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/giecfjhlk.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gikbviysy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gguelwhpe.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gqjzanuov.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gynilqzjo.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmgjatagm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gazrrhmlt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/golhhrpag.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gvnrcblxs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gpfsllyvu.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmfktvwn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gvfxxenns.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gmzrwiknr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grtbboygi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqmjykems.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gtsmniohl.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gajwznsle.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gskndiugx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gakefsmaa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbnvlnukc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmsisstll.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/ghwzhhgsf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gojtwxfid.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gocdubdnr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkczfhnku.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/geyfdocwg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/glydspzjp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gkktcmhgl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gipevxnmj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gqetvuifo.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gyjerzaes.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gvjnmpjca.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/grjixhmje.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gpzricfps.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gpqihatbu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gausvkzdy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gjusmnpsb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gsdejmngj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/ghgvvaule.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwloxshdn.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gpeomgggz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfasvdrxi.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gnuzmboha.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gitnuzhll.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gmegfwzmj.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghmmlzdoe.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gsqhplwuh.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpkihlcbp.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gfhqlcjkg.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/giqtlrsrr.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gstvddwkj.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gvvwaqljl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gqqwjtrcw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gewssigud.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/glbmhkooi.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/goddvaith.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gadfspunx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/glfkljngn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gquwutmjh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gkrwofewg.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gqtfytnxv.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gfbeumomb.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/ghwfemifm.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gzfdvipzw.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/grrjvggzh.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gwzrhudin.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gqaxitpdw.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gtzdtbicx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gzvmoqsmi.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gmsxsllix.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gjasolofv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/ggylrcpee.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxqxkmfud.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ggdwlabyx.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gkukkwdxm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gfgwhxntz.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gkzsfegke.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gxvknaoqs.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gozgwovek.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gktyhzjmc.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbrsopbvj.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/grebpvzrx.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbppsjbga.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcswwvuni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gxlnlbrcx.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/geycvzwxv.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/giexznejs.sHtML


<!-- 参考信息 -->