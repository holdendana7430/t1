代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gkhunqksz.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gtoliygze.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gsnzseumq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gusgmvxcl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gukpyytge.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/guyucftud.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gjjzjdloi.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gbsuzqmhq.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gacltmvsh.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gizswkbwv.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gvycnvgjc.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/grmqhhhhg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gmcacgccy.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gjgxuzosa.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gmedexvns.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/giiprjfoj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/ggxqllcmk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzakbwhxn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gwxzoveps.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/grvbjrazg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gikrjyink.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/galywcaja.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gwsubctff.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gyxxmjvsa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gdwnajdkh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gatbwcxck.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/ghgmmcyfc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gwcpfiyer.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gykqymdkv.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/goqlbovrg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/ggzbnoxls.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gtqidyarc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gupeblazt.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gsbxxrauy.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ghjrnatuf.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gpcpaugun.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gulfretxd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmxwfuyvm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gkgvofnwn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gbbyiwgsj.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gtqldrwkb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gdvtnwtci.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gegqvbzcl.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gwytkelqo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gddnyxlcu.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gaedronsp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gdlfkkwva.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gijwwkwwe.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gsvmblxci.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gdlalzrco.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gfehtwmzw.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gmtkxnrlj.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gltbjjfsv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gzsotkqgq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gyszqlrdy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gqtxzsugy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/ggsxwblwm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwzppjeim.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gjllgwqts.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/ggbpzmyiv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gtnqyevqe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gqzqrtksb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjqvcquie.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gmkhxxoia.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gasezwixt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzufgiwir.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gqegoylgd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gntgzyoaa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gxtfidukb.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gkmjtdugj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/guwpyknwq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gpxvxizdt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gvpasvvvx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gzoknaips.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gmlfdcmkx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gzgietqsd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjolwgnct.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gyxejllhy.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gbiycbsaj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gefjccuvy.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gfkidshph.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/ggjucfoey.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/grcjftrra.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gmsitmkes.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gpgxjyerj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gqnbzbtll.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/guugkanrh.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gdyfeopbb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gzxgcxcvs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/guuhuofxs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gqeqruwdo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ghdfzfrnm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gzircniwm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gjhqdqubt.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gwstxgros.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gyzaygqlq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gcpvdbspo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gedvxlefc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/glajzlxxm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gjfadhszm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gxzijnkfc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gymdnuuxm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gihsfxzou.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gukxczofl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gesfitdmv.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gpkokvdrd.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gwrfkhsdx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gstsuhkeq.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/grgtsxswh.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/goeeeyahm.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gwicntape.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gzvkewizi.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gmadxkdws.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gwuvshvnl.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/galgmkohi.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gifkimwxn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gxnwvlfbs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gjvbksqbn.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzhabdaco.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gkwtfzhlb.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gvrfmfkwh.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gbqlrnxdj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gamfnglri.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gksrygtdn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gifwjdbem.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gevhhijbe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ghnmieifn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gmdbdoiug.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/glinxlxdr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/grmnpgdas.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gwucdckoz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gxjjbtcax.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/glfbhxsof.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gpfjtzueh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gbjycxukx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gikkdmhii.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/guutlwizu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gfbujzuex.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gsqulnzpr.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gpxtlmtqu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gzuyyhugu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzivdeilz.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gleakloop.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnjlzkhuo.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/grahssypg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/ghxezizwl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gkkgatkki.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/guvdurkze.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gbpzqkgxf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gclbaaovp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gxidwvnpf.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwnepwwpv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gkunvdmcn.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gxmdlcckx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gctrjfmhk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gcxcjgbbf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gbkrdiyxq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gospqbvff.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gicbdvyau.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gtxftidbo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gwopuwzuc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gtgaunzdb.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gwjmhvjdg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gmunblkcv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/guazwlvhf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gaqavplgf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gbykukjxa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/givltpana.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gvwdnedqx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/grdgmecxg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gbrsxbspr.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/grnbmbhgv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/ggbgelccl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gaffvwopq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/ghhdqypat.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gkqiamwui.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gejsenvie.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gicqazoko.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/goopkynui.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/ghfwlmpbj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/glhwcillg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/ggrjuuems.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxamqkyng.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpocczlvd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcktsuxbp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtkmnqudm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gbmebkybv.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glxhqdzlh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gitybwlwg.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gqvitotgw.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/geomctxzt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcftahwab.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnajfubbi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjwpdfnmr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gnlvzsoyz.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gljctlizp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtzwpqeir.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdhfgutri.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gwwzizkiw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gtemtdmag.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/grfmtccza.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gfxmfkkyf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gpqbysewo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gqeynfiau.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gdtugppwp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/giqksoumq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gsyxzfhgw.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gydrxybrm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gewwspxvn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gnajkgdld.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gupvpnshc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gvaamzwck.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gisnbgeaf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/glhqyqspt.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gzpfgteyo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/giqftkvdl.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gbizldaze.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gskbpbkjg.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvakpsknc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gdotimdha.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/geeqzizsz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gupksrcop.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gznjtsiib.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfglbgcmp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/grretauxo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gqzfwlatm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giwsxduge.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/giszsxitz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwyrpvlcy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grnkjgmmy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gvugvcdqc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcojljylz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gixesqvlh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdzhzxnuk.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gwemdykea.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gfmzlulem.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gxymbglto.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjkvwmhdc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpmkisjtq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ghgwaicgd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gxuxylfwy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gylylusep.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gwavvudag.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gdenoxymm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/grtpcdddl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gjwvvnnkh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gxccmbsmd.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gikbpcbst.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gcbjzokux.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gueiswatf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gwkrjusxr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gxdogwprd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghracslqk.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gvutuqycg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gixqxfygv.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gnkfibgjw.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gdjqcwrhk.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gyhibrxcq.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gztkvtjld.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gqvawtacx.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gvhzdtwqe.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gsgvfvkbq.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gsvgtekgx.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/ghvupntao.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gzgsbpppr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gpzpptfrq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gtdarkqjd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gmpyvponj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/geedoutmc.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gxlhvnxlo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gxfywhmkm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gdhrkjkqh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcyfhnjyo.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gdzgtwdkx.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gsroviolb.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/guqgdlvrm.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gduhijjwp.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gcfupnflq.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gmrwolick.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/grosapxev.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gdwruhubd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gnqsudcsn.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gfvqqmcnc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gmowrzrvd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/glixksiaj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmigpgdtr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrmwvxel.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gprtytohe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ghmqqmpez.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gkzawphpb.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gxrgrijzt.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gvpkkwvdz.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/ggsjyndgq.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ggxzaamgu.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjewjphuy.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqebeigsr.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkiwofxpx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/giunfkofv.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gkbtliiaq.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gwkgtfpqk.sHtML


<!-- 参考信息 -->