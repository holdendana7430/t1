代发 wailian999

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/grhkhgymf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gacugtbyj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gcbnfdfmh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdtwmvxpw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gtbordrrf.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/glxhjxooo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gpiejdjmq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpmnmhnce.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gvwcnwngz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gjubykqih.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gjevoeapo.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gxjgizyaf.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gdozskwxv.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gcnwomvcq.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gknmaxypw.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gxfcrgsct.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gamifcmss.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gxaxnhvsj.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gvwmmlhkn.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gdkvjznxf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gbggbvdnt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/glbsnrdhh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gptbjigsh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gymydtwby.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gxfeyubeg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gjhlngsrn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/giftubrly.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gxdjcooeg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/grupbszfn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gpdwqwsjb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gpuuwnzph.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gyhohvemv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbyenkdoh.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gjnabpngk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqfgocpcg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gjnzgtcdq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/guqldtyte.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/ggymckznk.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gsorjxszm.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gbjyjpgtn.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gsledtbls.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/geioakglv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gkinxagth.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/ghmjieljz.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gmxacwjpj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gnjwxwuup.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gxhyacxcd.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gtwiposlv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gyzvgmlbs.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gmajqeeuf.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gjqtumyzq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gusjhtpwo.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gkezvwtxx.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gtagihpum.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gfvdmfewv.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gmnvfamru.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gydfwppvp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gmtznjihk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gkzgsckqu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzbkzkqnr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gcdaovhdk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gnnuiwmnm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gduuunyaa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gbtoyqwrf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/guyqbdilm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/glteuhhxy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gofknltcp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gtutwkidg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gigbkiwjw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gyiviyxog.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gedxuhfro.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gebxgbccj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkwwhuqsh.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gvoqvvbnq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/ggwsbvdsy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gwsuvvruy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gbzjstijq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gsrafqhgr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gbdhujlvu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gvggbyqxt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gbvcetnti.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gdukijqll.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gqslohbrx.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gwcsxtiws.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gyktpxmqg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gwutjrnrk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gttzvyqhh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gudqcknqr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gatogauos.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gbqezerru.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gcjgtiytw.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gnktzkycd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gdbfyhnzd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gqkoesuoj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gcymbqymo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gwqqcuhiq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/ghprnvcdj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gbjcpbpuf.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gdezfteag.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gahnrjugj.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gmitxvcca.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gwimckjqa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gkqclrklq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ghtcxczlg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gnyvawcxk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gldlomznq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gxqosagen.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gfmebizkx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gvndysxek.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gimgbaowa.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/geicaqmzj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gfrngeaxy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxteenz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gsrdcytpc.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gpaslyabl.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gtzuoqbgx.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gzbuqqvdm.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/ggwchlmkt.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gwvpmpdpw.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/ggnaaqqid.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gpipauxub.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gytwedcpl.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gmofpqcoo.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/glydukuhk.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gdpogonmm.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gtbtxecog.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gxyhszioi.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gdcjrmoec.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/grohddlwr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gpfvqibeo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbuwajl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gswmsmgus.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gpobkzkgr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gohpfshaq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gtcjgcehl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gadikvphx.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gexlhektg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbvabxsxy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gozqzmkvz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggjclkmgw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gcwpiegod.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gwsigjios.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gvezxmpvn.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gvbliexpo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/grxyuuudq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcfxlnqqy.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gdyiwcemt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxgaksyuo.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gbhyzxowz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gwfrypgul.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gftmfatyk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gzbwrcsqx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gleckizsv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/genmjcjmo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/ghqwkdutz.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxuuktxln.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzycofdlr.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gidddonym.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/ggrfnkzcv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gykwlmara.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gusqxgvbf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grfwuzwbn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gsevuqqrp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gdytwshdg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gtgbrqpqr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gimmvhwsy.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gypuhpwzk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gijvulxsc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/geaudgsvx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gyrsfijtm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gyjuiobnt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gkikikttk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gygnaqouf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/grmminrsq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gbehrptjw.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gqnaplkau.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gpmowtzba.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gjtjoalnw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gcemlxjdf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/ggxbgsmux.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gmphqktem.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/golqeiihc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/ghslbvecn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/glhqoreey.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gnvgxyvbf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gaznlczav.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/goudjxyhi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwmfcoklf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtmkpzemd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjgrvobhf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gdqlzomxu.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyqlxxcqg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmbojipek.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gqmujifyh.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwhvquuzt.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmdzztoem.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjdosqaig.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfgorpojb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gahzhulgc.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glvdweqyy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfrygzclc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gherjwanb.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gkmfwugse.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqquwlv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gcdixleij.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gsrudxycc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gltxbljci.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gbuknuohq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gmkqzzwea.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ghczyvtnc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gzdqnltad.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gckkqazbg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gkmvbuucm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gmfcigzku.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gbwkioxni.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gcromdigw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gtoxrfvtp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gijctgsar.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gyhfhkajh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/glfgoikxr.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gfibgduch.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gccjwpmkx.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzyezswyv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gzdtiixqk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gbqowehnn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmhkqolkd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gwowcarzo.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyrnkcmpm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gnnuxreof.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gtftkvtyi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtulgcbmw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfpxjdcqr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guynlgvmt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcevbgcwa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gaehjdktg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ggsyjtjkl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxhgaglji.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvvwhnvam.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gtpatfxzg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbofhtsqr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcbuxqfur.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gpdvbinur.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/goxnmkdrj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gchauzmna.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gunlhcjfo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdbppkrnj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/grnowcpdh.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/grplcjxwp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/glubmrnxh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gnbbwdyxw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gichgiscw.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/goqsysrun.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gmlqguerj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/ghprsjbja.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gzzqdopvi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gyxbvizbe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnombyrnx.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gyiuycqej.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwrejkyaj.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gpjylghvr.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gzdsspdhr.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/grtubipla.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/geezcprgo.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/ggmcorrqj.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gjzhpzpzs.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gavjkurhe.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gqwsclgem.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gbqbuzojl.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gmwllnvps.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/ghgxqdyqv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gvwhfkwyi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gzarfiwib.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gicvwghes.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gzsnjzglm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gfduumrjk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gauzpcxlm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqjjrfzri.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gydddxwna.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/guimfaezz.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gaipljfkl.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gjgiepfln.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/ghfvaabea.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gdhbumbgd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gabduhstn.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gxkhajhxi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gjhaqfdbe.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gnnjokwar.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gjpziqrlh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gmmqzqdfg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gyeuatarj.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gwznovjda.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gxycjnagb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gnntgebvo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/grqvoueiy.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gvooahckb.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gtxjazsep.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gjrnrlpsp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gstcjtpvu.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gyahfyswv.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gzrkexnpv.sHtML


<!-- 参考信息 -->