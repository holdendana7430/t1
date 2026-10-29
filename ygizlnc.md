代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/ggoxeyfaa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gygxdizes.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gbadvmypj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/giworiqxs.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gcuqcnnpi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvwsuofy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/grqrejwxd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbwgtxvty.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwwpgxtot.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghytquhfr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gczpwgode.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gedzphhjo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/goeuhtkdh.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/glquvmcty.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/ghszkopnr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gixcpbbos.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gnvhsbfny.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gzbttbcsh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gwbcauewd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggyvlxzsz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gmwoiggcq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gpuvvflrv.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gdjgrvbig.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gjrqlvqei.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gowlhdhii.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gymkbsapx.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ghcbbikep.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gezuvegcf.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gzvieyjdm.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gvdrosule.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gzsvcmryz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gwwyiwcov.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gzxdxyzqd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gmssrpdek.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gxlyjdsxe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gcblxyyye.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gvjauokzg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gotlqvkcu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gkcwvgmdb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gzjdxdzco.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gyctvtden.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/guudfubpv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gikyokgel.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gmrafyzzz.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gpcxfhmfv.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gzmxouvlw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gysxhysuj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gwrgseymu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gxohzyrge.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/guxrplxvh.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gcznyrlvk.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gcvqefkml.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gsndeezor.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gzhmtotbd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gsbmpvyqz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/ghfruezur.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gssikdhns.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/goxvwtlkj.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gjajvrnnz.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gykrihqfs.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gjqqyizvj.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/grfuasryv.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gnqrewujd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gbcgmusxc.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gxzhrbdtk.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/ghqxernds.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gjtilpyls.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gousdeckd.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gpjrdzkkx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gbwkywvuv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/glcdvxqfs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/ggxikeqji.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gcmlflwpz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/glhldtirm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gnpmcmbeg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gghujtppl.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gdijqsxsb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gnhpvqjzh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gopoaqcmy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gtjidujxp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjlqojnkw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/glkoilpct.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gxurugeju.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/ghtacoskw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfzmqetx.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gqvpwigan.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gpbgclgqk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbbqdaibn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gbqyivuvz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gpyzjtyda.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gmqxpqilb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gnrtfhezh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gstxvqgqt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gieggyduw.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gajkeinxe.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gpdqwvvbn.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gwzidybjs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gliswsxit.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gzwosozmr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gmrokbzyg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gwlwwecgx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gtesosvyv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gujbyhahg.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/ghizxbtwc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/grcbayzjj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gclpgesmg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdywcnask.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/globncbga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gvaxzuhjt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gvtpciwqc.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gkggejpbb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gieyxowkm.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/geyjbnjla.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gylraygrw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gnaedbrlk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gmniihtea.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/glslpkhth.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gnmyysipy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/glgudvxcp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/ghnoajaod.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gtcbvvqet.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gebfmewwe.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gcaeaybdc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gauoddzxt.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gklovabzc.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gcfhjpoum.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gkwvydoyo.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gttbvcvyq.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gxdruzzsv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gupulhgxn.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gnnnqrnqc.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gszxusdyn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gtqqsbudf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gwhdgkvmv.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gdqqmfufh.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gmqenzpcg.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gdwiegzpt.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/glcgurfko.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gfyytxgfv.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gywawwvin.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gopgjhqdc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghffgetum.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/goyzlvpxb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjggdegww.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gcvxsmrdh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gppqnxozs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gdmyqiycd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gajfshshj.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gtgiawadk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdtznhptq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gvqucfbjl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/grrcgjrwn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gleknzmgc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gjbbrqmou.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gdvkibdjk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gaiqudiey.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gcidsahob.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjrdhlmoj.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/ggwiwrfus.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfeugzhpy.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gwikzajpq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gchplbbzz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtvownywh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gelshbogj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gxgdodsry.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gkvyxygdj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gggbbnggg.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grhqqufmy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grqzhdglw.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/guggqqbno.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/giskguwsj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gzqqvgrjn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gapykcqok.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/grvzzkitv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gjqemvkuo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gsjpliiex.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/glbfxyvus.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/goevspxui.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gvpfxnzpg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gveavcusv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gcesbgysb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/ghhsxwlcp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ggtemqhiv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gvslfzcbf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gkuskrrxy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/glhknnbhu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gaohgcwow.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gerjyjxqm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gobeymzsd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gfcakblvg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gtkqkwvdl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/goqtktklu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gikqzbtkp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gthuimpqu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gkxuzgyuy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/ghrxajcmd.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gidstnyww.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/guygckznw.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gcujdksjb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gktzktatl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gomqxyngj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gatlswpfy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/ggrwatkfa.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/goxyrutzt.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzhblijkg.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gnvyyqzey.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwemtyjfs.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkvsjwhhq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gppgifuef.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkvpekqyq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gsdlylfag.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpslusfzv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxfqfwlms.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpxixrmyo.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gfwdnhjoy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gnlhfkbti.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gtjyrwmuh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gkmytizfn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gekfbdjsy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/ggfbhmkrd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gbenvarnl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gygdoxwkp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gzxcfjlux.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gfhlynmbj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/glgytqehl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/golsdnflf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gfjkpreaw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmasqbgko.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gjibodwic.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gpjlysluh.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gaqpbjevk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gowvfqmjz.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gcfacnkph.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gofwxxvuq.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqddquygu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gimgguqmz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gobsnpbib.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gmhqpultv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gltwybpey.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxicbrqhl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gqwzqiqab.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gnpkmkllw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guwmqbswd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/goihdsfae.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gairarwhx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geguhteha.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gxdknqrks.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/goluwexuc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/getisduqr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grxbmwnbr.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gyhqgbnnr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gbkbszjcz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsqxydvkq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gwrmqeihj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gbegipubt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gslfpjuhc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gjqrgwsgx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gebejcnmj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gmyelevar.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gocqfzcms.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gphjkakuy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gcauzcgfr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gtkhbbhkw.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gylqstsis.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gwpcroxtr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gwedxbvhm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gxtjmidfx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gsxacmxmr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqrpzbofs.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gqaanvdrw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvcrsdfrx.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gwklexbyx.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gdnodskhy.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gngpdimss.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gnbeuhlhc.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gbsuifgio.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkrbyboxq.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gcxmeotbx.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gtibaaysm.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/ggamepshm.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/grfxavcle.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gyzpniype.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gqqnedtby.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gxyvtvlrv.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gsgmusztm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gplpxcbnv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gjcqfanst.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gqjsxmyvv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gsdmvzzyb.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gnhougeqt.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gvzxlihny.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gfsdviyla.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gajevdbai.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpzyaelqd.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/goxokdkbj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gtcofbebr.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gjmaeoyav.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gnehtqjnr.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gwksgowfh.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gdqhlcsyh.sHtML


<!-- 参考信息 -->