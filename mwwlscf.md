代发 wailian999

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gtjpngmln.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gbhitdbbj.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gjphbzyhd.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gclsjjqin.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gjftzxyyt.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gdkzltbyj.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gehamwnjd.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gxsmplbnw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gqkcpfvve.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gnyxzcsxr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gyzczpmfn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/guaessrgh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gbbyvanrw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gpgoxuuwm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gobrlecbt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gtcskbwub.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gyvtgtsqo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/ghveyzvfn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gnelhhjcp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gthepmxwj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/glghdciem.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gilksgabu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gmjpjlwdv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/guzpyckal.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gjfellvmh.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gezqevdgu.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gmfpgfweu.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gythbvqgh.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gooxareol.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gimogafys.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gavaqhqqi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gahnecbni.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gvxqtcmcp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/glrmszmwp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gexafzvrr.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/geprqqcux.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gnxkrdipn.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gxyeyltyc.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gqnwyjfni.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gkmyveucv.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gifjnnspi.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/ggchddjgw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/ggvinaqbl.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/grwjnkslz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gecukudus.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/ggpvliupx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gdcgmxnmz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gfnnlzlzp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gcnvmogri.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gxbopxxhq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gqjlcilxf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gbfzgaoxn.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gockyrupl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/giiprqhii.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gfrpgnnij.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gpmwolfvz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmvatjnbq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gxiiioodd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gnjqhsxes.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/glpqrpuut.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gqqcywtpi.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/ggbxuydmw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gooojprhu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gsloymzad.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gitxpdkdj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gjomwcgir.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gitwokwcl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gtoczpzep.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/grrmmzifl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gnffxzngt.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/grcvptdtv.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gfiagpygb.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/guvsacrnj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gmnsrqqym.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/glhzrdyhq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gfyyznlso.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/ghkatdifm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gkjhwywon.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gfhbmccfo.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gzbvvwlfk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gcirbpteb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gtlhslcge.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/geuhbfdup.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gnrufwujg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gtokpychn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gropadebs.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gobezkzla.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/guugzxqqk.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gpsvlgoxs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gksbmylyp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gmuovxxeq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gyvonxvjn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gckqtvrxu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gecqlmubk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gemhfedff.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/grulffkco.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gtwacihhh.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/giockqtxz.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gfgqsbowb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvjayjnig.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gznllrtuv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gdqptglsf.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gpdmgfrjn.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gnhqqerai.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/glhgmtmne.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gqschtolu.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/grlthqygc.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/ghdtwssvw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gqxwgjqrv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gsjcortme.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/ggxmuffex.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gkgyfdkdh.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/ghbodpqnm.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gkywjnjet.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gnvmonxwo.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gdtferqdt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/glfvwahmp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gamsadafp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gxbznwqbl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghljmenbp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjtzcfllr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gshpiheoy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzxxsxhyu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gmlaiqgaa.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/ghteonyid.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gzljrmbhf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gcpokooeo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gxhbsqusd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gnriitckt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ggmuialvu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/ggdhdasmh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gcotbnizn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gizfsobyn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghwuaanvc.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/glsnkmuil.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbbwfshye.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gnzhrgqyx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gvyqbwvlx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkrstrqzf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gadnmfcvn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gclqygyvf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gksqztmud.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gxuanbfcu.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbpjqkayf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/grrduisty.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gidydidbv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/ghwrblmfo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gtghyndgp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gatumikyh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gqxpqhtfk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gwuhryncl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/girgyrmkx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gvkpxfrow.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gknpaqwws.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gramwnzok.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/goxkpubdz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gonnsjrog.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gkrkifpzs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/ghzzodzst.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gnvifeysr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gqxmbwzjx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/ggvwevpjr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gqedbmxle.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/grdpszuzn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gtyjbhaxu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gupttvspx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gnymtdhna.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gnagzulox.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/ggukzxlvd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gyscpioex.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gsfpemvye.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gzprijegd.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gxnxzocjt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/ghnndyjnk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gebxydmhv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfpqvnyeu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghuhyyokk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gaxuxqphf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gsekqoijg.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gukizxybi.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcbiqxlgu.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gkqyratlw.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdbthqffu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzyxlgxsd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsauroqno.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzmxpprtr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gkkxnzxgz.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkcnaawum.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzeqhqheb.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdykhaaoz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gadudqsol.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/geqvlelpz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gyamjadpq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gqjydsrxi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/ggrqxlnow.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gwmrcremz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/guuyixaaw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gvyamfbjv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/glhrdqkvd.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/glwkgjgqa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gpxnslwan.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/goxsjyiac.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gdjlpbjlr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqrepdv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/glizllohw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gtnbfgxpf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gumtdywej.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gusgwobfa.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gycsfejhp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gatxqfbjs.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpyunageu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gtoidtfnh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gcyfderlf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/giafbiwcv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gftkdtcuc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grzebgsvb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gjfidvccw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gbpwjdbre.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqfunlmup.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gzstmnoye.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/grpscfcjs.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnbcksuhe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gxzxjctvs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcbtgxflj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkafukmys.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gceqwjusr.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gyqpvctdk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gfvkvxccm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gwhtnuwfd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzdvdmlly.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gkkjlfpio.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gqbmutaql.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gnqkinwfp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gasjtodhm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gfmeuqjtj.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gbcvqdsqe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gekmbxfxu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/grrsujseq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gtdkkxwzg.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/ghfhotfnw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gfpyjqzja.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/grrnygbwr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gidwaiycs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gdymrrlwz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtsujkvnz.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gkswoiujo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gysdonnlm.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/ghisybuhf.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gwdcetpcp.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/glxigkcig.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gbwzflhyt.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gowsoljix.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gegrmygzb.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gwtvgecot.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/ghhsjoaeh.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/giqmodjkg.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/ghzpelamy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gruserlfy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/grnlhrrxc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gfjswghln.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/ggdcmdfym.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/grvrrxxne.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gyqljeqhw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gkmmyedzb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gqaqdlkan.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gnsaeirds.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gnfurrota.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/geyfeviuc.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gspwokacc.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ghfoaziyt.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gfkuyccdu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gfrkrjeea.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gxycgvyys.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gosfgsujg.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gpqbwhhqe.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/glulaymkd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gdlphsdby.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gocuiyxkx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/goxtjtqxk.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gnkuffvpw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gajpjsrbv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gfrobudby.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gmwzpsswn.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gtdjifcdx.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gljckldox.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gneauhkno.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzzxzehcw.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gsmudecze.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gdnupzeuc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gvndbdobo.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gwrclgcbl.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gpwhjcmmt.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gajqiflrm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gohippwrl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gzugbepaw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gypryferr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfetufhon.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gvviaqjbx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gziarrhvv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gdqpcjwvl.sHtML


<!-- 参考信息 -->