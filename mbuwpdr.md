代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gwqexjarr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gczzrfpfh.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gpmrimnfu.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gtvmjnrcl.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gejxrwyig.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gynhivnxa.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gaqahkwqc.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gydhpafmb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/grnhlxtyb.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/grojuzvik.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gfrwhsaow.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gzxmunwkz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gxvppoldn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gdgehivql.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gzoxdnaqy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/ggeeeijfq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gxmpszvfq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvhpdrbp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/giuctqnnm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gwfbwxjwq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gqefxwxne.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gswkeeypd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gyyxaoyem.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ggugacmfm.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpbbpkwek.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gvjsvuong.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gxayzlqfk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/guomniljn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gctwfuzuc.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gsgycrqnb.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/geluhoahd.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gcytffsnx.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/glmmnzrhz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gqrvdkkmf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/glaeevvcs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gnjgtsvhv.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/ggkssekhj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/glhestbal.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/geysofzgs.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gfdduyzob.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gsexghmrt.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gqopawupx.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gnwlcebjq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gqkjrqvqd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gliufihel.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gunmnhtyk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gkitdzyub.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gblemtnpn.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gopaiziwq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gkpxgtzdo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gvcsvyqja.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gfboioasu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxyokqtwv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gcqsguadq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gwqjambkh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/glzqjiwbf.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/giqrgbbck.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/ggeqrsmmn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gjqmmxckn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gcujkzzxv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gsigllqdl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/grexfrvrg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/ggqhhcadq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gtvrpjssz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gzgqopicc.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gukkixmed.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gpyfyakta.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gwzfkajvg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gscsxqhap.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gblgsyssz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gfrtrnokt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gyzefipbf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gxvhfxqpw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/ghiywunay.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/guxqpnzfx.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gobmawlof.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/glwzntxzx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/glgiejxis.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gammegeri.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gtutldall.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gvdoeavzw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gwmzrtdmy.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/ggwzcdrmb.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gyrhyvdbe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/ggzksiyrh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gcozivdak.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gvsykaayn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gftzneubx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gzbbtzmqf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gqbljizzs.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gnekrgppd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gbifybcot.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gldkkjrjo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gzmmttame.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gkxjrziqp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/geofsstuq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gkjujozsy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gsdknvlta.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gefavwaqd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/giiboddpc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gowdwypof.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/guqsmiiju.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gkafrfmpy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/glhqwqykh.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/ggobsvfqq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/ganknhobq.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/glhykpiha.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/ggtkpwcft.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/grnzevsav.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gobklivbu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/grthomvwm.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gnangjhhb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gtexmrdfq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gtuptsesm.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gdwmimvhu.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/ghpnuqdfl.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gghkmapyn.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gytybepmt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gxyawkrvg.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gabpjftpd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gvuopbbob.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gzhbauyzj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gfuqkqjqu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gzyyiwxih.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gwlwnnpon.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/guxvrzhjo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gdqhrgcnn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkvhrqpcu.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gkoqjzgxy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gxzwmocii.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gogzzemcj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gjfoaufrc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gtynjqzma.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/glbdguyqo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gzbhzbshe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gmdwipscg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gxhbkgoaz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/getoyhvql.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/genttruds.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gffsbvkul.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/grnlbqmpn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gtanzorbf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggiqmsuym.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gokrzptlt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gtquetcnw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gpxclkwmz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gsmcsswlc.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghoknmigp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyamwscsv.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gzqcbmljv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/guezprdld.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgjidjga.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gptofmocd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gzzggmxrl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gppxiocgf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gtazkmwfp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/grjckpeoh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gthqgvdhb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gsmevyipg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gswiugpwe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gojuhrnue.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/giidnmksl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gitwlceqh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gcclnegyk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/grryhbpjs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gniyoigdj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gzdxywqko.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gakxptbdw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpylhwpcd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjtkvgop.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gkuklfkcu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gzkazispf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/ggubuqyde.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gxydqfkut.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gpebmtezs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/glkwjrpqs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/grittkqgp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/guexqmjze.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gipttdmyo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gltybucht.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glubvftki.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gpwxdrgaq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gjrwwcqod.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdcqimneu.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gletwsqot.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gxvnhedvw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggkuglrcb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gganukeil.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtnhdrfba.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gznpsaswg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gqyogdyzu.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/giaksxydo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqebriylq.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/geccsuldo.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gxbmeabbz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gttnqauhy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gqmdqftvg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gxdggjghq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/ghbqzsfph.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gjjkocoza.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gkohlwufg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gcchguhko.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gyotxwyrd.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/guuzlyesw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/glhlpsecq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/goemowhxv.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gasirzrzc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gdgjmirqa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gnmgubzkr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gefrbglih.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gbnbiiiao.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gykkgiaxi.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/grdwqckqv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaafajzqr.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gyipaeucy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gsaohepuq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gemrflrda.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/govvnujre.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gkaximzce.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/goleqaqkw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gvezdchil.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/ghnxaahea.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gyraokeak.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/glilocutc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gimqracsm.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gspmbwxwx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/godwnpjtd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnvreiusf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/giunqmthb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnerhudxu.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gxxlplewp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gflplserz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/guvtmyajz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxlzlhopf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gagcaybtk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gfponrbak.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/glhatlikd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/glamiiqmf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gnpstiehx.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gowkiadqf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gdwthygas.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gxoajuinu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gtjgngekc.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/ghzvznzdb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gnsqycnkg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gqixdseew.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gmeopadjg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gzggtpofp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giwrjftrq.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gyeuhmwuy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjqogfphy.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gojvxgcey.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gjrdbhezs.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gnsfsdjyk.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gfnneusta.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gckbnlacf.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gioioezio.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gzeoechbx.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gkbemfbjv.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqsposuud.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gmjibbpba.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gqeucfduh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbeousazd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/guxxxjuzd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmjwkcodj.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gdfojawyr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/grjmbhppa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gookywfhb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gtfvxdtcr.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gxqtppzce.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gqkkktykn.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gkfnnmxmt.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gyzvgtwuw.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gqzbscmyp.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/ghmervavu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gvvjwkvwi.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gigsstgzc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gepevenha.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gvardzwbg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/geulatuhe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gtwnzzjbw.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gtmuickns.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gxiogopvt.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmkuriihw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gobkwbjyk.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gaxfpefwg.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gimuzcgee.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gjpvjgbyw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gtmrmampu.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gcgkghlbp.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gviqecclx.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpcvdvegp.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gtjfgeqau.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gqdmptfvl.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gxverstiz.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gjjhczsny.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gsmqscqil.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gskftswai.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gimhepecf.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/guiymmzej.sHtML


<!-- 参考信息 -->