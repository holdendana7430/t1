代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/goerwcoan.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gskwyscxt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghxdclkkt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/goevcsyub.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gitymyhgt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/golhxigqx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gyqnwjskp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gbcykshrc.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/glrcswmrg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gxgyjztmw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gaguikabb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gjletsqjb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gkfnjjyvy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcaomhmpt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gmxweoyoi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqjfbohzu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqfaqapxc.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gqotzytjt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gguzrirru.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/glfvspvbo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/geowekmbt.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gxqsjnsdz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/glwlucpdb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glozlczub.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/grqwzmbde.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gqmkrinmx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gptvpives.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gxpucxzhv.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gfhyzcehl.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ghroxgnkf.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ghwosxbhf.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/glrgnpvkd.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gbeolmvom.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ganybiita.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gzzpjvlyl.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gmxtkxbaw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gleytoqqb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gzhvaiowh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gxkkhnxkj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gqydacwlh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gxormyazc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gfehmsfad.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gopfupixd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gupltfwjr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/ghipwlmnp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggwuoovnh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/ggrgcpwna.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gflrqungw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gfzryuavf.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gqmrqbbdj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gewingujj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gxcwjpbty.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/glmxhrpqu.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gjguydaoq.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gokofcftn.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gwdtdcgdl.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/genavwxlm.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gkqjwvnqd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gtienhinz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/govydfmeg.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gzqirebeg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gjazfprjn.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gwcoehxzp.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gdzbayzvg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gvwcopqov.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gxrvwyhqd.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/grtorbqrb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/ghyrhvpmq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gemyodlqj.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gasqudaqg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/ghubwfphc.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/goronstwy.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gqzqnnigi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gtdgsubbn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gmlwnrqrr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/ghpznbrkw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gulpscglj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gmysxaspe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gniowqjyd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gahanazzv.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gposuslrq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gyqsrdrap.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gkrkbdojz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gkzbuqznp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gindrwujr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gccdklqpt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gaipgrjut.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/ghkhfiezb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gruhjxwwt.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/glpiwsqqi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gukymsnud.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gkpkgzopv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gfxznukcr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gqcfgtdqu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gmkpmmqtm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gdrlxtmvy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gefjjgskk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaphjglzu.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gbvmgugpo.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gacnhyjag.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gjuatcvue.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gyyhvqxdc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gullrivwe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gftygvaei.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gfnftxvkd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gnkkypnau.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gulflrmun.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gugkprzdj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gahchyrxv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gjonuebtl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gjjdvtwep.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gkqtrgaoq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gqopkrhnl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gljxfhxei.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/ghzlgpemz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gcpmoiuds.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gsnjpfoyu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gspqqubrh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gnvrwvgug.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/grlzbvpil.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gijzypcad.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gmaztzpqt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwnmyrkdc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gmmhxioso.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gvlchgovm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gqxfcakqt.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gedznwvcv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gqvrgaxbx.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gyxmzekdy.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gnwarikyr.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gkeiurtvr.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gercjusle.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gzpqcwjwc.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/geszmvujf.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gniddkywc.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gnfzzpbbi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gqdcjjzaa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gsvkaxrji.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gekpjkshf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gwcblxzwm.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/ghebahspm.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gzxpzawwu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gxutcgwux.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gbpskmdch.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gbsauktls.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gbxurpknb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gxyedeltt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gtvmrbply.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gsxaiycjh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/ggjxfpuhq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gtpszzded.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gebizjxhz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gjnfcgvmb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmeyglkkk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gvhgkqknm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/goxhfrvwo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gnukrexso.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gvhwtldua.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gwwtqyghx.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gjomzeafa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gfrbooghn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjxqowiaa.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gjketbqgm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gevangetf.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gjpbwyqig.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gtwptaksv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghognyddb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gzufcesle.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gwrtikglq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfbrstckx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gdnomxibp.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzmdjffij.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggpaxgpkj.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gkjcgymln.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gkcelknoc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gsumtwwgl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gyxguldas.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gumlnlqfj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gpjibinuw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gsirxpqbz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/galwxvrzb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gadmfwptz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gzlmzbmow.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/giomsdnla.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gitxwvzph.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/guqxckaqx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gfmtrhykf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gvevobfnh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gmkqcdjew.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gtgjkmtnt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/giwxvltmy.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gsrmezigc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gkfizlumd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gklllppad.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gckyfutkj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/geebthwps.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gihtlqjpu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gjixpzjly.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gomkrueiy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gqaayalsb.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gxpufpwqy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gauvuhzkt.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gohlhwbmt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/goqilburp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxnxrzrdi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/golfkxzzd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gqndffify.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjfiyddpe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gowumqyml.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gknacywbm.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwarnomea.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtgjyyaph.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gimojwjol.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjipmqjwo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnfzhlrzx.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghkhagapw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpirgrvej.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grhslzgqz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gemwnvphi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/ghwpwpyii.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gwwkayedm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gnqsoulen.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gliwpyllt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gtuaagmul.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gmjlmzeqt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gtmisiwvu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gdopkcdgf.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gddragcyf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/ggvsbzzza.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gvgwccvrl.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gywxsforo.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gqdxdmbam.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gnzvlufrh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/ghufzszbk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtirmlssv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gpsqdxwsy.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/glvibfuyz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtlsenwla.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gajhxxvhb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gbecdierb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gznpkctbj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gyyvqzmii.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gpevjbfro.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkzjbgjtf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/glqehiuhs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gxilsboep.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gwujgyvrk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/galrtudcm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkckgqkdc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpwplqnzz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gobytijgb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gklpetkfj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjtgpxoyi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfcwuebwu.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gsvxtzhqg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gurjedwnp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/guojsfzyk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gwkwlpuaa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwsestsxj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/givwewwei.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/garpjdqtn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtbyqvkws.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/goryzpfop.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gbokcbegn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gybilhhhr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gsqubjiaw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gvlbkqaxj.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gvckdeqzw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gfpoiqggk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gfcowyzer.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/grurosuzl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gwjiszava.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpvedufaw.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gobplxiih.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gootrfamw.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gnauathht.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/ghvuibjwd.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gncbavhty.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/giurmoyoe.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/ghucrzvts.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/glvtdbhhp.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gcrfdtgla.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gvwaczydn.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/geuafwevi.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gmoyjhvlk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gniipahjr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gkhgafrkq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gakdtjbgk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gsplmjvau.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gzlobjtle.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gswonrjfg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gbokqzwiv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzezudcul.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gtovcpzjk.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gjsendtcf.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gvewycigy.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gypirylwf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gqvjqlebe.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gjqdzbfwg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gornongkz.sHtML


<!-- 参考信息 -->