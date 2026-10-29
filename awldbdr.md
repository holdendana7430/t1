代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gdrggdffe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gqhjskcdo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gswtkkrqi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gzcywvlqi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gsnylyenk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gnbztordi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gmzpfhddr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/ggqangiew.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/ghtsynlcr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/grhdqjepa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gafzbcqhc.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gufouybxt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gbdgduoqd.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ggkiblyzq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gbdntzbwv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/grrfqzyey.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gbcfcnmqo.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gziudsufp.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gxnnsykie.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gvrzacooj.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gqgsurraq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gltelbajr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gjnezrhke.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/grprnpaut.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gsvxxolid.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gohciftyv.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gnrsnzlbk.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gwsbmxtlq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gqeugtwsz.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gnnovxkiy.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/grobcijfj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gzuzzgnaf.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gsvpidlnq.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gwtgygvch.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/ggofquuin.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gphcmljac.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gdbiggmuh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/ggezcjebx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gozyjtxmp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gffmtclyk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gblwjqmri.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gdbmrxiqu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gysznbfmy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gioesqcuy.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gyegdnqbf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/guxijgfdx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gaexkadhl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gqvhjorci.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gbhqghqqk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gctkebari.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/ggcpvzfsj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/geqpzinsw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gqitmojfv.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gdupjemny.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gsfgmvlmx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/glvlsemjv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gknoawqai.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gqkcymtjn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/grmqklnsk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gpeyattpr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gkzfwwcol.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gzlrbhzpu.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gedooymtv.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gemgekgrl.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gvyirfymy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/geyhqcmfx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gjrqsyzrg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gnzkzmxhe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gtgwxzzgg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gfijlxbje.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gvlnmablg.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gtvfhzbvz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gjvrdpwgf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gyfyeztdo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gmjpprbwe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ggwootfif.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/grnlkipyo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gmxyzjjcx.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gknbabgeh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gcwmhcuie.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gkdawjzeu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gtpxxtlqf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gbemuxmsh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ghiwrysbz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/greueoajk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/guqbbjrwv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gdglzxeqf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gzcttkdov.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gjxipceyz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gvcrqmmtg.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gwjekmqhz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwuuiyzmg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gnxrzgnab.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gurlkxkro.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gtnzahymq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gqsdecqly.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/grzvqozpt.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gmpvcxsjp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gusvrowcm.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gfdlnsnzt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/ggartbgcv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gylwxbuxt.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gzbguwcev.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gksiufxsx.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gwcosyzim.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gprvafutn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gopxavime.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gkjzwlhhb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gjhlskcek.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gjjlfrqax.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqxdfdvaa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gljdxosev.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gngkrelns.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gqdhxchqi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gujagdejf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gqblpxyne.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gcfltyhkz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gvlmociiu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gpmzqywdl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gsdktqvxm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gjpeunegm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gpmmomvxa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gndjhwmdc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gzmmsqsqi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gtgpgdceu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goyomjili.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gdxhqxaoa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghtxpngmi.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gzbhwedym.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/guntkhosz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/geruqakdl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gyldnobpk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqgkubwcl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gaeiyhltg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gzxasyhkm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwtfwrvli.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvceugsap.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gtlwwyjxn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/ggfjyozzl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gjweoauut.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/giyfrrobe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gtnfyapgi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gnpetbnes.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/grjsgpdbu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gqfxyypfb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gxunrntye.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gtcjtolxy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/grbomdrpq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gqsnopklf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gpcxrazxz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gpovzsmxn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gvdjhkbuv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gdhtyvdiz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gfgpmiukq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/glwzhdbyd.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gjmqmbeah.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gkooynhza.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gtmcbwvqh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gukbpfndw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gggztfnil.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gzgsghugq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gncbjmvjq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/ggvvdmdyd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gggsjmfyv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gtlgtxpuq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gokgvwnso.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gyaceklrl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtgtzrwyq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gifvvrgqv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gykevcvvk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gqtaqsgjf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gacldxiad.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpvbgplxg.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gxbqdskkd.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaotwjjes.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnocihutv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/geoxxjznc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfkbircib.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gfjfzowqp.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjkzzcpoz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggprihnod.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfdlqmrzo.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gluddwgdv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gfasfzjio.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gjobiehex.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gyqorlvcj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gcronjxti.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gteuqkikd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/ghvpaisqi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gnuqcnipp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gzensetps.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gvwyriscg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gsmcqlrun.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/goztrxenu.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gamlptbwq.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/guoylaenz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gimnvsfxa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gqqioufne.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gwudacser.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gsskmjwtj.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gwiunxdvu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdqfeemss.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gozpmqhur.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gjscextla.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/glpyeuvwx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gvgepiwql.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/glpwcmybf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbspqbcsg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gpliaorqi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gfizbumzp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmamkzqgt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwtucsfll.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyjpuoigr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbiuvical.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gyfdjnnbz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glvurovug.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gclcsaqei.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gplwcveer.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gwkieyerh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gdahypbsm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gbvjfwttx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gtixxuemg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gatwboasn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gpiejfpxd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gsvwntigj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gnkayxdxs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gougpeosu.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gfcbplecj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gnjhxqabl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/ggjxneqab.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/goffwncoh.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gkvyxuqiy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gmvjmyrxh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gsotyzqsn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gnwygahrq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/ghebaygiw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyqwltnxn.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gwwiairoa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghunbgdgx.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gomguloah.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gfeiqbfmd.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gsbtdzxko.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gzfqyhtwf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gqlyoopfs.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqxaggoar.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gvkmfuuoy.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gyodkcpja.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gpicswhxh.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/ghaomttvm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gbggeazev.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gurwlbowo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqqjlmsnr.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gqtoxzhfz.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gtlpwxwmr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gtjjdxqwu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gjghlnwah.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gphwbldwy.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gvlmpnbgj.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gbfbxjsnl.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gzuhbraia.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gckqbdclv.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gvntvkagn.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gyfhqcprq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gpslqxmyy.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gepxhqcjx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gexdysmmi.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gxxjjvlgc.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ghomytvsx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpwkzayvc.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvevrkpva.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/geytkunte.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvjzkovu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gukzjyhwx.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/giphajmpe.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gxzrplybe.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gaxvbjwvl.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/guqnhuapj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghhgcjors.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gnksgqmsx.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvyndykla.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/glsdmwtyh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gywzvujyf.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gqtysyahd.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gvjcwqutr.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gfepdhbfs.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gqwbzpcle.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/giejbgahc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gvmcvmyfs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gprvaoftg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gmmpdezpe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gtkzqblaa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gkmcnlmym.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gnayrygwz.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gsswywbgv.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/guirygbnc.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gyndvavha.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gjrfarbse.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gzowznhuz.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gtpdmlokn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gwxofsyxu.sHtML


<!-- 参考信息 -->