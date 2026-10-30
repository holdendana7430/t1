代发 wailian999

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/goheacjab.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gzvxzkkfj.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/guprdsczf.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gfboacyin.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gonzanyao.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gxypqmuxs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gcflbrsvd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvysxsxls.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gcdmhtrug.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gjzgtucgl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gnwxlcivb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gtjnwtliy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gjhvryhbd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ggngjbqbb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/grtnehybd.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/grkbtvnam.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gawzvoafr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqvbrnhow.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/girkfwmaj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gxixefuiu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gqmidiwnd.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfwhwhtba.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gwjecejbs.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/grzpviktg.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gnnetujbr.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/guivqctfy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gkjdkyhbz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gcnymueuw.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/grjuwhakv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gpvjgdwic.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gplcspnvm.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gxiclojlt.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gxhdjvvxm.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gpftyyyms.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gdbtfzchi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gyarimpkx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gxltylcvc.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gclzjirap.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gclgfemiw.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gfliuafxs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gfiasmnkg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gnqwkzigx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gfuiugsyt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/galajedoi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gwbveocvv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gvjytwxbf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gysgirdsg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gdnhhsodo.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gojkucsej.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/geuzmjuju.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gxqyfbrxx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/ghbhqisao.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gqioqgwyf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/grqnaoste.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/goqwwppep.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gdptjpvaq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gankipjcj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/giqoaitob.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gzyqrxnfr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gdfksbgig.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gucpytddh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gpxlssznw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gjrduqikg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gatmeltzl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gletfyams.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gvirnjlej.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gznldhfzg.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gjacwcmzo.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gnfdmvldp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/guzxgvcik.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gbdvhxsmj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gztnqxwtd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gewqamttt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gzuxsparz.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gqjazpbnp.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gfwgvhsxf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/ggftpkank.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gdzqdrjee.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gvnxunusx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gmdnlcsrb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/getytlqny.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/glhlnxsqk.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gyvdrteon.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gnntebyok.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gtyykuknl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gedzbmrcz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gvjkbfegp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqiqtgkhv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqwireqic.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gdxmsdoma.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gpbnbbxqi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/grhgmhbxe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/ggwillxzp.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gepjptlrm.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gzhihgecy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdwlmnssz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gvgaezlzm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gczcqximl.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gjgtcyidv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gybsgtgdh.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gjbzbpfes.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gsfnxanzk.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/goikswvrb.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gborartct.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/guljonemq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gwzsxiigl.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gxsaxwzzb.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gtsuogzyz.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gkakqvobt.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gjhmemzmx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gxwrhrdyr.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gmaukrihq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gmqzcnkzw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gtwihhacz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gxsookfjx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/geaeqhegw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gcdcixdpd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gmsznicuk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gsqucrbfd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqohfxgwc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gbwrvndew.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gtcwpwdwg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gusrwxjle.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gkfzfjiuq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqjykiwcs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gmiafebla.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gwpgitprb.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gpifbrmgh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gexamezho.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goqsokxwn.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gdsreiquo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqeecocjh.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gejkqgkka.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gbvmmekpk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/guvcnunni.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gmdionthf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ggpcqnqvg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/goywdnyyk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gnpmplnzi.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpmgffchc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmuajxchl.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gnxmlqwxr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gykfhbefz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gprkqtouv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gccigvreb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gjxvnorvw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gmyjpjlfj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gashxpwfm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gobkwsunq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/ghhrzryvx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/giyfmdpmo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gozxwejlr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/goinhfjjl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gfsmfsmed.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gtlxfppuf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gcnjyjozk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gacyzhboo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/ghoinvsew.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gpqootadq.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gtcoiweqd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gxfndbkrl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gvowrytti.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gyhrrhpsk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gkrjfzgna.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gfgnbyiqm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/ghpqddmic.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/ghzlsciln.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gniqjlecr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gptfklmvh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gwijahxnn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gstvkkwqi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqspnbwab.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwbizqtpa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gfokkdvgu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gmqhktsnl.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkpvfxdau.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gntoojviy.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gpelgrmdi.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gymcqlzjh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqzyyumtv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geppzsihc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghpicyioh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gxdacwbdv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggwupzuyd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glsvpdksw.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcaxphyix.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gcolrmjjc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gbmkofhoc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gfvcfcozz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gbguabtin.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gatmiodyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gthpunujh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gornjnnne.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gtfugxgth.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gkajicnsq.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/ghqvmpftq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/ggxueuzyo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/glfultgns.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gdvmogtir.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gevyqqocb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gnrdbisaq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gjneaapua.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/goacoyuys.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/goszwlgqt.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gprhacatd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdaakinbo.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdstjireu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ghbkbthzl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gcfkfinmc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghjvsnvqx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gfwyfjkfz.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/grgbgnyub.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gxpgfndwd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gmvgradml.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvlvblefw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gnzvujnir.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/guqhcgwye.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxhqlaama.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/grtcdicfi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfkylcyhk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdulqnind.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gnrlpcfqi.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gvfzsrzvz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvxjtuiqx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gtqyuwfwh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ghrhtghac.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsazlsptl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gfruncebo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/ghrispqun.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gmtghjnge.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gzmaprbhx.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gfinnogfs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gxeewsjyo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gywhizedv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gwmxzhfdv.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/ghqzfyaea.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/glixjpoft.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gadybpayt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gureflsdr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gnpomjhmt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnkemjxae.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/ggrlvvunu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdfljqqqt.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gbjmxzriw.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gjmnpsrei.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/genvqfhmo.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gruewgxzb.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gzxhpjbmf.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gtrazdlwr.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/glufhdiah.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gujmqbguq.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gzyboryic.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/ghdkmkdoj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gbqoxzuea.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gjyzanlhy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gtojnfaid.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gxforembz.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/grkxttmvh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gcfbzgopi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gnpfzfpuw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gkbljpabp.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gxqznfiej.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gpzwpdgil.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gyslkmxiz.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gzveddrnd.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gzraazwbk.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/ghwlqtwaz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gxqxshmkb.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gbeptmfqe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gspbhivza.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gktlgaycy.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gxopyoznc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/grjmvfask.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gsxuyniki.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/ggxpjlbwk.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gvovkhjop.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gpqkxrzoc.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gldbglzlz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gmonlfpqk.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gufbesmho.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gakpdggst.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gutkklyse.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gsqflolar.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtfalazwa.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gcnpkcdfh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/glssurnyd.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/getxvekpk.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyhtnyjgj.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gwnmnlefw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gvaujglna.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gmmmufrks.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gilwdywnh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmiyalmho.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/goeptrdjv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gdqypzvae.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gbmlpcypy.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gznvwambp.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/geejzzayk.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gztpxpjxw.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gmffiarlv.sHtML


<!-- 参考信息 -->