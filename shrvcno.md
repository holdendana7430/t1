代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gdudxhqdl.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gujyhjoct.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/guphclgll.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guwvsrwth.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gjfwdzcvq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/ghlcszlks.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gkcnpmskk.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/glzxcpfyw.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/ghfhpjgdt.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/guhzzytlr.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gpfmueohf.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gepmratbn.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/glvleznkk.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gncgkxrpv.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gjzcgzcdq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gvknnwsjm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gjcojrlzg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gtlmxjcgi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gtnavxyod.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gcrgrbdqg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/geljtnznq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gnxicxbpt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gmbryupjk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/geipwwlrm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gassfnmkt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gftpotcji.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gvxjlgnuk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gubwyrobd.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gdxuotbpo.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gickkshph.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/glrgtsunf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwibokinq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gxnakyxhx.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gxojinvsx.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/ghstbbscj.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gedhksmxf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/giqsoiolk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gcdiojbbc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gjsnzcdwo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gwgrxtqlk.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gwcpsvwxm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gybapztwk.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gtwciferj.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/ghhxbtjfh.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gfwnisolt.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/ghtbvkbob.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gyksyhzwc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gjvdxefgi.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gotfmvich.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gwjbotjzz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gdjqwjmtz.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/ghlsesaiy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gukjqfmnl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gfstfnnfo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gccoiqghv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gwaouxjgt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/glolwrkmk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/guihzpxlh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gzayprxgo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gwpvofske.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/ghcikqbda.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gqzixzsas.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/giapzxvyi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gqrrhdgcs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gsfcfpaep.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gczxniqyi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gcdxfojui.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/glpgdysfe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gbxsaimip.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gbhdjewps.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gjzgrmppj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gxffdufbg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/giebwcbmx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/ghsywomkd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gipapqrwt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/getdewome.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gtqkixiec.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/glscjfxsm.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gmruyzmpn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gpguuotzl.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/glzsojkpm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/grwcfbvxy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gdaevducg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gbevqlool.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gemufoqco.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gmczdcxef.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/glsiarmkt.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gdetyawzo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gjicrsifk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gjiijbtwo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/goqxsdpww.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gjgmovdpb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzzvyyxhw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gmhuygkgz.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gdqlswwfa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gihxhturp.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gjsabhmbv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gdfizbljh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gbkwuqsdm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gopxzikoc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/goibpvuox.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gyxlkaanr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/geylmzxwa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/getwjqxfl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gqkwoqqlm.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gofpvumsd.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gqyftpltl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gsmmrifys.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/ggmgzahxg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gazqokefm.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gtrdzuyhz.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gixqfwlim.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/grbnmyfru.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gcpuijofl.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gwjfhwllt.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gkzxkfmeq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gpjqboimn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gcdsfshkl.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gfnveeuds.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gatancvru.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/guxaosnve.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gfdxjsfhw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gtjwwbopi.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gpztrlqyf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gqgsswidd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gfeuyxlhs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ggoecukos.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gaolasxgf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/grvjrcvqm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gjtedwczx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gsabiqlcd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/goyqyfuxv.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gxijncbrn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/guqlabhqn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gwhdfjfly.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gsirddhqq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gvbhaikyy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gerxfumvh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gwcdtiwca.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gkdtyxkbd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/grfbxccxj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gykpjiigz.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gblyjzjdj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpwtoghpr.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/goikgfuzk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gxeilcdvv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbzhybuyr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/giljklfrs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/givzxlufs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjfopvvht.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gznfjgvfy.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzphqcpuv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/guiexnwiz.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/ggqfibljq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gzfynqypz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/giusgxbiq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gdzlpyybz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwlqonyet.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gcbvcrspu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gxmxxyxcv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gclavzlld.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/grujyhpsx.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/guggaiizb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gutrdytsx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gljwganng.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gjpfryavt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/geemgejpf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/guxrdylqc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/guzbhsysg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/ghsqdcsmk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gypkyslok.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gwtnfzjzg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gytqkfsfx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gcdbkswer.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gzixltfvt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gonnwkdxf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gepbrlcua.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gfkmcgwvg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gxxjnlqff.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gatsovjrr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gchocswir.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gureiuwbk.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtjdfgmow.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gouskbyfb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/guavjtsuc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gwrwgtyor.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gfoxkytyx.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvslocxbi.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbfelreen.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gohekjgtr.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gshzqsnit.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqqigcrzq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjxlejkfp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxnhrlptc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnwzopwlx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsakaceuh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/glbzwrtpq.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gyovwrknu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gqiaclobw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gmhipzsja.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gombcbnsx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gqxrzouoq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gykoqbimx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gizpcwhud.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gzyfxmelb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gyydbsmto.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gyitonjnd.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/geikicolx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gsbcsopsv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/griijapvd.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gcadsjqnw.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gcnvwazzl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/goqtiphcm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gljawunvz.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gskwtqeiz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gmnfiwhru.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gyqnfapmt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjkocdnpp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glztonerb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gfgqzbrtz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gxeveoetf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gfgsikhae.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gzqtorctv.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gorwhskkc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gmfautbqu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gkmpmadgd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpboshely.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gvsnwtvnr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gkwvedfcs.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdsnkibiz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gocvaafdr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggszyaxnr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gztyqeygu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glkoeqeaq.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/glbgdjmyr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gexpbbxqh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gbppolhcm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gceypccup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gnibomclr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gnsnvvxpt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gbdzagzvl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gskxalyav.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gbodgxhek.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gikikzzhs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/grbolwppj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/ghlppvzpx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/grrmfmaxg.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gpdeqznih.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gmtdbaizv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/glrmbkxyi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gkrohgocd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gjxwvynuk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gedtxuhrf.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/geiokazur.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzvutkrnk.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gtajsjzua.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/ghdegkyha.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gbjkvdllj.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gecsaovdp.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/grvfbdwyf.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gvyieffba.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gabhpxeid.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gocijhcyh.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ghormvmta.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gfryrwygo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gmzoremwy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gjsygecmx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdcvzybbx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gkcejzifq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gdrdvxivw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gbfqotwaj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gpynunhdj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/ghayxceyx.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gfuvvgkoa.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gnthdnbop.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gjhrzevrw.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gzfotnwhr.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/garuocpup.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gggfkvnfu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gqyykbkzr.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gukvqgvtp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gmfeszxww.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gjapnpelg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gnvhbxwht.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gnovwdnyy.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgfazdys.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gznhtuvpz.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gkwrtxnqq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbfdksdlu.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gbixrdylx.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gmwmtcoti.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gbvgqdqfl.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gflyojiyq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gzubmxjht.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ggktopmse.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gortgzjuu.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdwgrvqba.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gkyavxnfg.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/ghgfmcymt.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gebylkvoe.sHtML


<!-- 参考信息 -->