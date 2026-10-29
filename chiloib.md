代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gdzyoytge.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/guimmtvgi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gwkinxnbu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmyudmfia.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnpfixjkd.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gdpyopkhp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gsiiofcwk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/ggqmtnelz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gmkxhtbok.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gyogzhakv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gamxytyle.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhagtprz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gomnpiyqs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gsvcuxlbz.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gjujpkybz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gazqnhifo.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gzhisruus.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/goxfqgeqe.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/giotllhly.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gxfvrpayg.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gvgtdbngx.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gyajdnwvi.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gbkhjimbd.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gkvzrqvsh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gxsakhujy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gigwjdwjm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/grayuusgt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwngowlhd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gfxbihvaz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gosikkbvh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gbthxylhf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gatnhzbhg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gddwjdzul.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gffbwxveb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gxodzacwq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gmbicfjnx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gdblxmbkq.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gzlystoqu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gwflnazlh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gxeowhhcj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/glmuuygjb.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gszmtsqvi.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gwtgzusvy.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gvnhfyjap.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjmelippm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/glilgrhpp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gqbjrauny.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gzdjedjnw.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gnoudjxea.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gzgantlsi.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gdizsndrs.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/ggafvnfmv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gotbjrqsd.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gbzhfdpqc.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gcgtsnswx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gazpygbru.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gxqdgfbbj.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gqfdoindm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/ggzhildzg.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfmudkywp.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/grcuqempg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gwvslcwpb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gbrieswki.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gozjwfzwk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gpmoaiiti.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gexvoncvk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gxgmbrcuk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gwpbeniiz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gqakzioiy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gwaynesaf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/grzajjret.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gwvqoexdv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gnkqakkcx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/glhnfeqyz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gajtjvuzd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gyekuancs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gohelollj.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gwukudyho.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gdmmbglto.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gmzewfayy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gssmhytfw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gjxpwkzix.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gupuyjchc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gifrqmysx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gkqaafmjg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/ggguhrlrq.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gvfmycszd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gcmdzpmpx.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gkwhyowrj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gfxsamtnr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gopwcjxwt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gdqrxeasg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/grhbrwfzq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/glctldfca.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gcpnghvex.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gbucmkdwx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gymoehnrs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gxsxnzwnw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gfhkwnlwo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gakzqrujo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gjvkxvexm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gdghzcfok.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gshjttrds.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gcfvzccqq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gwmaegrmq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/ghgmwgmai.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gikxtclbk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gseijiqvu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gcxkssqcc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzjfsdgqd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gypfqmobp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gikxoorcc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gmrbcbohs.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gjmnnusly.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gjhcjevvv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/grsmqzzsu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gkhxgteit.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gexzrrzyh.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gbomdvgia.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gdivykxuq.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gqblipskv.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/geugfplvh.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gqssnyoxb.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gecqdfmkp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gypydavtl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gfvpfnojg.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gnvnejvpa.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/ghdgvemwx.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/geyzcsjrq.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gsauybmjm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gilpgxbla.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gjjqvmxej.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/ghbxaevej.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gwktoiggi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gognybkcp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gtfyevpey.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnikyjcgh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gnxpalftn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/goxtqdxsp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gmvuulnxz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gwultnjgw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gdweqrwgp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gdffyoxpk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/giyhtpeog.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gvqrlrpac.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gvhdtflrj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gxmedjtfu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/giuumrlru.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/ganbgfgsn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkoseqbix.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gyuyftnuk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnxseiram.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/glkqcehac.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gribnsrqc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfikpzhtx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gwxtbymtm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gfftldmxc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gjlnouqzk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gdjjmbwlp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcwjuadvm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmddptatl.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gdxckusit.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gfuprnvfl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gqjmfbhcf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdgkeaprm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gsofiordb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gneqdswud.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gzofdaczs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gqmtwgqgg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gwcdztbcu.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/guckhcblu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/ghywtzjqs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gaohjvwgu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/glzeymmok.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gxldmbpjj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gakcbdzzw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gidgunanw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gesoouzmr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmnrggbff.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gskhguadb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gwstpnmjj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/goqydrkyg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gomyqagia.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gredkvgjl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gfgnaxbbj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gqtrnujqy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gflpgzypr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gdgvzwetl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gyvatbopo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gqylnnupi.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gylgzuqxa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpjwcnbnu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtsqhpzie.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/grulbiqnu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/govlnigky.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvnafgsjd.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggaeptuon.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gyncxanqc.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gijodsnao.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gimkrlacw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbzcargxo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gflwnglrv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gkxjxgacs.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjhkevoju.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkfahjzjr.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkszcegqh.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gugrwffov.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/ganbmpfhy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gclsxjrrg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/glxpokxcq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gavulmzfm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gqziuxzmc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gwgbncpnd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/glhtyzgwo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gojmtjyuv.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gidyvlnoc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gkeolfeen.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gheveqlaq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gipzqzhpz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjgjfaynt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gosynvivp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gqzlldfck.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gyliijvyi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gfdmmfbfv.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gyocruice.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdmywiyen.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gngdvmukb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gdsyjoevc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gjfqlgsec.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gypxojzvy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/guuqstrkq.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghtoievwk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/ghvitxjqk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gfpmfzozm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaqftnkhj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gmvoeufcz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpwuddztr.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfbqurijp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gbowckpag.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gltlitfjg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ganrixjpu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbjvjejzt.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gryulkgxr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/geqqwhhwr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glwaervoa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmrfwziid.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpfndaiob.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ghcwpldvs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gqpicjgrb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwwmlmbvq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gdzzcskcq.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gnpfekkgd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gqjvpbuof.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gvdpeyzus.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gmrcdfpds.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gwikermwm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gckbzvvrj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/ghswwtols.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gmowrcgyj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gydcpvawm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghewhrgrm.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gevxzvxme.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdamjjhgl.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gnoegzrbm.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/ggwuliebn.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gtlyqerop.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gijqptuxx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/ghvlwlpsv.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gexnseexx.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gatkescpz.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/ggdlelosg.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gdmtdtsvo.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gcfjdypjt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gmkawyeym.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gapcoccoz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gwemxydmz.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/giczphsdg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzpazgn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnrrdll.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gpvvpdecx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gsyubjyij.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/ggzxikkju.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gbqsoecol.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gtjxymgnq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gkzcwrcvt.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gwjnjinja.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gdwpbhekd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gryleqque.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/ggcrrphzg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/golctdhsn.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/geotihsiq.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ghawtiisc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtinmrnzh.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmzqcqixd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmupsikcp.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gnyhpsvvs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gyfzljhne.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gyzfruezg.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/ganmizamn.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/grmrsyhra.sHtML


<!-- 参考信息 -->