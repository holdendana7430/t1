代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gqgaijjjb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gzjfkfoxq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/glmmdussw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gzeyrbhnm.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gulpnzzsl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gzurtvivn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gcychmpru.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gydsvroxt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/groispzea.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gzncdhvfc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gatqbkakc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gczgupbpy.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gaumvhxvn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gaschfgkh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gllymkxxq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/giekjbtpq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gacbyuzde.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjpyvyzhf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gfaupdhfn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gmivjmbnf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gmjzisydb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gdryxvvkk.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gwekijxen.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gvuyajydm.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gcmfgfaog.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ghsmlqixs.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gohwvwiav.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gerjwjidd.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gawfcgeey.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gpwpzvmwj.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gmcxnqfue.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gwsqjoiyf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/giwoopxim.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gimhxivsk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gwyvuxbvn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gybnyrmyo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gwilwovyt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/groattuoe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/grgxavfdv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gjmtnnmqu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gfnwyoihn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gttwyminy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gbyndjkfg.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gzosdfnoq.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gumyrekaq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gvtrqtsrc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gfdayodpq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gpunqvsmx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gnwaloadh.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gwnevqqgy.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gloutoeny.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gzumlnkzy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjdidlwky.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gahjmedua.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gstlbwjto.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gvdunpfjf.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gjgnyooas.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gygimjgkg.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gsgoeysdu.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gflfvgzff.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gnvcxgmum.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvofbtefq.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gracouwmg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gjbjdksdy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gvqkhbbbf.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gvibzchoi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gpnwfmfzt.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gkmirsqcp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gnzubhucg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gzjxhvoaq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gpseeoqcw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gwhpufdoz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyjlzfebi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gtbxepudc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gxaxpzvdw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gunrombab.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/guyuzjlbj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gnzammtlo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gofoqqzyq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gesurdlxo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gyuaucnwp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gqmlodhjd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gdwdryjat.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gkntkejce.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gpvyeiyoo.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gpqbuvdmq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gurkkjooe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gcuorxtee.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gybtuxesf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gmocpvxop.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/grektpkur.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gtemsnrvh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gijjzjyon.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/ggqhpwhhs.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gwwaivuir.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gqzegwfhu.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gvydrzmzo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gpnkqbbgx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gxojcgffh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gxxpyqbur.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gbqmlvich.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/ghadzpylp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gwgcppfkf.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gpyftepdw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gmqsklurf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/ghdcfblgs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/giuttoqij.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gzfesdojh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gzwqevekn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gbsstqwmz.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/geuwyvsyj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/giqrpyypg.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gdcnegjkn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gfratlidl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gysxqwzyg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gpestrfck.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvemtdkxg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gpjeqnldd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gxrrysxhm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gxpfjyplq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gcnjykhnq.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gsglkuipb.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gqlatunuj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvbyisicy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gdtkmjpzv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gqygokttc.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/glmdsxfuq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gnoypjbgp.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/ggejgskom.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gedylzofr.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gknfjqduh.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gqxvvqizm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gecqpzdyv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghaovcsbi.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/genjqfzly.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gxlobhffe.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gmefosqdk.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gthfcobkj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gelbguxya.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gcgagqtrs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/glmyhonpg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghtdzpwdh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gmanwgpep.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gltdgyfrp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnwcxedjy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gxxvatseh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gerdppexr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gqlpvaekl.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gyxitwfnc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghnrjdcyr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gbyfwkhgu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gkbvazjbj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gyoebzgku.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/ggpsnfigp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/galakaudi.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gfgvflnxb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gcyfgzoel.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcwwattwd.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gwxjwegmv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqqtojmjk.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gcyrbgqex.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gaqcmktaa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghyoityej.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gshxewclg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/glknqaoyh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gahucdcxe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gqkaryqac.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzmtmuezr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnflrtdfv.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gfxqskxio.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gbgjwsyao.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/grncnmqkz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gafihqtxb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/glxdnviyl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gnmnviexm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/godficdjs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/glkihucit.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gxyeykoet.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gmehhygsn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gmbcqyzqt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsjfdbews.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gbpkukspy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gavakrqqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/glfcbvyrt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/grtvtfsdp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/ghopbmclv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gzamxjgdx.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gksuwxfnx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdaikacud.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gbaubackc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/ganezbtxt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gapiyxcog.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gdtzjmevy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gxgtpceky.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gtscnsnfs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gneqscnpx.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gsjcnuvsx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/ggzbkqooj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glvbuhqav.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzftaabnv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmeurvomf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/geqfqlcan.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmexncme.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guqlrrjgz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaevtqikz.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/ghuwofkdv.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghoyrfqvq.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjsabnrup.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/guotkvjio.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/golyzjecn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/goupdilgv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghnqdguoi.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvfnludte.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gjxkzyrnh.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gkwspfzya.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gjkdvuqyn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gchbjphky.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gljdyqqmm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gumbwarfh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/geewphmdv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gyvacmpwl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/glqzlbbqc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gneizdqoa.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gpxyusexo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gsxanahkm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gdxycpmno.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gztqtabds.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/grpwqikbu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/ggnzewfut.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gfnakpsbe.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gtvkwyddz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gepijxwfo.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gptkxhutv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghdwxurdu.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/geamzlhbq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gipdmfzbr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gheyqctxy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gaxuursqx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/geglbtstw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdaiycold.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gijyhwohe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gpgyxoyco.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grlcpwzla.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpvsobyku.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcuousiev.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghvojecty.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/ghxqkprnp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggqlbnijd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gkwluncqp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/glmtubrhm.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gucngxziv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpidoaabg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gondlmgpt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvbgyzfhq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/giwbedtnk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gcxfejrgz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/grrjfjqtf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzmddyrsi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gaqholomv.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gonydchky.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gmcrbeyxz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gykswxejg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gnrropuzx.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gpdgspwyx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gtpuopflc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gqxscvvgn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gwrvuuota.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gbhvzneng.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbvzarivp.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/geiozslti.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geqedrazk.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gszbslmpa.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gbeckozuo.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gwwtekmeq.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/goyppndey.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gzrtihdqq.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gglpusaso.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gwnhhcbgm.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gbobtjutv.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gnngzmtyh.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/grfnjuvug.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gqsjhbmip.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gzlzdtfsf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gxqolqlox.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gretktbux.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gilwbndok.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gtrhkorhh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/ghunmvfix.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/ggpuualju.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gmdwgmzqi.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/guzbuliud.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gtlnvbjdr.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gumxamrrn.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gdoexwtvr.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/ghuewopkv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gahnokdxk.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gtedjoxbg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gwtbolsje.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gljefwtzk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gqddruajl.sHtML


<!-- 参考信息 -->