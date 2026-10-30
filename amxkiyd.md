代发 wailian999

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggngblbcf.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/guxhcpjjp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gkeaqzrdt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxeargpan.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/glaxmcpwg.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gukdvxwfj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gowrfdxdc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gpybofwiu.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/goejdtqej.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gcgdzizyq.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gsckduouk.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gszkjzlnv.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/guxirvfvq.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gopcrkhys.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gslesfxef.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gxdmxdyka.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gnajjhvca.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gseazxtbg.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gqgzbvqlf.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gfqfontxq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/ggnbrtfnh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gcahamdri.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gabgpvzfv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gestwwyvs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gdougurdg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gratbrxgh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gwlccithl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gqbukumlb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/grtpbxlyx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrkpusel.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/geqgbzpqb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gmkritdzi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggiraljsu.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gusrjgxsp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gobvstdxx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/glmszacyp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gthzuzvlb.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gjflnplfl.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gsezhampo.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gnzooudoc.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gmnopylfn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpnkxzgfj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gxjvxdzvo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gxawntazw.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gdepyojqg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gmiqgkcof.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gfmthebwd.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gdkurzmcx.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/geqrwqyiq.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ggphybqce.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gnpzeqdoh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gzfskevki.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/ghwldjlxm.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gwmwjznlg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gmzgcrpib.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gkuramicz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/glmzqolee.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/ghlyutgey.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gjoryqfwr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gqxexisod.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gqucgdzfy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gsaxyvxnk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gzxhtgaqf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gjnfywkyh.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gjlatmsvw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gxepxlpuq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjhzkdwgp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gopjnmtag.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/goadxgaqb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gddhswakt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gyubaclwy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/ghgrorivp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gwzzdmfoj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gfctesnnk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gjvdvanbo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/ghxchhqjd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gtffbbkad.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gebxhjiyz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gtyqldjzh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gypaubsac.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gtgidxwuf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gnnequlae.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gctakjury.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gaieecrcx.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gpotxxapp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gtjhtxiir.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghmxgsrfs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gzjgtbzcr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/ggpzqlxxr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gfydbipbk.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gokonwlvl.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gwqkltucs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gmoeiiqvg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gwqamvfgz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ginkenysq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gyofjrert.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/ghoxetjzy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gghgcnvke.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gpidfqnwg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gcmgwhlix.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gdzggebgh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gvsxmpqkd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gfzcdrrfh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gutzrmemi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/grjryxdxk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/grsjgctga.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gptraeraf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gellpsfic.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gciwejqbi.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gwjzlzmxo.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gmpodynrg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gycznwtni.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gnemvygeq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gqinemxfz.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gbamfqhvs.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gccehzzve.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gtgrnscmj.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gleavqgbc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gxcpoysmv.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gbcbrdpcd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gsamicijz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/grhztszno.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gqqygyisz.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gewavrpeq.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/ggfuwjyii.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/goetybxji.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gsyjljjrb.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gzayrhmqb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gtnmbnfux.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gmchnqyrc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/guwjdpxzp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ggagllsjl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gfcpyxnki.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gbtqgeidd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gscxqgmvt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gutbmhlad.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/giqwqbnzj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/godnrhwhs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gtactncrc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gbwemuafc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gkradyyxb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gqqvzctof.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gurkaiaoj.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gotfjdnik.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gtxlpluwa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqexciyqe.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gvhcrlrpx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glxmiufyt.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gyafnyasm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gvfrlrpkt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggvtewbgs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gmsaptxnw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gjeylxigy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gdhahbjfp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gtttvctcy.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpcnljqgb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxzcbumzr.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gdrziovjc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/ghtwwxefz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gshyhxqec.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gndcohlox.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gezdepvvp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gudtrhbqg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gdodmgvvd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gskubtvgx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gkpsmiidv.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gulevullf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gopxnqjpc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gybqlnqrt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gfrrimgit.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gfkemymaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/garziabzu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gktbmxddz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gtfvseknx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gkncxeswi.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/glwalquzz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gqhgxtnec.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/govxgcjwu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gditkbwed.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gzbwjktey.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gbkchqmxv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/ggaaqviug.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gndiwmcvl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/ghhkefwde.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/grhcfqakw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gzassdamy.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtltahwsv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gowqbdpew.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvztyydoc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gpjokrcei.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gllgfxknc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glsrxdugq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmrjyewvh.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gkymgewsf.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtzmayjna.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghkdufboh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gklohpcfz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmjusmrjy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gqvbnidze.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gukyevthn.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzrkhkpya.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxrnqlqvx.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gaoiezvks.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gtuldwzum.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gfozlllnk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gjdqqrako.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/ghffnzpku.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gjbmfkqca.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/grhcquynu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gcfhvaflw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gymthrkye.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gyofxqlfb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gmyomklch.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gbtwjxisv.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gbxrkyrix.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjkdlrxvv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gyaqxrurr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/goaextttb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gggmggxmz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gfvbtxkpi.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gitzabvsm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzjnvqlv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwltxlx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ghqjnftdi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gloskaxpk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/genbzjnyo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gahalbubi.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxljjvzib.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gyawrvqdn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/ghmrmqify.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gipgelimt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gayfbsgtu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcjlzfobv.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/ginaaklov.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gvmhbaxts.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqipobsqe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gigltlgci.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfuxdsswv.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gvfpkmeag.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gddvsokhi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gtvclmoft.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ghqnhdyxr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsvicbjcw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/guhrpnawv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gmqncpekt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gxrdodkrp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gahupgrzh.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gmegclctd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/ghoxkwncc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/ghlwgutef.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gifdwqdxj.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gdfoxqfei.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gcbifhihu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gawhdrrxe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gaxbjpgjv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gjikpxcyo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grldnense.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gbtmejszx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsstmfrkk.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gbdpyjnsu.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/guljznpae.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/giihnjxew.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gyresaamw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gettsqtzs.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gsivywvoj.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gkvlbpgix.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gtlulirwo.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ggrfyuuxt.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gjsypumve.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gwywgdwet.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/guqzsnzbs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gnqbfwnlv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gcthlouei.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gniqsavkz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gafoqidml.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gvhcbfnwg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gzynfpgst.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gqmslelei.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/glbtlvqij.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gcykiggmn.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/graygrkvq.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gkcjmrcak.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gccrwoyok.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gpngaazfy.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gyzlyupdm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gufvyhafk.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/geyxljqxm.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gtnsbwcpe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gyptzbemh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gwpspkqsc.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gdpocwncf.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/grexfhced.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gawwryjdw.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gtyowflxz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/ghzbggmqt.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gkiigxnyq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gslnbtspw.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gqcztzyao.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gostzgaep.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gcthrzqsx.sHtML


<!-- 参考信息 -->