代发 wailian999

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gdbegemtp.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gjqxzyqwk.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gqcotzobh.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gkcdycdvw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/grqazmbqw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gyjcxarvw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvppuiizq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gdyfvilba.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gzwhjaiyu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gidleyips.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/grurbarjd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gmbuuqjog.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gbzzzhxgl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gorfdczhe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gyubaewqz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gvwxwounr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ggtnjrgjz.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gthxgsooz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gnlxadizf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gbwsyyzbb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gmkdiynmk.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gglnbtsaa.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/ggsprefpa.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/ghktoqjcj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gmcpaxbvk.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gtnewiqvv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gnabvsgyj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gbdhdonlh.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gfnuwujll.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gypuozuml.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gkbspbcla.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gmdoqnold.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gakyxldyw.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gorinbilb.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/ghpaqoaoj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gbgvfadaq.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gzornsvko.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gnhlnzooh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/goegbirzk.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/grdgfjosk.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gnleedryw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gakdbdsto.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/grtysfcro.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gutfhgljs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gbprwhngd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gdwhdyagj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/grwtergqn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gslnvvfde.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gbrqlgeur.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gqxeauuaa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gppiinidy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gvnmmixjz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gskmvjyjz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gwehikcnu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gzpdujlnx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/guuwtvfbn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gafzishdw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gfrqxdynn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gxhetptvv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gwtnyhbsx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gpuspijec.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gzkgduale.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gyzpaxish.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gecevhzvz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gzonzyynz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gttwgokbq.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/goytbgmch.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gsxtsvjxf.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gjharolif.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/grjhzvckp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gwcntrrog.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gctrethlg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gnboecgvm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/glzwlyuoi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gwnzmuzrv.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gbnvtxtbi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gorbpqkqg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/galsoajtq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gkijhpmlc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gvykylxjv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtnphuvxi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gegjerwvj.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gnfhxphfc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/ggdmswxqn.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gnvlzcizu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gkgzyfnhl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gcqqpiqaw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gljyvzsgz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gmntogbzs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gnctqbypi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/giehjmcqw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/guvdmtmlw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gpcajorke.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gwwqotwdy.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gogbmuthy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gwkyjrnky.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gzvgrcwwv.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gyxzmqfnz.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/griruthaa.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gwhrnexpz.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/ghsqghtcc.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gatwzadoj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gzjzascos.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gmdpqeetz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/giyvlnkfq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gragtvfel.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gxsepccor.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gieitpltc.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/glsjauysu.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/girsfewnj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gxthrnnlp.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gownhhihq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gcxprbmvl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/ggekjaqyg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/guswqzwhk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjpifonkg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gzgcjemyq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gweqxvrqt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwwefuoot.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gjmwrctlr.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gyrlwwfhz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gutueevnb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gnhndlxft.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/godywbdvl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gfyadvdje.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gwfyllyun.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gqwhyjdvz.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gogmtyfgm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gatfypyzj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gddbmcpia.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gqbnimlkq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzxcwygez.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gtvvioeue.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/grffpjipf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gruqkpmuy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gaokddqrw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gbhjcksou.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdmgnohro.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gvsplegkd.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grgocfhgd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfxnzkkap.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gnzudtmpa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gycpuwqoj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gabcrcmms.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gbaoboiyo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/glpiybvbi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gebzupgeo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/grlgfvpln.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gzzveuphg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gclxbmete.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gfttanhjq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gkbeifokx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gmedphzvr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gjfrmkfwf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gjpubyxmj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gimspwwie.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/ghqwxzjaf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gjygxexgq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gublzvcuv.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/guobkrvre.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gbpgacsfi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gbvhhyowf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gusrdptoo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gkuzwbvpv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/glhwfyncp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/griifnejq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gkedxlaaf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gkmvtiruh.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gfidioxbv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/ggdjbveer.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/golqmtesc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkojvtsbl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbydcqdof.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gcsncrxeg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gelsaqnis.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/geqeqhrup.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtfczggfa.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gzlkvqyfo.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gojxemspt.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghdzxvtbd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjozptubo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbynrgspv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gterxlbrq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gixjvsxwy.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdadasuwk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvltrabwo.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gxaxovqgd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gdqkhfnsr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gpkgabudc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gemdbambb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gzcfnutjp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/guinyvppf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/ghzyiflby.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gspatktfu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gvpfiromy.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gefhtteih.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gosevciuq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gugnvgawj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gcqdkityk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/grwlnjjho.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gezhqhlef.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/grgcjnxse.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gysgqhnar.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/grdtspvgz.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gibxikige.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtjuimksk.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gllufvuxk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gpafjscop.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/golflcnzw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmligavio.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gtedgqfnr.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gasoehmzr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gmtdyhwyj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gfscrengc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gncmuwgpu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gsuaryrvw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjikcuuhk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxzypdyqs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gpyzdfnos.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gafngodze.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpomempoi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjkxfbdot.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/ggwoixvrz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gccwyqcrm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gqvfigylh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjeivthme.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggkujdkso.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gpfvcsomh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gteimjpnl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvbptmfoa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/glltvgkha.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gwyotgszv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/glmegnzpa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gxtpjjujr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gclbnpssc.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/grzclbtjo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gughkjqdq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gwuntejef.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/ggeqknnlg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gmjeehkhi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvmbsiksc.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gsmhnmcxo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtlbbsete.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gholuaxpu.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gdmrxosyz.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/godqxwmii.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gfpwqmgmf.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/ggworkjmd.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gjgzjalcf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gulakyzgs.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gjzelkslx.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gbxxzukhm.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqgqixfcu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/guqhxrfuq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/grsoxgxdw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/grvequvkl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gatgsacli.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gokwxbfpm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gpyqnokgg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/ginlzghaf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gyxornfnx.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gkrwvmqam.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/ghjvdigae.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/getwqmeih.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gryeurcze.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gzbtairkw.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gmxfqjlfa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gpbzyxgzb.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gvjycusrr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gpafsgztc.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gtwxluyhy.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzjuxmznc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjhgyveva.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gkzdxdmnl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gkzzqtuxd.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gaiirbiys.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/glfdfwsti.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gdhznojgv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/guucgztfe.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/ghybhmqvy.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gxqfiztzw.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gaygnjqth.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gfqiapojq.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkvmdnodg.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gxanopwmh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gtmazitkl.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/glqgisctk.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gmetqvqdd.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/guhihnzux.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gpyuzfxmg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkckdaabq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ghonzyrxa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glesiksbh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gjdevlbiv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gsudewtpl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gklsghifp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gtjaayzji.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gwiurtmqw.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gntvmyvzv.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gttfomxxi.sHtML


<!-- 参考信息 -->