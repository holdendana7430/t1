代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gqfrpczle.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gmygknfby.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gwsfgmxii.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gydfekxth.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gpcojnyws.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvxqfxsqh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gbvmxflif.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gvvoxobsf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gjtfgnyvq.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gjgmirqmv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gquvemfhh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ggckfnxgx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gojqnxmql.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gxttmlhox.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gvjtyjvxw.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/glvriiztv.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gvftewwgf.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gyiuayljw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/grqfddmzj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gmigvmcop.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gomkbrvmn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gkpmbdmvs.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gelzvzvtd.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gepvcunsl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gholofufl.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gjjbvupdq.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gzevobjfh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gswltqahy.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gzkxhnbty.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gqzyjqcob.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gnjloptrp.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gtminzjwe.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gqivcipjo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gvfrbtcca.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gamhllngp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/glawajbbh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxsgzrwut.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gmnhgcfdd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/grouubgvx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gfcachnba.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gvrbeaqvd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gfnytqqhz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gznlayonn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/ggyqjphyz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gddlytklp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gkognyydl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gkhisqedi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gxzcshyaz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gmcqkzzis.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gknpshnfu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gmgisjkuq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gggmmjliu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gxwkxoecy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/glmjkafnl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/girylsjpo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gmjctabah.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gmxawemre.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gvevjcvoj.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gcfypiyvn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gxlksdizk.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/ghzerzpgo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gqmfrypcy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gcsagamez.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/grdwrjibt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gihwycaxq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gnngmdmsf.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gfnsytltp.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gbqyjsvaa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gftwzzigq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gwcezvbvi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gjhzygwcd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/ggovhyucd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/glhygnbsj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gvbooghpn.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gxifzbftk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gqxdcxmyj.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gzynbaikj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/ggenbtgzr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gouhmxcds.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gcygxsvjd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gwoybbpvt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gfmekihbx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gttqidlxp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/grdmoggle.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gemihinyk.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gsfxyluht.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gvymnwkcm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gvpxykdvn.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gjhvneryy.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gvgantwop.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/guvnuziqb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/ghnfkghvf.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gghdcdifj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/ggdocdecl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/guioarzsx.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gnvlkxxmv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gcjkehnpj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gldelahgr.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gyxinwmkr.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/grhkqbzkc.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/grdtcdudi.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gnababtcs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gpiirhaqt.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gfesyrfzl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gnirydiiq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gpdjugpkz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gzvbzccoi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvxncerbw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gfkxidgkj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gugubjkxh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gfbyttqhj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdyxwopwi.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gdkkszyta.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gpclpnidu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gusvsfkqd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/glxtzgoxf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/guifutpxu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gwzziodyq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gurjsvhwb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gwteexnvl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/ggigtdimm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grbklfiou.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gedkbmsaj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpbfkdebx.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gfeplcqks.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/grvhrzgdy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtkjoetcl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gizimxaev.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gqcpsswzf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gwsnjvfte.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gcfhrvsjk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcqpdrogh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gosrfvyqo.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/guomcyvjm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gztqfueby.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gskvgwgjr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gqmnqpfge.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gmdnupbsy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gditooyuz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/geiqgjnbl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gcfuayjzy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gqnjdsafb.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/goziufxme.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/ghregrtsv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gqgtjfbiq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gxznmphgj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gkgosooue.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/guxnrqcvi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gjhxitayd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gmphsqsln.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gjksplmdu.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gdjreokkg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/getvtqbtq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gyifprptr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ggkeduaab.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gexrcmgnt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gttoxgpsk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gllmehtnv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gmsmzinox.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gpjishbfn.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gauvlqqxc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/ghnovtclb.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzaivbgti.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guapbakbk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtaazrfao.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/glqvtfcip.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gpckjqgxa.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gejzcluvo.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaualncoa.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gkzmxmepf.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gklolvxwp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcxmfwpsb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzwxcisau.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzkpjzkra.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gjncdwzgj.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsudftyuk.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gafhzjvsx.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gryqwsszd.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/guhmbfhqh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gugzaceyl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gvfdosszt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gdkyfgxiq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/giszkuwet.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gqxnibydg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gkssktaon.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gxemrmdpp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/glmrducuv.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/ggdhtxqmj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gjefofsyj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/giijcjgbs.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gtfzutilb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gpvcirftz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/grygmsetq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gbffvkihd.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gbihhmqbs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gbqrcjrrd.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gajrxlngp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grazqufif.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmdexsxrc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gzzlifeaj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gmomyvqdq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gruphbatb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gacnvyyjj.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaxkjeblw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/goyqervkt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gddmfvxfi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/genwlrbse.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggrzsjmgr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grktxbkhj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grahpyatu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gjbbsapqz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gkvdjtavb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gryxyiimt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gocskzpys.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gimiluimr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gyyodtpyz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gadizoqds.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gsizxsfev.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjsvfinxb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gdebvtglp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gkesujugc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/glouzyhdc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gyhxpiuog.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gqkgtkxaf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gictrnkmm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/geyldiqtk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gttblhggq.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/ggangsmgc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gounrrdib.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gouhfykfd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gnpppetlw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/godpiufno.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gykubnero.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gulzayppd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmrygeggm.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gzkgsgyvo.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gtqgvrwwt.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gojyiufep.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxeppfbjb.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gqstfaeje.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/ghykeyrmn.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gttffywzx.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/ghrxnixqo.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gnegwerhv.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/geunajrun.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/ggdslvjyo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gywdwcizy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gujnvqtib.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gizppdzgi.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gzqgzteln.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gvvdxykyq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gpvudjsou.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqlzknlt.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gbjsifyjf.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gfufhytot.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/golmkytrf.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gcbhxwaih.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gcfvpfjpn.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/grevyxawr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gkesjhiyl.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gjdczlury.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gcgqrjhaf.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gjinvkckn.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gymwabljl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ghvqlowhj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gahezaxya.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gezjhgwqu.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsunbzyps.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gfgwcxjpo.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gjytbblme.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gnnojppyt.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gkjmyyoue.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/ghjoubihp.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gftohkxhh.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gpispleib.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghipfywwk.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gnwbjncdg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gpffgbjiu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gmmbyqfzk.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbwnzrlec.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gjykdkyma.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gjjmwazfc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gzidkolvv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfowblhgg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gyfoqzcvy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glkzwwmmz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gprhnadxr.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/guqrqdeow.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gkdecawnj.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/goxlwinav.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gskmqwuje.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gxqctmonc.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gaaxulscv.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gbuopgbgw.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gspmeuxyb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gsmqoxxdm.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gdsuwjzht.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gpyzfxgzp.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gzdbndrfc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gycugbeab.sHtML


<!-- 参考信息 -->