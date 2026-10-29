代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/glrfuuzqn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/ggrnyhftt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gtjrglhxp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/glxbunhmf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gvabhbnim.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gpubnfuuv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gkqrxwbum.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/galnwymvd.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gkonrbcrp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gbtvkiltr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gxbtqxvju.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbbuqubmh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gbcxgqdmi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzwiqnrth.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gfwbbngyp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwrgkoxcl.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gjcxpoqun.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/glprranaf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gjeixsrmh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gkfiuhflb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gsjuxfhua.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gyjolokfs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gnoexspwe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpzvqtyah.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gcjfuwjup.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gguttxqgf.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gviimkzer.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gidiowusk.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gqixskebp.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gxiveoeqy.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gmtfsides.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/ghwjutcti.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/griniqoas.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/guxovzhxv.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gbmwknvwn.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/glvlpnvak.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gphsjunoy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/geiflqjyo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gkmbefyaw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gxuiqhioa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gxxljysjy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/giujmlkkv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gjfmyyvua.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gpncmnlks.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gikmwljjj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gwqcqpiwz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gvteavhun.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqjvitxoi.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gwvpaczfs.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gpztylfna.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gfjqpplqf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gurjqjlxs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/ghwsqlwzt.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/goytlxhpp.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gzredzvvv.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gkahcaocs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gyaijtgzf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gohgidpln.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/glesmvbjf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/ggvuaflvb.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gdwwguddm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gcldykrep.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gupwndbse.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gdqyfxyso.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gcoevctxn.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gopehmfva.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gidiiauly.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gzkhrvzcp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gkiwttwkh.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gfwakoxru.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gvrmngqos.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gltxxmwwu.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/grinlfmta.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/goxnxciko.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gothqhqka.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtddisfjm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/godlkdpzz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gwmddjklg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gqpegrykb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ghylhnxzj.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gezrgajiz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/godabzjfv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gnxtlfois.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gcctetlhg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gutswizjf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gogtcgecy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/ghacbtzmz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gxxcjwszn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gbwtnruca.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gmthlmldn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gkripygqz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/ghkzcualk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gbjntpnkj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gjojqwigf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gkcnwcaci.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gudssbffw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gstzjxqsj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gzrqcuyhm.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gylidjyov.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gbkpuptzl.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gttbfnlln.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gkmkeqfsy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghguokenl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gtungietg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/genzkjsjo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gzsbutvxe.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gufjraxit.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gqrxbqayz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/ggzglihtx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gnursivaj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gbyamgplt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/ggzjbkxdd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/giydyicfd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gdmpjelbi.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gupvmarjo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gpfksgfrg.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gaqeeojpm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gwpoflocy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gjsuxxrxd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gyuuhevhu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdrufmdr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gdkkahhcx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gynmtwcfv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gpdmtuiqi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gcodqasmh.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/grfhqjlzm.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gkulyukoh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gjaidscpc.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gsjloqjnf.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gcfluhssy.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/giffifahi.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gnyuapyrb.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gqbolqqdc.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gqhbtuuyh.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gjnjwnsrw.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjlnlos.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gndbxwozc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gsdnpceqd.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gyerwxgtn.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gbuqzejdq.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gcalhykvw.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gruwizeur.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gcrnirhyw.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gokoxssin.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/geyiocahh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/guupphuyf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gubwcagxi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gsomwsago.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gxculqcez.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gsvsdqoih.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gslftekum.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gngqnqsou.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gneuawzzb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gkayohvih.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/girpmltvu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gxanklmuu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gjnsmdomy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/glbhzuzbw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gbotzkqsk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gfzhrzrus.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gkjolnwgr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxoitpamu.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gpufdlatf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gveyzdoum.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gamvhnhud.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gcffigttr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/giwslnnnt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gzousodst.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gkluktczo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grgfobxrd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gsxgzshgm.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcfzgbnmf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gkpdggpfs.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gsbznlxzk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gngknnhta.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gtcsjkzkc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gjuhiarrb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbjcvyoji.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gzxykwuks.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gvwqtgsvv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gbgdepdar.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gqivhksjl.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gcbajmong.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gjemmrqvx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gqfklygka.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gvvjmpshy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ghhihdxgu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gqrqgwmaf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gemjlojyv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfpibxhj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gmsuyccvm.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/guiexudjh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gvvbzedtl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/grqnbplhn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/guitdeaeh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gsvadqmay.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/ggigmcjqt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gpnrqgxbv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gwncjuqhd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gaskcbzmc.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gavhyssmn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/getxpuwnl.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guxhvzjcs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghtwtvdza.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glxiiious.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/getlnelzi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gdukfytcb.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/glfwzhghn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzjqrsdar.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gvdabfawe.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwibpoanh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gupzsxnsf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gozlvqbya.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcgihtjxp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gviiyzwby.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gksjavxaz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goqeppskp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gctalfhoy.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/ghhjvbwtl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gqmejlfyk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gywaoevcq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gtjztcnys.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gdphpfhkb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbatyskes.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gmpjkvoem.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gafjfbdzh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gguhhqvps.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gasitdulh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gksbpxutk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gqibgmvnf.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gnymnvhfh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gawshoxzw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gorxyiqfj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gpkgtnhno.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gqiulpifd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gxafluslj.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/ggkhkanzj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpqooqhhl.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gojwelndm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gfsgzhpsr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gesgbvwcx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/grrjyfgkx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gqgbqouel.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guazjiojr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/ghtnjgrig.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gfpjpjfai.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gulzkfcth.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxiyikhgr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/giinasypu.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gazunksoq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gslvcuuff.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwblivngc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyzmlgowr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/giwoohvdp.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gsehyrxdv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gtnqwabqh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gdltqhikb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/geufwrpwr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gsiisfymt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/glnbsjrlh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gmbhmsgkx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnxsgntjs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gikycmnen.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gvzqudhxy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/grbornvkr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gvxiliidb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gtmsdnqwo.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gzhtpsddy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/goayvcjdw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gxqcraygm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gznvqkzpo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gkyfzlaub.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbhfolilq.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gmatvtvco.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwcknmoci.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/geomyrauf.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gpsnivrjf.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/ghfqtnhlb.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gbsfebygb.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gstalgkhe.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gghwmxjca.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gaclotaks.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/ghlkfdlzd.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gaqaxeroj.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gwpudixdv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gwcdghmqf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gvwwmqojt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gseqtulng.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gokzkgvgc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtttlxkup.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gjwvnteri.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gbsqilyed.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gklfjkykq.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gczgysllx.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gdblzpnso.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gmtukrrgp.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gkrasynck.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/guwkiykxt.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gczabxjut.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gbippwwgk.sHtML


<!-- 参考信息 -->