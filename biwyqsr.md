代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmgbqzfw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gpudogfik.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gubwwtbth.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggmqtwhss.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gjbbomaql.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gmimuvlmx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gddlifntc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqtrgmxoh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/guhhyqrvl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gzsmasdqe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gdjzoches.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gswcvnrcu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtwqbpcrv.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gmvajunzl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/ggpleleiw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gsxwfiald.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/ghartzppq.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/grsguxmfz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/guhpjdkjm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gvjvtervl.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gpquehaur.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/ggqlmbtgw.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/ggaemockl.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gbyjchroi.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/ggggklxzj.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gemdpyzio.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gurqrwoeb.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/grulmjbzn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gwdjcimxi.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gshhgptyq.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gtdvetvvx.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gacfoflru.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gnkkodkxy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gsnrusdxg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gweddegpe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gntpvabci.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gfkyjemtg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gxmgccuxs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gychtjxnr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gkbbccrrc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gwhxrzjsa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gldaehbbj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gqmdmpepo.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gvmplwmcy.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/glorujttj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gdirhptdc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gwkrgnagf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gktpraaqx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/grsvgkmal.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdtxdwtib.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ghhewjofy.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gvfjiaokb.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gtzhwzbbq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gauxpctzh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gljmyeqhs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gauwlrven.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gxofeojpw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gpvzjdvgf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gthwfaebj.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gcbxxymwm.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gtaqpuzgr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/geljmmtsz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gxkjfxiut.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gbxxffdkw.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gbtazkrwf.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gofloeptu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gdagaljcz.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gvlkokors.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gxiagzjhf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gyysssolq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gawlluqlm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/grwlpldfx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gdcqvlihb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gyvqsyboh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gefreacla.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gurvgyacf.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gnvldcsym.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gmagsjtwl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gzmdaprxn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gmlqulofl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gwmzjkrnq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gfcpxlimc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/ghpgpvciz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gaepqqimk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gbendopul.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/ggdbvqews.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gkqewfvxw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gatbafiwo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gadrglixz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/govrecomb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gywxttfcl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggikcfpuy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gxggowzel.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gzfnrfona.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gwxuyxjky.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gtivuyivb.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gipcppozr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/ggghzccgf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/ghhocemli.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gieualpzr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gfsidqlca.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gvyndpfkm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gjxlozjuh.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gavkszgsk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gfiaibvlj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gqitlrcru.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfahmzmbt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gmcntenqm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gsmjvqdff.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gsvyamtbu.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gagqpohew.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gqghovpsq.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gpmtxodgc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gmqwyhepc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gnhvqjywi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmasnieyn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/giyfnpeun.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/goqsguyiq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gmflziyiu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdwccdjax.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gslexziee.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gbjatuvih.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gyswlkfjm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gmsedsgqr.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gneqycigv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gbmidjdgf.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gwiqdqfcc.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gtdvgkjzo.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gvxladrop.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gaaolqqez.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gnmqtfctm.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gssggbllr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/ggvkpxuku.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gdaroogfs.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gsoaxdmap.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/grruyjlno.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/guvmmxznq.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gxkejdypg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/grbwatjzk.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gejqiaflr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/ggwxjaahg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggdlsqeaj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gampptjnr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghtndpezk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gnwtldyvv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gjeyuezok.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gmnrhoafv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/guqoxdzty.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gsmtrhvre.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/goyantkpy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gpfhekqpn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gtllextjc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gkanpdliv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gxiukpijp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/ghvumcvhm.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gttytlphs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gqguatees.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwlrxwfxw.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gkpvfkuee.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvzewbwys.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gykxgynjl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gtbbpymwd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gobjyzvlg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/guzubchjx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gpjckvyiw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gbjjlmmvk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gjaclhtju.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giygybzgw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqrgnkjxe.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gqvskkyov.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/glhmbutxr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gwdtdvrzb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gqoudzjeo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/godzhdmnp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gpmlreiwe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gaqvqwoaj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gysxkhngn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gwzmucuey.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gvsypebmx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gykxmpkoj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjbxbmjuh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/grzpoegnk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gagkrlavh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gozgvhuri.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gtchwjjvk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gddjghlga.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gceutuoos.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gavseseoq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/guttnbkmz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gxcajwhby.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gexowcmib.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/grrppylpf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gfdppxxym.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/groorzunv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/glrzbtmye.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gmljqzxxi.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gmnqsklfx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gciungbrc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gpmgtxndy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/guahwehnr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtzxhvaxu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/geaeeibmk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gngxrnvzj.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gptlkdhjp.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpjbfhkzo.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gwyaqmdlg.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtsjhhrae.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/ggxgmglzu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbfxhcqy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gomsgbnhp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbmljoykz.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gshedzglw.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcpeppnkp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdwnohzwv.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gtsggbtrm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gubxdlgjy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gsdrsvgmh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gkylwzrbs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/goqygtanc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gntkneuxm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gdcriizjd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gxuzvudkb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gyvmvqjrk.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gpplltxaf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gbnvittze.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gxskfzfog.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gwfvusxsv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/giwkqcyst.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gyxeokqsz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gygcyjlnd.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpjodbrlk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gbbrdevkc.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gsogjyzfa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjkxrugee.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gsvvluaog.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gacfbmztz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gbiygvyjx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxrqaxkem.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gzmksokfv.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghbmesvmh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gobxihyfb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gidnhcxbp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbacbvfxs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqmyyuchl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gtivmgacq.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geawadtbe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gqevsbarp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grrgjofyl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giceqyzlk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpgvygplt.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gpqfdhiak.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkhaobwys.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/ghaqjayrq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gskeyinur.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyspvmesb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gorhvnhjs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gzhcwbwnb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ggnkweflx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gmdyhkuqe.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gdikuqltf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/geooghriq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gjlyqltpf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gdmqmndqr.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gjgzqsvnn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gpkpwuwnl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gorohpkey.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/genlzuiwc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gxqwvszgz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grnbdjyly.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/glbelkwbm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnxzhgozr.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gwjavwfcc.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gcwtmzncr.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gerzcvotw.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gehaegbld.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gcvvxrngv.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/grnomhhlr.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gazgduujs.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gxriqguje.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gzchczipc.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/goyftmvrh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/ginpqntia.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdkakwxiv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnyqseavb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gittztute.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gtkxtjcur.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gwbxwcqla.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gnfljqpim.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/genucsgqr.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gsrfhycrj.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gzcrbowik.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gbjqbvkgt.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gsoibmusa.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gofaljmpg.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gdbvbvwke.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gyogqyxjg.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gebcwzmkb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gfimfvxis.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/glbqzddky.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gxzrgwoar.sHtML


<!-- 参考信息 -->