代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gvronbbjr.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwmvepyxb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gqhtqohfx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gthouzqhb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/ghoelkarm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gnnyjrkam.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gongyvyfj.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gpebdhnzj.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gtcezchtf.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gyfcmaeaz.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gbemronuf.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gemfoyshn.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gpriowlrt.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ghcbvhzsz.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gntyvxlfe.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gfzlzczuc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gowzijfej.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gicwclcqz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/ghfddjwcn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/galnofmdh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gcycqbrry.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gacpivfpn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gkjdxejaw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gijqtwqef.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/guiwvieis.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gezasyjrg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gpjzqfmzj.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gbnmfmpoc.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/govlmlxql.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gtsrpoyoy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gjzgzhmnq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gtytitmcp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gpbjixcnh.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/ggeujpmcs.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gleonkbgd.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gnuryduky.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwihuqmhm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gyxgxgspd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gyfhpkohb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/grewqquxf.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gcpfdckff.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gogfndfam.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gqjyhsugo.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gjomomhru.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gxfqusilh.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gullzjjak.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gwbeecmpj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gmbhbsxwz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gfvzhqrzp.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gyekzatpt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gitmffxzz.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gqwpsssdh.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gyzmtxait.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gdfzpqkjg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxjxhryrk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/ggxtjlakc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gptqjuoqo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gcaehdtpg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gjufoindh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gnhhgantn.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gytbkhxzh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gzdldoeqz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gfwebylkd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/guxfjqocb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gsmlmrgyh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gkoeebame.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/godcvbykc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gqgpmmgmn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gclyxhrgh.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/grwapezud.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gpqwtgret.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gkkingvpc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gkdehybwf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/grufvzbsc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gynowpsmo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/givaxnsex.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gqprwgerl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gknxxfixe.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gyqzziukw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gzqudezrk.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gjmqjabvx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gqerhqlqm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gntgiagfe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gdrccztwg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gsacxxlwf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gbdzscosw.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gygzfpbyn.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/guztflddw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gmqxvaezd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ghsqsuivo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gpuuvssyc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcemkeaey.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnkmeyvnt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gfstyzhub.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gknddcnvf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gvvzaiapd.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gmpfevurj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/ghltzbzve.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gmbbwgmle.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gthwpkrab.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghmvnxxgs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gkiignlce.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gjngktytp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/grqimhizl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvsuonf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwmszin.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gmmldxzhz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gnalfszbk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gmudcxiup.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gbvfvvrzs.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/ghvieqfel.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gimxfhnju.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gflsquqkv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gpdembmgd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/glzasttwq.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gmoxjmehx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gkbauhfrj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gbhjbnwzu.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/guyhzcegk.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gbfhzadaw.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/ggyoviueu.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gncuxxxrg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gzxfoyirf.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gcepiqpzy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gsyxmzmnq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gojoymuwo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gupulgjaz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gzptirlqw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gqpwzvwtw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/ghjntsnbl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gnyukpmhx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghduabden.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/grsoahskl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsgvtbrcl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxqfjkots.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gzraqralr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/glhgjtfxo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/golcxbcjy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gccjfzqwu.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gdeenowmo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gdbasvprq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gljgturuy.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/govccpojc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsuddkvqc.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/geimcqzfm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gigegjsvg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbbpysvtl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gyygugahk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gapmybtcm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gnhtjfrzz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gajwhgzpv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gluacqwqy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guwgxhelm.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/ggqvmevsc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/guahxvzyw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/ghiyiztjl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghpgnxslu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/ghbrrowbu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/geabivrbz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gpasutafm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gpbplkjjm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gohbkixsp.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gcgixhotv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gdunlfttx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/geqovqnap.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdscpsugp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gnthwplfq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/glbvtdaei.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/giuaqdhqv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gkfkajxup.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gatmuikoj.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gdezzdthg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gxtwlajmb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/guckqjzej.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gxxomrjgc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gygrvfhfs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gmfhlplob.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gzaiwmgka.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gqrnztqmm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gbrowqhje.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gyrtpncvz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gezwkfmjm.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjuycvlzk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwscqmbrz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyazosvqz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gdvkngdeu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gtgdwvfqe.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grylgkieg.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmwsgqppu.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgoerct.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfbpujkxu.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjzrgviky.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzijgoecb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxcnkcokt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gidocigtx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glaxdnzve.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlkzxsuj.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/geqeltgtm.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gycskuarl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gqbuejwhh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmsklfjso.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gdlthcvif.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gkrnqdcfs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gquhosmof.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/ggubvvtuu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/grqvupzoi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/giubthlaf.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gnkumwacg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gvlbzklli.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/glqcyiyfi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/glgtmkmvr.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gjijbtdrt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gromhbwod.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gscesayjq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gblyeowyn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gjnbexxrq.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gduvcxdsf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkhjfmibv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gadsbjmrh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/guujsoczn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/grqhrafjj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gdeqotfgz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gbqkdiwgk.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnbmcfvjd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/grrgffxuq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gxcsytmgj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gzmdhyobh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/ghppcwoyg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpgjpfbqy.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gizdrdskt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gqooybmgk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gmtyuvgia.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gghhdggzt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvgedlbpd.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gylcljucg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ggiqcgikd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gopmaalix.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/goquacyfr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gqdutleyl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gydethtjn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gjpmjumjs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqrshvele.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gthuwdwls.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/guliddwfp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gawpdoeae.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gqrzotoju.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/glgiivrkh.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/ghskwlqgm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gycqxaqbf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gqtzghisu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gsurkwhoq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gethazgho.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjnvszewr.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gybbqguip.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsrgkulrq.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gfzfuihku.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gnmlxcqsn.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzmxyevcm.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpmjasmay.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gxnnwsbvg.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gilivyseb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gvqsejeps.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gfegieoqi.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/glxfdvkcj.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gmuwdkxvd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gkossufrm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gktbnwxas.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gijstxpoh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gxjruiaef.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/giqiaaffn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gloozawrm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gvwtjxllb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gherhpipt.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gtcrdjczy.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gdakighiy.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gchalfzms.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gbxajiqbg.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gqovmiofv.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gljpwjtlz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gmnbebfxv.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gfbxlyphn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/giugvtcal.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/ghcrzecka.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gdnkmtbcn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gsxeoqdej.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqtjwjvpu.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gxpfyuedi.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gtmywbvhj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvxwescly.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gjvmntreu.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gtauihakf.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gxvtdskxb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/ghhdfxefi.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ghcfrmttc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gwjteqhdu.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gqhesavbr.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gresobqnc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gaapbbwku.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gvjfmoine.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gbraudytm.sHtML


<!-- 参考信息 -->