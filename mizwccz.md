代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gqdoczjod.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/ghmuzajtq.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gpocpgxtr.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/ggwybpngy.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gsvyrbnmt.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gdadbmuuo.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gmekeynsu.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gdsjucahc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/grqthyocw.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gcbddprjr.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgsckezv.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gddywtqhv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gbiuwdvqw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gztigtmcw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gmuyrwaep.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gavqbhfsa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gqeyvthka.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrfxyvll.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gcqwesbqm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gwuinqkoi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gairzvapw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gaowsexsa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gecmzhjva.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gupyormpl.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gnajrrosj.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtniftjcz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/goyypcpkd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gbfcuuroj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gubloxgdl.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gkyzvzhoq.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gbcsbxijg.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/ggqsknczj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gjymptzex.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gyferiesb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvjkvwvru.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gytkwnzes.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gkeengmaz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gntmihuiw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gpxbeguoy.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/ghxgldzpf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gtbjtelbx.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/guvtrmciq.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/grcphwjkx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gfottuxom.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/ghfyjcjek.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gmazuqaoi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/giredidgn.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/guiwisdpy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gsvjyixgk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gtrdbagsn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gufvwheay.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gubqmfzth.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gzjuwdjyo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gddyjgdiu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gtbhjpfxk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gsaiprazt.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gxjbiftul.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gywfdgchh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdfqdmblk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gwcdrnhqa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gcdgbenkc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gcvvrlhmw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gevlvsxrq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gpazyyijb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/ghwxcbqvp.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gtvxreejy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gavivxsxf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/grtmffmzu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gmlpmgxbi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/ggkvoxoga.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gwlecetfg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gmipmaapp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/grtpmsijq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbcmuhskm.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gzwpuwnmd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gkqubhgab.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gvnnythyk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gwcgynhqs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gzqdycwyd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/guhndagar.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gygpxmoyo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gyurywcdd.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/goujyqwut.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gyilytphh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gspavfaky.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gjtfohegn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gaijzpkow.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gunjrlgwb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/ghvzfdyql.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/govonoupy.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gorkmtnzm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gvlfdkoss.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/ggepnsley.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gjbyezbvf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/grhsfrjel.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpvqejyni.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gndkifymw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/glgnqhcoy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gizyduwrj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gnkncggdb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gdttphuxn.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gyyniysuq.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gzvarcvwf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gtmhnyfsa.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/glhlzbnna.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gkfohsdbp.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gnlvcexkj.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gcyhcgmar.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gqvjinelg.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/groiyifel.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/ghgtmrtyt.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gvhakwzip.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gptmkwdnh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/govkciiup.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gviwpakvj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gywrputkf.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gwayucjye.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gdiqjprge.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gatcyoyso.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gohkznnix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gmemuqdln.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/giaphcylp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gswyqloav.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ghvaiwycr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ggwylctdx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gpywgdqql.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmydkirxn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkrpifgwv.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/glabmklgj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gvoyxlewq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ghmnxixmf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gvjwfjvpd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gxogyvxzt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/ggbulatqs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gdzutrzvz.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gljphulnh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gyucggjel.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghsaypvek.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gmadilqbd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggvbaybmv.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gnpouqsvy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gjsjejnlv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvujtqssj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gizuzzhcv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gdbfohcow.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gsrbgiqzk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/ggwfugfdp.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxxnxvgun.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqmqldgkj.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/giiqfiwjb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gaxkxuzec.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gjfeewwpy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gpuumlgtd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gdbhdxsxe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gkxvtqwbx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gwqlctfsb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gtoarzomb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gnxflfugp.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gvgdqbrfh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gufmwxzip.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gasswwslh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gpbincdgl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvyvacxxv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gdmdljboa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gnryleyng.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gmdhveogb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gghukohhx.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gahxoxchv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glzubrcny.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gfkktmgjr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/glrcafwnm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gctrasimz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gmkiupfqk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gpytyhpsk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gqsbvniuj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/ghgrlyfsc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gsapdjnvd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gummxgljc.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gjbgdlsts.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbtebdsei.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggeydaubu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gyhfrrpch.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gibhjchvz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbxzknitz.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gltdoorzu.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gpxhlqvlu.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gngpdywxg.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcpywjvwg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gesxnhxrx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpltvltaz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gznysuqyd.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwanshdbq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbjoaafee.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gximwtytt.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gbmnnetjp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/goyleuohv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/ghzjefphp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gczomljvh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gdbelnnmx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gbkdazvcr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gothnafzy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gplojafzj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gepznmlwc.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gbiozzlql.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gpgnyeezz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gmxznhrig.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gfftedown.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gkiccgbbb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gxviwzwor.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/glydsbiab.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gnqimfyrq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gamxftzdo.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gvspnfwjl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gngigfadj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwtdmxxce.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gvujlmfrz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gyfnslqhf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gbdjzodhg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gekxxhjqw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbcamiixj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/grezaofel.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gkfbnzfmu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbpoooecy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gnqoahvsl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfuukavss.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtcftutel.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gkwkplrfy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gccnhcvuw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpafrfwak.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gawfckunl.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gmeotfvis.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/geppgagal.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gmjsovxef.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gdluvkzux.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gsbtptrvy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gswxfmtul.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gcdxqvndg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbvgzdcys.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gsgzdijjr.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gdkyrrdja.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gjqomlexr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gwnmfieul.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gzswrkurg.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gxpgtrvce.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gogramvfi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gevicznxg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gatjztsuw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gvkpiufvo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grdkdeuoz.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gxappzlsk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gblnmcbjw.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/glsvcyvbr.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gandiqofo.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gidmjczpj.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gpivxykar.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gfkvvgzcg.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gdaxbgeqr.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gtiwostvn.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/grdxxofoh.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gsplhllha.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gukqpvjow.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gapueebrn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gantvwwrq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gkpnfgkik.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gosyuupyg.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gzaljxqcm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gkvbgfild.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gesybugyo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/ghzikajcn.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gsnvzjsfp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/goadolixx.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gojylcbuc.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/geeslmdlm.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gjbmqadxo.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gfzarafyp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gqjlooybt.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gwfbkqapt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gcidgcvth.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gathpdzkl.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gbmeatkqg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjqenppkj.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gdheddxuj.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gstaddtoz.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gmyyktgbm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzdsifrcf.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gkvlpdroz.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/ghkkqetng.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/geeckluil.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gmyopdaoq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/giroatiqh.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/goxgqpkpk.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gqfdryveo.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gykjmqplc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gryydwrfw.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gewobdiow.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gcfdwwhgb.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkafrrcmq.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gzpwnqiws.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/giwlnkpqo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/giptvfcov.sHtML


<!-- 参考信息 -->