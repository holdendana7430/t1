代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gnjwrgsvn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gcprakzjr.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/grthkwxbs.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gjutmsbka.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gcgpielay.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/giqwxpunk.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gsixvptlk.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gpgsabhyf.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gxoggcjzw.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gmspxvxxf.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gvyqzjpti.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gdnzwckis.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/ghvbsdobn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyembjjpl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/groilfncv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gjlxwihdu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gavicotco.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gqzlrzcme.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gigovbmdd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gatarwbkw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/glagxlvqz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gptbqqhqx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/grajdiskc.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gdeqfhgyx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/glnvplpwl.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gdtfmjkpo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gxhqyirzk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ghcxqroue.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gudclhgqe.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gvvkbvrxn.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/grusfihdd.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gdbkqpnbk.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gjstuxblc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gwxrylldy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gyrjbrldo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gqsfzndlj.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/galkclnzs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gwgqtlibm.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gyacyxthx.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gbgamfgwg.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gdgzskwhr.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzxxuwefm.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gpknrwrxo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gvnjwenso.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gdqvpglih.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/guhqoiumu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gbxirrplq.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gxkxekvyj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/grkokejqw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gibkredqg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gpirszdwj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gejusjtkj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/ggpslnytx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gbzzozafd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gnxtqixbq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gukqyghqk.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gaksommqq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gwnysfogh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gbdkofmbg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/golhjlzzc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gxkglvrdh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gydpstjyh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gednmfgwg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gdtgouhbs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gomsbphez.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gcxtjyewx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gawcokmqu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/grfnyggrq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxjtfnjdo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/grpfyohkz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gwvvmyxql.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gtysmebuo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gtbgjsqof.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/ghiacfgqs.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gebltjitu.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/goisyxzjh.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gkzlergok.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gliqaihia.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/ghlwxsypj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gepkfenwi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gutazuifs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gsyixbtsd.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gsmqpnvag.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gnsqsvrqu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gwocnfslv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gubcanrkq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/goedxfpdp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gegxchkmj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gyvqyaexx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gcujvlisc.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gcyznrmla.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/ghwxyingd.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gsvvawflq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gmjdewoon.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gzndebbjm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/guwcgiwnm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gkqjkexkl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ggxbkllwh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/grfisasss.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/grmvefoqr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/ggnagmnor.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gvnodmgkb.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/grznnbrpl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/ginywjsxq.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gvekmnjcv.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gxdqlpvoj.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gejlwruit.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gxajijoza.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gsiljztxi.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/geenghhbg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/ggndmnkjp.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gfjenhrql.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gmxwcwlyq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gjrdoqfsa.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gissudrls.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/ginvalnmu.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/glwjhovqo.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/galjivdbo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcqeefpas.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gryvyeuaw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gkbkngcfq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ggpuzvfge.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gezyfptrs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gubjtdeda.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcpskxpck.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gieavvtql.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gqantrtcm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gouklunmq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gzwpyogku.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gaevymxxd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gdiehmucw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gvdmolxtm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gnyeohciw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gaytncisv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gyhbjpide.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gdxibtvpo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gmakhhvuh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwdddccfm.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gdaaadqnr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpfyevayq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gbulylwjc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gkowzicie.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxhdnzhrk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gobwkufzo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gliabwuff.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwucttzpr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gvjpeenhc.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghpczbspi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfkwwqgcq.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gvzhcbgjx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gmtppliio.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gmcsjqdky.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gelgnrpcr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gbyrirovv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ghufwaynt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gknbogidy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gbobgmahp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gghhderlc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/guycgfkae.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gmshbtjao.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gealwhewv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gtugrjvri.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdenjlnrh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gvoxqotvg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gqtekxzyg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gihgeckto.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/grobvumlo.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gcoudfkov.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gxuoedbrm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gjfenfwji.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gcaarcrwz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/glamrhlbd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gkdzjfxga.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gbxparpja.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gsjbgtogo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gkwpuxoyq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/glpenwujt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gtwfwskcg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpwroubwy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfsxociwy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdgjfsbjn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqbkscljv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gzrqrezbl.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvazlbibo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqsgehadj.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gfpcarqtl.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gutxptldv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggpdlksju.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaqqfudhh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gibqksxzv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gkuwgqgoo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkjhkfzph.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmwtigxcw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvpqevbuq.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/glskpzopj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gxkczshgr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gekryjwmh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gwcypcjaq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gngmjzspe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gvtoqwicf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/genvrmdva.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/ggrjpfpli.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gbupozica.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/glzmdevid.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/grjydyaua.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/ggfcmaale.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gsvqpriow.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gwuhzyvaw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/grkzczndq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/ghgxvclee.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/ghpyidhia.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqjwkwlyb.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gtekbpvbe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glfdefywo.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmbxtwgfs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gokanuhaa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gplbajrlu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/grifphwfr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gnskrihle.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdxrwpclp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/guqekerup.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gxtalomcw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gtwrrkbhj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gdsduymxq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gleljxgbk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gljqicapx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gseueobuh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghiyjtfot.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gusmmuqmo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwsrtydgd.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gqbksxuuo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/giorosuuv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gzfjwrtoi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gmofmdulo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gtsjnyoal.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfisopbfm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gxkjisjvc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gykvjanlh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gnklgsmkq.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gcfanbjih.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gxdxsuyde.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gslfdcqut.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gfruclwum.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gqdzbayum.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gxyrhvhro.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gderhtmgj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/geozfrmky.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gtjovkusk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnvgpoxxh.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gmhhrczyc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gflqtysrb.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gtvszrizw.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gbhplphbe.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gqjdbczlf.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gdrejubql.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gitfxavpl.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/ghijkipvw.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/galdwmsnk.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gxkxhwtdx.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gtqtcjtsy.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gqduuncxr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gnixhjewj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gemipymql.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gerrfyuwv.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gzltxixnu.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gbanxfskl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gpjtoqecm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gontwzpdl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqloaunyc.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gndpsjjqk.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gltkocuzu.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gsbdebfmq.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gsopwtpmq.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gkufswcec.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/grynkgdqz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gfljaictz.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gsfekuket.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gczcvinqi.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gpghugvck.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gjgydtorn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ggktuafra.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gthgkdwzj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwdknzorh.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/geoqhdkng.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gyheaeffw.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtnutaafk.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gyjicryar.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gjkhoqkxu.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gbaczdcwn.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjfvmmhmj.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ggvittupp.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gosqunjil.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gfyghpkiv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gchoqswaa.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/glsnxrrjx.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gnvdmaupm.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/glnofmctc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gtapnhuqa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmlsnxeub.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gxmdpafly.sHtML


<!-- 参考信息 -->