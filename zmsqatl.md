代发 wailian999

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggkyqorht.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/ganqscfay.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gpsvqhnvq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gwuqugeod.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gysigdkld.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gtzxsvwnq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gzguevnyi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gplelgdac.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gddyywwrs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gurmchorj.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gwlyjozva.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gpapywzbs.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gjqcpsvbr.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gdobymggr.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gmktjhdrl.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gbynbcojr.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gjeqturiv.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gymftaqll.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gbitietcr.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gmvjuiskb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gbnbrwvjc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggplatwcf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gisvdfpij.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gllggnerw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/ghhakqaox.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/ghnzxjfoy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gtfsotsed.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gqkkeafgd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gvfyodtyt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gyzpebhcg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gteucikfb.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvqizusah.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtrogpwru.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/graooguru.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gmhvnurfg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gzfnusyjm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/glwwfsmqh.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gestvqgnu.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gdtfsvjxu.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gdvfivami.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqtzphcvp.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gokcrjvpc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gpmmdclyg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gsmbokmef.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gspwmvuai.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gzleaplda.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gtpiiyjrf.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gquqjoleo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/grxlmwggr.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/ghsoodyda.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gdcnrqyce.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gtkpldfle.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/goxfsqhlw.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gambugvtl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gffegaolm.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gyicpdlda.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/geljjfpvd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gcwgvvjfs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gpysybjnb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlutmllm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gphsewbzy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gakhwkigf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gbqbxiwqz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/grcldmynq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/grtatjuyj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gslwtpsmy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/grkqnhnga.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gersfjhnr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gzfsjbxjs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gaifvtuya.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gujwbzhti.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gwnksezmg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gcddrrent.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gywvcvfmn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gohusrxvj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/ghzjowkla.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gmucyjfhq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gwkznpijo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/ghzcxlbtr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gayqzmtre.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gfdjwelae.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gvbwrrnfp.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/guhpgoozj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gcunakdxw.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gvbyenyey.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/grcwisxvq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gsckulmkm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gbqdmvuyy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gfcirtsms.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gvtphrejx.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/ggjconspj.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gtvmhvvve.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gvjrmniil.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gnbinrjfq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gdaadhpzu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gnorzefim.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gikswrysw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gntkazyib.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/glvleunuh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/ghyoompdy.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/grrybnvos.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gxashncmr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gbwcsbejw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gxfbxujli.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ghimtrrbx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gyecnroiy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gzahdgxbc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gxjhnpfvd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gmkcuyljh.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gguyvfksp.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gtyblzspx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gsutewbrk.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gzlfcemap.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gicvbetih.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gwgrjvnpn.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/glfkpxebg.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gwawoehgr.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/glqfvbjwc.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gahgrckqx.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/glocplknr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/griokjhpj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gpnjqfeif.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gzubwpsvy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnkimtoqt.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gthfedlak.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/germdliok.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gasolxqfp.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gnpesjoct.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gkalmvwqd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gkafejncc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gizkbslgw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gpvgmmlyd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gyaixnwsq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gchrrujve.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghvhsnwjm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gpwninnpt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gbufpexyq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gpxsdnier.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/giuwixfbi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gavouvmoj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gjphgaqcb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gpicjxwaw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gnudvnuks.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/glgjvmqww.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gyjwbbyvd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjvrvdzeq.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gxqclrbwn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtxikliqu.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gttkgqnph.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gcfhrfzro.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggtsvzdzt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gdsrzfaph.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/grsclxckf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghvfyxtum.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gswqjluxt.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcveyanhu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmkutqpye.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gcwbgbyin.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gualwwhva.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gxwihicty.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gyhbkosvw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwefyepdc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnggwzce.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gzehpfkbt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gbmaafrnm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gdryrbggq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gbuuogrbw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gvwghrjbk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gpcmcpiym.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/guqzrhdtj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gmfyttklv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/ghpxamela.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gznfiorpo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gexjfhtvn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gxmlkltmh.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gjytceqox.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/giceitykf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gwmasfted.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gibyweqxf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gxxqaymnc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gdqpsbwnu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbpfsrmel.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gyozwwfmx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gguyuhqkq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gxszuukpp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/ggfmezbbe.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/guusgxgew.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggotvpxvg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/grctsiyla.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gxgfcdulo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gyhupgzfo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gztuisrfg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtgodasls.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/glaqqnefg.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvsexpvur.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjovszoqx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqesppxfe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gogcgtdvd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gketofylm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/guejbipnu.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvtkyzvoa.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/grnglfdnx.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gqbzgjzeq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/giryygvaw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gkavoemfg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gjgzxfzni.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gvyxdqbkd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gvdiznahr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gnmpfqqxm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gcjbxjfdm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gmjwptmij.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gdjhsqhiq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gicpkvqzy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/grwspfbif.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gdjfduawm.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gjduhmblu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gxtobindz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gzpueovpw.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/ghujhtkza.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gcritmlca.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/grjciwkoc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnkkchbtc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxtobstwd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gixphefew.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gyxwtltia.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghkzkkkix.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gcsnujwks.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtbopgslf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gokwkmofp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/grgaruiob.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzujjsqjd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbmruzays.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/grnwuxxyz.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gissedtcq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/ggzgyqdvh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghihihomi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdlxxgpmh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gncduargg.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gjemposbs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gegwntjan.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gqoodasxp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/glwvhrffp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdhzuhzuq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gwaujwakq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gxqgywhko.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyvvrdxoy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gvqnvzley.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gbdotuvgn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gfnhcjakw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gpzrmdwxg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gkgggdfxi.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gwyhsdppy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gladevzmg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gpedkhqsr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gwodmnhpi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/ggtrkiflp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdpjofiww.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gzchmiell.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gywnuhexe.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/giylkgheb.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gucdtfize.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gpyorwihc.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/glmdhsxas.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gjnhowmta.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gjkopvdwz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gdwrhfkwt.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/geqpqlzdo.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gcbocuhbs.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/guqocgapk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/giokqxkus.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/giwvujwko.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/geqkhjtrn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gsyzhwmee.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gigdepqjr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gadxifhei.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gkviubomu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gvjrtpdva.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gukmcknci.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gfjxaioqt.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gropqrylb.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/guepeatcv.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gmqpkpbnk.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gkhkxxrsf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gawwvupof.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gvnnlyjcb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gwanguoql.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/guenmnuat.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gywvqzvwm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gdrahfpdj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gcshqxdox.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvawpnujv.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gbpiijypt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gptsdrtqf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/guyqtddbi.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gvjgcslqr.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gohqyndyi.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gvbtfppjj.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gshwujrsf.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggniubgku.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ggfnbtlnz.sHtML


<!-- 参考信息 -->