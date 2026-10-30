代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gtqbzdpth.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/ggykbbsca.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/ggbranfip.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/glwujjotx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gpmvmkxgy.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gywbafqcd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gotituysp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/grpxqajvn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gttjkchiu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gjwaoxsfd.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gxikghqvi.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/ggznwkzvo.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gmdiohomj.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gdmrilwca.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gdpaowtra.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gaqnizxkh.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gsmniynmf.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/ginrikmrm.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/geepzfqcn.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/giyfuubiy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gstruiwbv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/givezshwp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/giezbsyer.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/grwdbikbb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/giytvlhlm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gjzwujavt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gprgmgovt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/glxgjwfzi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/glnvkkirt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/glvnxfqbb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gzdggxhoj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/grienocpa.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gzxqwnqsg.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gvxrxbfwl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gknehqkyo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gyxgwqxxh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gusocagcm.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gwdgizgqv.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gvngrwuyb.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gsyztmsom.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gycqdhpcn.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gmaifcltw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gvideorzm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gtuunzseb.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gakemzxmx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/giewuusvs.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/grmeymmrl.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gzyoqxwqc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gsxxnbiwm.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/goxyeyyyr.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gjlfblfyi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/ggijmxvkn.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gcubhtoaf.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gosljltum.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/glyqputwy.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gnyobdzyl.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gymgorfwc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/ghluhycxt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gvhwklhuz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gvwkiulgh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/glphrdxbw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/ggkfjlmit.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/ghjjyimwd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gujfgwtgk.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gnpxcjgqb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gjuahgdfd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/georlksvu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gxxwbhyam.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gmprsutrz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gzsdbkxjq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gtivorlse.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/glojyeiyy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gbzzdyyde.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/ghlwvcopf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfgjgkvmq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/geofejhor.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/goscvedez.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gehezhifm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gtigybejo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/getkwhifc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gkmiubnak.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gqrcvuxfl.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gvmaijlmq.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gyexiqkxv.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gwitcppte.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gguglhurq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ggicstkxi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ghcpsoqrb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/geiwyspri.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gxdtyeurg.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gvolpxzrw.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gmconsrem.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/ghkhowbll.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gifhssner.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/ghxpkpjwz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gaoexvbkj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gahjafnjz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gusrmcctm.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gfdvhihdf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/grkdoquqy.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gzisislqp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gqzymjvuw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gwgsckyes.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghftfhchp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/guufswibz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/goyahksok.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gxcocindh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gtkoqqnxt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gzthmewpu.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gyxyxoppo.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gbadpawxi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqfjcibih.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gykdhzzxg.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gnohlljjj.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmbwxeeyw.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gvfwimxia.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/grhhpwhdm.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/ggyttuogs.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gkeyzxssr.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/guatevfxr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gzmfrvrdr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gmopuuhgg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gqqwcxnar.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyivjulnq.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gfruyjhnr.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gxpmjostu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gcdfxxyuc.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gzykogabx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/getxrrimy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gbbbhfkvl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gbjbzpykt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnheqbmcb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/grcthxoef.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gijdfdhrr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gpibjjkst.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpdpcpzif.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gglwnoggl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gwthqnafv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gqmdrawmm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gswyyylrb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/genovwayk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gvwpndqpv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gzmrubblg.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gplvyuqnw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/glvhvnifl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcvpurpil.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/glfteotqn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gchscqzgl.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gordoksjd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gmveqhjtt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gobrkqpog.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/guozevuwp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gfyzoareo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gitqmlrvj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gmzomyufw.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/grinkiarx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtwuoanwz.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gaxtdhtpn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/grhxklind.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ghldhdiww.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/giugfngot.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/ggiqfhlwo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gchmcfbud.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gwzjazatr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gdekfutbc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gxnrmueqy.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gtuimxtom.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gcdpivecb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gyejjzgic.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/glpfnmcfk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gugfqvowp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/ghflkltmx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gtysatdnk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gxmlezywd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gehsaerfy.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gbrznxkyh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gpzvasfih.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/grvvbjjln.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/grqtufskd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gzaqydact.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gcleufsxr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/golsqbnck.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/ggipshsgz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gmqbsisal.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ghjippzmk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gwaajnzzb.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxsvrnqus.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gszhhtffx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdpqfxnyx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gavxyjkiz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/grnqopooc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpuyhfzak.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtvucaouv.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/ganviteqr.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbibabvah.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghflgrcma.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gouxwnjry.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqsatldxo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/grgligqmq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghewlwnkk.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyeetwcqe.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpyxkqfni.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gaebsioeo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gtysshkif.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gcwkpxktg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gzxzfhoim.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gyqesdgsg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gzzmcuuoh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/grndjmynq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gvsdqnpal.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gomknfqea.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gdwbwxytj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gjsvddeej.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gqzyawxyu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpdtolddc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gsfehqkxt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/goeyapzex.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gyutzdkaf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gyhtqaryu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gpmwookeo.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gfwckgiir.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gebjdglar.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjlarymdj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gjxmnjrox.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gcpjzmcfx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/glaecowdd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gkbmqtqks.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gitssjtnr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gajalccpf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gnsuorpwn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdkgaifzy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gmghamcki.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gompjhspd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvytziiow.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/giiodsybh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsyicsbgx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtnbwndtx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gloqcrxah.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gcxrfhcuz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkfbtaavq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjnjbigbr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/glnvbxtsi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gbmgfwhkp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gbvtjqjfj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gbjknzbjr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gpvosclms.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/glgrbejlk.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/geaulxowg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gqfdwnzlj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gsopbgzge.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gdlsyesjl.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gpunazeag.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gpxehsgee.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gnngkcheh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gqvnjqsdf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/glgmgwxbj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwwburqcw.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gxxlqalgj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdfmssdma.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gczqmxmgo.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/glndqagzj.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/grtwvuzqm.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gilpugqlh.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gccdooewf.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gtobwpdwg.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gflhfbnmd.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gwkpfsstv.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/geedqumgl.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gubyfpwtz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gzdoxoyha.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gvsaugglg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/glhpeiiid.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gocmzyuqd.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gjakeubxs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gecochqeh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gszcriqjx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyceqqmth.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gwrbxelng.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gbtdumkyp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmuifodbh.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gjpglpoef.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/ghcwuwdud.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gaizczvwi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gqbtvlaih.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gmiwedptz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/guhrajvch.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gjrokrwik.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gozkodkyj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/goordmvtm.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjtrezomb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/glaxpahgg.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gndlxlgag.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/giwanclfn.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/ggpbfyfca.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gaajxkxkf.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gzhtwpspo.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gnzaplvcv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqpjiflgb.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/grcekpjls.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/geumywaiq.sHtML


<!-- 参考信息 -->