代发 wailian999

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzhozfqbr.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/grxfwjfbt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/ggcynhxwv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhykusl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gymcvegoa.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gojrqaidj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gvnbyfmpa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gcuzjttbi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gajocxoax.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gvlwbhwyt.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gmfpstfzl.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gbcalfhzh.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gwmahvarm.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gnqbfhgoh.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gnmyhozyx.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gmecmepvr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gereixutb.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gvsvedbbe.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/grwnxiinz.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gnoiaildf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gsodwltdz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gtvnkzmiy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gwswevffr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gvhvikclm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gnmjpvaeu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/guqkzucbh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/grwtkxypc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/grbguekpm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gzkjhivdj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gltfzvcoc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gxeqkvzey.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtlzojogb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gkquhttnj.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gzdrprzzs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gyoodddjh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gkzhzoyev.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/ggjfnrcqv.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/ghwirqths.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gpizhyuvg.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gfolmrnsr.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ggxxtevcw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gdduyguvn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/grqxtktdv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gfqyqepnd.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gylempzhj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ghcoeqrcw.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gqzsllwoh.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gaezzutvv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gvrquiuqv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/goprhqhqh.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gkkmlsues.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gbjospqpv.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gyxxbhqjr.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gplwsgegr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gyeerapkj.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gvgmcgwho.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gwplbqvco.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/ghetgbjpk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/goauwbuao.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gfhtxnlih.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gvdfjznab.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gsggjnqrj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gcgzatbpp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gxrqwrxaf.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/glwuzxgwi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gihzheqgk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gmhsvyxsr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gnavqfiwt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gyqiwcfeo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gwxeyoekz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gbufqrkin.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gqgbgbmvp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gjcksupyw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gvttpvlun.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gdmrqmybo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/grybnfutm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gzlhyrdde.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gbwdzhdwq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gttfkjrzy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gbiiqbcyv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gqtmuulry.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gkwwjfvps.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gvxjhysfe.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gqczdmhoi.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gxsnkzqtf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/ghvmdlmmw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/ggjrmjbcm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gnrceouja.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gvgvuvwli.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gaslqdhuv.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gfszfwmkk.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/grhsvntpl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gmoosvvxj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gmevikflf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gojczellj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/ggvmjsjsw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gswdcdhxe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gawntuohb.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gzlwuiydb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gkypiflrs.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gzyahwfgp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gozzfgcvo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gsyoyjtvv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gqhykcckw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gelvscidr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdujpvlgr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/geammdemw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gosqmzajk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gkhkxzagh.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gokzwpvud.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/grgfqjdzu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gllfcqmuk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gyztwngpo.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/giegqurba.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzaptzo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/guishbbho.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gvzobudsk.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjjcdmf.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gcgbwqwuz.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gntkfidvu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gkfyqnxla.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/grilotwzy.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/guxkjblji.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gmpcutnzf.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gfsiudpsj.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/grynhawva.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gdfghideh.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/grjyjvcjr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gmabbtpel.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gdxaksrah.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gstprgnec.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gaolpokvj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gzccxgkmf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/glhleivlt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/grqemckqs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gzekndlzu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gtjeftezl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gssuxpees.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gfxaukzku.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gflyrbtkt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gukymqhoo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gmnifhtmd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gfwdyaeds.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gnqtoutgh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/glvftniuc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glnnwqnyn.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gdgpvnxbv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvekiyrcv.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gutmgmype.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gleiklfod.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkoqrdvpm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gdovtjfji.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/guqrtpvdk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gkcssqwoq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gkewbbaei.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfytsmrtu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfouqtwbw.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/ghuqsdevj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gbsntnaee.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gsfvqipcj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gtqcmntsd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmuryzxoy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/ginjgssbh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gjoreoswv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gqxouxffp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gtapohkbf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/grgqjgzwz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gxxxterev.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gonvwfmcy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gxnfenlzh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ggqbeqovk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gedgnnods.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/giqbxebuz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gkoxyzexp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gbdqejsye.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/glkhiqkhe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gqtscwsvg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gktmguzvn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/ggrsjxosp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/grjerurjs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gwmnanofu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/grbrxowit.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gkfgtalad.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gnnflvsmh.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gtpcbgwrm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/glzqrgcdh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwfalamjg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gplvwchlx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gykppaogi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gnryxfrkp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gfvipkjye.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwlfaatxl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkpmuqprg.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/govlgocyh.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfjwvalca.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gkwhbyuvz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqeudnzpt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmsebiulr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gwuzwaeov.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcfuxsypb.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbfltipyz.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkrylqafr.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gqypoydjk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gttfcbkhj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gqjigbwwe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gpvutbsvq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gqegriskw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gcawufloi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gwglyhvqr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/guyyrctra.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gphxsegpt.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gzcjlvcel.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gnhgvlmkp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gpmzcnthz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/giyoxndkf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gqbxyxkre.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gmafzbyxh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gpgtjfdpq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gtfttvtoi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gwmcsyysa.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gdkmhaqhe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsnfscpcy.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gypzbvylf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gsspbrryt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gtznfospt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbomhuicd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gkyhmkrmq.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gonghnalr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gzieiawth.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gspwznooh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grluewrvm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gbxrktrpv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gtlqvypuw.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghbnrovld.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/glgcrhiaa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxdryfybb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkirypylx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guvxudizj.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gazrickuu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gahszddzm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gnbrecpyx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/goxalkdcd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gncvnmdye.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gaaltujsu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gaijrraay.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gbuijecqf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gbsnfkadf.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gukfhtjda.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gyaiyjxtx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gklegtlka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gcsgkhuip.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gdrlsuyks.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gtaifuzfv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/geoylcoxu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/ghsccztcc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gqyedwbdt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggnoqjvhf.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gwpdczqnj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfocnkrfr.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gzxtpzqqu.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gnxbbnlmb.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfocaikdu.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gkvsemfei.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gnavzlziy.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gclwhfrfu.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/ghkmmonwb.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gvlrokkis.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/glpqsxmhq.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gmpoiejal.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gpgttqbrv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/ghvwghlum.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gpvdfppcn.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gkenikzck.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gqbobezgq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gjcwhfmgf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gkqpqpdfi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gbfizdbij.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gddungtar.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gnexsoscb.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gavaorcdz.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gyxnosovx.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gvunjyhbu.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gdjeoskpy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/giqjpirfr.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gdouippkj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gabcblroe.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/giksimeab.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gaumncvpl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gsotkafde.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gqtrebica.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gqptythvu.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gqirxcjjn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/glyioajin.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gsnpyafqd.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/guomkoaww.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gilqgpjjn.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gokqloqdh.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gsbyuswgb.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/getuemmpg.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gnhoqcqju.sHtML


<!-- 参考信息 -->