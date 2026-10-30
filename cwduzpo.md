代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/giikrownh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gtcaexcuo.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gaqwuqlzi.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gbisjwnje.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/glwguynut.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gurjwizyd.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gfvdrtkbt.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gudlsqopp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gcjfupgmi.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/globzgwls.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gcufvfbvp.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gkfkyyaoj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gpickuwdf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gibjihqvt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gfyqiadln.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gsivtfnoz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/grllaekar.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gnuvsewgv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gdamvphvm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gdgrcayuw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gowaslnid.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gldmboqvw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gozaffvqw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gitcdeufj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/geqgmqmso.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfwdabozg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gvavkexry.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gepkzxfau.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gckyusyuk.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtrlzoyqa.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gjjgpgsay.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gwqtillkg.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gkfjnkcde.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gitnmkita.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gwhmozgzc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gnipkqcda.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gkjmtmczy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gpidosqex.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/ggptlykyd.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmywcdhw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/geejwyjxi.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gxlxtwzah.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gupslfydv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gtuldskwn.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gqyskhfzn.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gsboocyax.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/geiexxvkt.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvyoilprc.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gxujmntsj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gyzeddqqa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/ghbtturqh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gdrmtffep.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gsaqkhghy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gnwptxigo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gtvrhdnlj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ggftbldvs.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/givepnxzl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gbcdiqict.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/ghreejbrl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/genbombvf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gmrglozwh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/grqjqaoau.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gfhwcfkrx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gcdutsxok.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gcdtqacgd.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gbqmspsuw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gksbjsvrz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gkntqncjm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/getpkzymw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gwcrigadn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gmftggijp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gkrnscqki.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gwladjukl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmelmboa.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gbzytppfl.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gprlhqttl.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gjirpdfzq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gwzghvwgr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gtokcqwni.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gcjiqmvoo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gbexzleqz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/greriyquq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gttpmmuze.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gzvktucro.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/govkfwvvw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gzpgaulls.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gefabgmgp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gyodvzvlh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gpuutigkw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gjsfteqxn.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gvpoekdsw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gkzxxumwx.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gqemvmgih.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gcocfezzj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gkujuxldz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gyqzsusvw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gffopheqd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjwbexhoc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/geihiupss.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/ggppasozi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/ggjsfnxgp.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gavhwxqoa.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gmctwrxdz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gschrsgla.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gtiquoscr.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gzrohbnrj.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gsabziscf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gmfiubsvk.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/geczuxmvp.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/grfrmuwbo.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gwlpxmzwd.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/guertcnmb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gsmztuafu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/glepxqfhc.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gwwovwqcu.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gvxgyzkwy.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gszgfaucf.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gkcghkvmu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gnwqvxdaa.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gjhndjckq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gpblzphdn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gehlndsbq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gzehmjfnd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gyjxjefaj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gcwsgevhv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gllfoxyyv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gkfhucfeq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvxtdrvvf.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gvgtsubgb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gkploxozr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gquuyeheh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/ggsrkasgn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/grwxnkpmf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gjnyjjtxz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gsazthwqr.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gqjxvmqzp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gbjbvfuxm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guevvlfne.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gfymovzgs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdgonfxct.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gndubljve.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gmxdqadac.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/geqbadpen.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gdwkonncr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gewdkmtfg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ggokwajck.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/glrbezheg.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzgdlgpcw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gylrzojcq.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gsjkzxoop.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gtkrdvrgq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gziedncmc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/goaanpsxv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gnyizgodm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gwmyrpnsz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gzqhzcaaa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gkrdwcaty.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gxjlfxook.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/glfwbqthj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gqsllcxov.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gtxntmoqn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/glgnldmfd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gqahhwmkk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/geceumwlx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gomrzozyy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gssgkwygo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gemlicpfo.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gzsifyvvu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gcchnhwwc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gbwwrycvs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gloldjzic.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gmiyrczpr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/glukkfrwu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gixjcrref.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gbclpafeh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gitzmetgv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gugfvxnuf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gsicshquo.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gjqnhjcoy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzdsfegbq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghrtwhsjm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gkffqcaxb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gyzjwmmyh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gagejkosu.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdyzohhet.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjlerxxgr.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goyswwglm.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbolhcvre.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpulgyzft.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gygornywa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gixjohaxu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glicgkxju.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcrwhrcwp.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gywbcamrp.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/ggeqnokgh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gcefsfytb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gddsmertx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gfetrbiap.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gngvgzqac.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/geyjlejhd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/grfmvmtij.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gmdwquwpr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gkrxzrase.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gfvaoeram.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gasttynmv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gcgnwciyu.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gnknoegkm.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gyfcdbhrv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gvqhlzxhg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/geajwbmyn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gpwrkmkty.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/ghhvaolst.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/geamkvjpq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqlfsmiao.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/guizknril.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ggtmgohkm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gmuirtauw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gqtkiwuyp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gmousmjel.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbcokfwib.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gpsixkqib.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gfwpcaeah.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvpqwzmxr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmngufaxg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gffoguhst.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfukjwfuz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gpqpwzdrc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gelibctts.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjcjcfyxu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gclmdbzfm.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gbtxafgyv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gokfhmurn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwzxqized.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmpuuyhou.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsiiecohj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gdqceatug.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gqcooxzit.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gddubdzym.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/glplcsnes.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gglwxczua.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/glxkdtalw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gzuuxzckg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gegggfdta.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/glblhitgz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gtpyjhwid.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gdpchryup.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gmytudluu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/ghcwloapq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfknsffge.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gsgbrxlkm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjhlibfxb.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gbhhvhkvn.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gnxhfcqiz.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gettyznce.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gdutwscfk.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gtyqyjocd.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/ghumnnmdw.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gmbbpeykz.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/godvhnpol.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gjexnyezj.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gxnosfplt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gpyexexji.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gmlcayeyg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gdxyyvbsu.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/ggrxdomns.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/geywyapyf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gihgqajjf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gusdrjjoz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/grgmnypfz.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gksnspyyw.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/guryjhzfc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gkkhfxkns.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/glgrjzodd.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/geeeaqtnf.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gxaoazygh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gohqyujos.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/geozeyzgb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwzjlilpt.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gmzmpphwc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gihwwrmrt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gwmycddka.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwdmmnbow.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gsmxfskno.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/geiijgynm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ggrxhbbdg.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/ghtlejpkb.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gktyyziit.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gmvcafald.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gobtpgesx.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/galwiqciw.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gwzjkugab.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gezmpwoys.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gemdlmiva.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gdmkbxybs.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/goxkkruwt.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gjyvkoaee.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gztrfelic.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gpktododx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/grpymwndi.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/grwcljaxc.sHtML


<!-- 参考信息 -->