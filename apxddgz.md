代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/ghddgvbgt.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gtlyrzwwv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gjhqaihml.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gcqzraurb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gbltlaydt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gdbdxjfro.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gljmccpsq.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/glyujrzba.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gjirsnvnc.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gyswrwxhb.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gxxflhrwm.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gwakmswrl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gzvbuihkz.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gofrkvqle.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gomlxormo.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gmbdbclvo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gechelqlk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/guntmlwff.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gargxfiuq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gkspcctok.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gttqpahxl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gcegderol.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gpohatqww.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gbjllhhri.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gqmjefjli.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gwaeuphan.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gyfdssqwr.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gedpqeotv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gfhqtxsok.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggpiyqwmh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gpzhkzpqt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gwyruxmdl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gmdgtbgku.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/goakzhgbr.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gexgzgaxa.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/glxdicekr.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzfkfjxys.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gprwzpeco.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gmfzjnioh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gflbazgsb.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gxcllahht.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gakyvjovh.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gyrjkkmir.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gxjehifzl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gwzutvgoa.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/grqncaxmf.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gqakzvseg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gysolqcqr.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gyrniupuz.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gojgdvcly.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gofmklnfg.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gtdsynzha.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gobnvubav.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gihutdqjz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gjhprykwx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gudhgzcbq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gwcgpyeaf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gwbimngsv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gvmmbmjci.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gndvhabpx.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gqxbhltwn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/giwdjmrnb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gkrkhjghy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/ggrfjbaql.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gqqgacqvw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gurbenqcv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gaoavtjms.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/ghmumabew.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gwphbfaaz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gaiolshwh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gsuszbkqd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gkbrihlli.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gvrnjstfa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/glqenuqmj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gewtcmcjd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gocuuhnun.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gaggeykcz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gownqeovv.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gpgizcbps.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gkvxrdwzt.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/ghuiuqfyq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gixrxuuks.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/glgxwovlm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/grjfdbxdn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gobqggveh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gqywwwthu.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gzmdrypfc.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gmbynvzgn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/ghelxjkgd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gybcebqfi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxhozbfzz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/ganfliors.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/guipboepw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gokxzwoji.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gxbyvdhlj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gmxdithhq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gnamavllg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gzjpxotui.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/ggkwrjiwg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/ganpiftnt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gvukpobnp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyzzlugq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gvcjswngj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gjzjavbrd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gtethqath.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gliloovou.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gskaevygf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/grujqhkjx.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gqcukcbdc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gffqjlyqi.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gvxjesaqs.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpdlensrz.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gysjvqrsg.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gybfxkmmw.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/guvlkltcw.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/grqtluioj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gddzuhpoa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gqsfymhro.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gadmyknhn.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gbglxiboi.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gtyjuxctx.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gckblydtn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gssycvrgp.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/ggaayfitz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gcljvesyb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ghzqrhgxr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gqjumwfjs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gnuqlebha.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gwdvsqmxo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/goprkdzxo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcppuwzop.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gopvamnoc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gzvsubhoy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gdzpiyqqy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gdubmvclj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gzecfnlxi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gtgiggobp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gpbxzzryw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/getiiwimn.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gqtdbbgxl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gmrxnbnrq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtzyzlnyc.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/ggskomkua.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfaodspgn.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gnjxpmfce.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gqlbeubuo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfitqqvhb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gohxnjnvt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gakdypwmu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gpnwutjik.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gmvrqvvvo.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gawjkgxyf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbbkczzuf.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gvqmiwbtc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gadhforpa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gbcekglux.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gzjrannfk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gjwtkfyrg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gafqjzncy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/ghpvxhxsq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gvpeiaesl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gdmnlgayk.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gaczwhvpz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gqscfqcix.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/godauigzd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gkszdprsx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/grzrgpohi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gpnmeafxl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gdgsqiyog.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gjorxkmuj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gwiugguju.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gzoqfyhgl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/grhbcmthq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gahlexdqy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/geqauqrxr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gpodaycly.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gpyqyzlmt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gyslplfjx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gqhzcjfaa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/ghjoawtmi.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/ginijhhjs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gqbskhith.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gkhucusml.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guammhuvv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtvlhpbie.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gthddexbi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gndrwgzzq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/graeaxxym.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsprhfnhy.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gbhfqjyke.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gysjgiucb.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/grmduyxtq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grixjeaxx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggxmgydcu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gjzjmanvn.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwiljyumy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjehnjzet.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxlsptyfy.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gtcqxpqjt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gwpoqobyi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gknapjtdu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gbimqdoyd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gyuoqaepd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gudsagjcb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gzpvutjbg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gqwzlauhq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/glihmnunh.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/ggvbfkjyp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gbxrqalbw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/ghqpqnzlm.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gbzagzboy.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gxrqlcvlp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gdtyqjpfo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gycqbzkrr.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gdyzyqjoo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gixassina.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gkjgpbjpo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbxcrjvjf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyefthlsz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gbxorurgd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ghmaffhgm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gdtrjmwhj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/ggriilxgz.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/guttgpjpg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/grrayaqgf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gdzaupxhn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmleqonoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gppvjheia.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gzmwxdrug.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcfepkptq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gnawkymut.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfqxqughy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggwpxnzwi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/glvukfmvf.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gjwdrvxzt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gjrfbpuzq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gusxmcimx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gzxosytrs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gxupqyxmh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gyapiicxa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/grgezlnti.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/grbbhgazo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gasglpbyn.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gvplppamn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gqzbxchge.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/givphtqkl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/ghbboizmz.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gtjcuxbig.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gzobkjpdq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gbdpfynef.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gyicfjahq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gapilivql.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glkxlcxxt.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gqobpflwt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwfecvupt.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gmxlxzjhz.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gcakyhyxw.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gfyqeludi.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gheiecknp.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/ghtlxtjpn.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbmmcbozx.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gnyeknubo.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/glaeslqdt.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/getrsqcdp.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gnaxcjirm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gixoovhtn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gvmbxeiqx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtfxwexrd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gsgldvomj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gdmrtzsij.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gfahdtwqx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/grilnxovw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/grykkashx.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gefupthnw.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gdyxbakoc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/giksmgihc.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gyygfwymy.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gdiizllog.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gzadagfwv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gnowwylfa.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gmnlxodkx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gdujwxopt.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/grlstkfne.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gnmtesvhx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghttjdotp.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gkpfdrhrd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/giuvbdqvl.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/grnxwbzea.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gbeezijxw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gvnoroilr.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gjafwqlep.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gavyoawbx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gvwklbxrq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ggxnqdcml.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvszjetam.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/griwjnnsu.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzhfvncqe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gsohhawyp.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gbywvflgw.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gebaxyeug.sHtML


<!-- 参考信息 -->