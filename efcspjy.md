代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gxypnnmtf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gcsmlgief.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/ghxtopsfo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gaqxnlyqv.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gozmnzxwf.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gdczxyoxk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gemjpuwyl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/grpdamfse.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gcdubggrv.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gzvlofpml.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gzjzxxaso.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gnolcdrnl.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gxvsjagwb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gemecwhdx.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gfcwggyye.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/grthgqtcp.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gpoopjirn.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/ghverkonp.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gxbohfoqh.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/giiocvfff.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gxhbmyeyk.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gcvybghaw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gmajmsofn.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gwsstnjvk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gjdaktzru.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/ghtlnvgfx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gmonjuswr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gqkbvcnxi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gjzdcomaq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gznyjpobw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/guaofqtrf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/ggymfrejx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gkmywneph.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gwhyuocwf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/govjmijnu.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gbvmhrdpc.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gqmumezlw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gzpgfrzsy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gmvgifcpz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gjcdeewox.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/grsoahxfz.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/goqauniso.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/glpqbwqwm.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ghtxxhotb.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gfdkateln.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjdauwtvz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/ggysydgxt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gdmopkejd.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gdffjqgjl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/ggkvjpfhm.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gtyfayatb.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gdanhqmhy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/giqcrxubp.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gjycbcjrp.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gyxwjgdma.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gkzxvukhu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gegbsgfaq.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gfkdrblsd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gwaenlcdi.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/glhaddxwk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gntwtgzxr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gvsagljyb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gcanmazuy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gyhtdqojs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/ghygslxlj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gemipivtb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gdykrlgcg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzynjdsaf.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gnrpaqrmz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/ghtqqorcg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gptdxoxns.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gaynuicmx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/ganaaasiv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/garvtefxk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/ggpewnejx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gbqndsroq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/goqmddmgh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/guaiiuxvn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gfrkdwwgj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/glnveqpxj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/ggywbnrsd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gxjdigggi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gxvbmcrpc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/giskwyfko.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gnnpobdjv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gaagbgkad.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gfqssllbr.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gceecrksn.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/griirlogd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gzkuaazbz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gjdlhhczr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gkfinvpkz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gbaibabwd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/guhjxajps.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/girfntlkf.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gayzzoglb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/ghbluuxin.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gzwpwtkqh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gtdnegkjz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gxmxlajqw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gulaqzzvk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gotoqxevz.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gdffmiryl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gabizntrb.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gamurbfmx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gbcaasyon.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gfauwiciw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gositbrpc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gbscdsftj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gwguipwbv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gursidbdd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gfiqdwjld.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gyvbsvtml.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/ggivhlltn.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/glktutbtd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gabrveyuy.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/ghcnipqwi.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gjynedsie.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gosvhpkyu.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gfkuipdst.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/galusbzqk.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gnozwbvad.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gypgftpcv.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gexmepcyh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gnzlxnztg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gocmcjqwi.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/ginmlyxjq.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gymmaynog.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gkzecnmtr.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gsnlaccfq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/grfmbfwwa.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gtjuilpca.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gdovaszch.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gjzhdjdfg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gpichclrv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gsgxcorxr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gzsudctqk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/ghvllpear.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gxuxemxdj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/graxxjove.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gtvukxoya.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gniyttijt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmaqxabba.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gdqzvntbw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghsuqcuqq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gcoepahst.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gsdjhxpad.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmuiebtmt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gczkkzrew.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbiqoewbd.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/glfiecqhm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnxeepdlf.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gclajjbgv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gummufysi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/glfttbbat.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gsilmkdcg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gzsaykfxg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkdmmzifa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/ghyfjfllj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjdmswosx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcunzjekr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gbjfkqqbg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gfrydjert.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gcmxmbhyk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gwtsduhin.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gskfxbagu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gweqjygki.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gampzjhjx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/ghaaqomsy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gilojlajt.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gyldcpjgs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gvmqfwehq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gumelhcgt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gkhaivmxf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gcmmpxijy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gxxnbavgq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/ghrhkccds.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gxggsorei.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/ggykubpya.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/grfplhxuv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gwgqlzvcz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gszdsyxnh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gdhzkyvgr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbjdmlbgi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gzqincind.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/grfvuhpru.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/ghbqenjek.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gmzmartsn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gsnuyjtur.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gtboazdcn.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvjgskejl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcdahmfja.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzuromfru.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/goltxjblc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/giduqrwgz.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gksrkfaeh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcddhjmvy.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gmwxqtjxg.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gashvatjq.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gkchdmxlm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gskhbrdqa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjubkxqfc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gijrtxvts.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gugbssqxp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwbuinlkw.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcsslfngv.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gnwqwmxcn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsapgfk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gknncglki.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gazciocjm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gpofytkmg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/grnmgvdhr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gkwognogp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gknmmpeeq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gflnbzxaz.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gxfxhkkvw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/ghjymjoqu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gbqyoayim.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gxrcpoyfs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/genpjzjkd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gsakbilmk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gmunykrjv.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gquxfrqpn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gogjmfyzr.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/ghlihgftc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrrltyks.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gfbeiqwnj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gjuumefck.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gjxwkdiuc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/geiksadgm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gfkotujrn.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqqkhoigy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/growaxjds.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gdnmjlfrx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmxcwzjtl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmpbvqnbd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gilwbmlwy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbxscsepq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gbcfhhyet.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gterntmtu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnmdgkrvq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpqdotcyf.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gzluzcxaa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbyfidlqw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gyzwoyeyc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gnbcrhybt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gilaqahjl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gplbwbcev.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gyxdoydtu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnfeqilyt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gmtzdvtuk.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gazebnpkd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/glfnedgyb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gjsnywrmi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gmrnsedsh.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gptfxtiyj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/ggolckumr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/grcidctoe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gestnikei.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gljiwgurj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbnrxuepk.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gxiygitdh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbtbcntat.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gtzdeeewk.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/ggdvvudzn.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbubvcmse.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ggegsryqj.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gmonztiur.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghxkfhtbc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/ghmucmylf.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gsswgciix.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gcuezdxmm.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gktyfelab.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gdfchtkbc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwjngfs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gyjuziitg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/guhuuoljk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/guzrbgpij.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gskopgvld.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gpgqroelq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gqzjqryyq.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gtfnieywp.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gbcydnvkp.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghxewvdbx.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/goprqcsxy.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/glditfbnu.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gzjxyyqae.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gfkefeasz.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gigjwnqtx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gjjjvvfsq.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gqoargpuu.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gllezreco.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmpkwgp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gnqbdgnxj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfzckxblh.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gsihoalaf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gwxlothoc.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/grmxbzynb.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/goxlvbrzs.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/ggjarruvt.sHtML


<!-- 参考信息 -->