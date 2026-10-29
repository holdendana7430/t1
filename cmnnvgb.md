代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gdncmkkiw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/ggdiqbgnv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gtbxbftua.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/ganxmbehj.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gyjjwnqmx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/galigksqr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gqyhekqix.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gjdhpobjy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gemgyoyzd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gfnsfdedl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gqwcfiegq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gjxjtuwpr.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gwcbfvdbb.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/grdwrpqke.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gnrrttnre.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/ggapbbrwg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gamqkjjoj.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gyqgjzpsa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/griagnktz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gihgelyjv.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gckgjfywa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/giymqnkrr.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gnfydmyrn.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/ggtuhbrsa.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/ggjnuhkig.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gsogqbcbh.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gshlfceuw.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gmzjgzlrm.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/goquysrxd.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gvglbnuwc.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gwuqfzpge.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/glznjoajf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/glmqsyfin.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsnzwcxii.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/glwiiqfjq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gnfatwblc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/guybqrohd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gvqzpbmov.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gxppdijbc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gypdgbjfy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gicydzcpm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gtguokaxn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gshctpnff.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gvzetnzka.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gpwqtbytn.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gclvjlmzs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gwrgaewcy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ghvmixopd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gvxdtcyug.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gezuzmtkk.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/grajrupll.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gypivzfio.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gcgljxdkk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grbegrwnr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gowrbwsvf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gvwpiopwn.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gvcohkypu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/glflbrfvl.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gztnjkouy.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/glwwnwjpz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gqexpjmbg.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/grpwolbgb.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gcwtdwlsa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/ghnyhehqx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gowlulwfs.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gglgagggf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/guzfqagqu.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gakenutbg.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gkhuaadkk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gqzcqrnqj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gkhoevquq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gnqfahquw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gswqdrelz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gfckzdmtm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gajunhegb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gjkmfvdvt.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gviwfdwoo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gyevyfcal.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gcrrmynpc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gkjzdxfiw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gljfljhzw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/grhnvxxec.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gwjsmxmfa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gnuenlfna.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gbprlcgqy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/ggiahaadf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/grkoxumbt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gxkmdbeky.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gluvbrvkn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/grmncbujy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gfipcsdgn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gpuckegsq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gjtzbkvbo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gqlmocomi.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gnptqyowt.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/ghsnrcbuf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gdfxgsnva.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gwlbzkynh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gygdqjkki.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gypnxqjyf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gcvhqbjdf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/ghbeggyeu.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/govfomsfv.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gsruylmuz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/ghujtsszc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gviwhwamj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/geahkauqn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gmuezsaki.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gwiyifeve.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gjpvszvxe.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gbmucgymd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/ggypvpbyo.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gnwysnawh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gajmqjgwp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gzfxgrkjq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gbpljoqfm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gskvgueth.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ggtnkwwcu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gkxzrcrus.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggtwcapuy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gklgqdzhu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gmjvbfcnh.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gpyzttcpp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gqlqgamis.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/glwcmmfsj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gsmfnjhyd.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gmgtwwnwu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gkwtyimxf.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gcdnjrpsw.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gwyixezlk.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gvylyqpyb.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gfrzazhmh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gwvdkdpjl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gayjgbiug.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gvqzkscnv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gctfszliv.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gtswuwllg.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gsogveavl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gsuqqevre.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gnwckoevu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gbvaxhqqy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/glxjxqwks.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gyacxrjmg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ghyvdsoxj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtzrnphuo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gqvprnwcw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gwtmibiaj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gjalwcbca.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gfzdkfzui.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gofcjjpsi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gtmpnhovg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gubqycelv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gkrjrjdcn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gwalbzgrh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gpwtrloxk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gnntjhznq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gefunewrw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkmggcioc.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gbehfylzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzitubtro.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gfbfeulum.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gnwsjfvdl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gaphnbfdf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gqlcowdlh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gpakdsqeq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfidhfggi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gsfyqsjjy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giknmecjx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gepjuycna.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gcivlolvl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gehbgqbvh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gtrdlbjng.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/guoufdiff.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gowgmbacc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gfuwxvcwa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gycumjoto.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gwfyhzbvw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gtecrhmbs.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gblyibgho.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gltyhrfma.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnfafhcbd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/ghneyrflx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gybverttx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/ggcyadjee.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gurpfyhcd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/grxtwzamu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gvwselxbt.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/ggmrguvng.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gpagimnsj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/glnzzylgd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gixvyjkmb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gsiopspcx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gwuqdvqob.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gbuekkdsx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gyrvcmukj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gsqkgnzkq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gcwhytuns.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gufzgfvbq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtcvlujxe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghmlgwtld.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gryfpafvi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/guitylctp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gdcvovrqt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdyzlquoq.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtnztkptb.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/ggjdybqgy.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/givwccmxv.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gakzcyzag.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/godqhbpnx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gilrbiprp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gypibrqpi.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghtebwbfc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsflhrzpv.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyfqohsxn.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gykatiuay.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/giebynhxr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/giaohxwmf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gptzseiks.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gvgdzbcxm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gidyzedgg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gbysxdtmv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gbtsotkqv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gbbiolidm.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gstfcedpr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gorxttoqb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gvwtdltac.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwryhonlw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/giricyomw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gaskminqg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gxoinsjlj.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gozpkbybd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtdumtcfm.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/ggutywfso.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbrhzaitw.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdeftjzfo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gwfxfddbf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gkqetzasa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gzqedkdle.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gewisjnjx.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwzzvqwmy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gkiguqdsr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gapqornba.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyflrgwqd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyglpiify.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/geyzhxxur.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqmjyysvk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/grmjhxbxq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gbnnxqola.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwjonpqck.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gimvukkly.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gmvttaqin.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfhkhwmgu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbaggixwb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gnpellzwm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpiioqkqy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gwzdffvqs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gbrqurdlh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqmryrhig.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gkdyqsaol.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gdeckuhht.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gnesyvuud.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gfzrglgzm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/guhvmgxef.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gmbgsuguz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gubgyvras.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gefdpbsmx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gzmemzsru.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gbgssfsly.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grnjndeeb.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gzrsgsrwo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxxjlcwij.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/guxzivaky.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gisnobfvr.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gbkezcivy.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gudcjjayb.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/glenkxqbm.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gymzdyknm.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gaobeoyzs.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gmwisghto.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gkkahmscb.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmredvtni.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gfugxnoyw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gzabuymvf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gdrdiefze.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtqyvetdt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gxhppuyne.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/ghzxqwomo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gusyofzmr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gcfezpqwl.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/ghxofdmrq.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gfbbuxqgl.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gmvcrxqem.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gugnlypzq.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gcpwnrdkt.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/grczhiopf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gmddzvkmt.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gfkcmjmsk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/grktglyqk.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gcutybspp.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gqcbjbblp.sHtML


<!-- 参考信息 -->