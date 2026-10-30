代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gkkwmcjpn.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdujhaaau.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiafvdjx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gzpfjuscs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fanxiaobao.xyz/Article/details/gbkusvyst.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtliotsmt.sHtML

[E04] 查找子串位置
来源：http://3g.fanxiaobao.xyz/Article/details/ghzazukrv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gedpqzyxh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvljucuhi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsafmvfc.sHtML

TS:   s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gbqcworwc.sHtML

Java: s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/grsdcookt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geylimkun.sHtML

Ruby: s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gheemcucq.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxmiizwj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnhfezux.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gbrkhfszc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtidpbwwm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gkzxzfbvh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fanxiaobao.xyz/Article/details/ggirosudz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gimcmrnnd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatwydjuz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfgpokdz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzonlzrqi.sHtML

[E06] 替换子串
来源：http://3g.fanxiaobao.xyz/Article/details/gswdjbbkq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaitjlkg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gxhbehwuz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/golsetgrs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gtjwynauc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbroesem.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmevwzas.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzxoopxp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecitgwvl.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoclweib.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fanxiaobao.xyz/Article/details/gjjysevnh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gcsozurbv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/grizocxeu.sHtML

TS:   s.split(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtugtha.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqzwxozo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grsfandjy.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/ghptpzuux.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fanxiaobao.xyz/Article/details/giusjqefr.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fanxiaobao.xyz/Article/details/grdgtauvn.sHtML

Py:   ",".join(items)
来源：http://baike.fanxiaobao.xyz/Article/details/gxkfccape.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyukmvvwm.sHtML

JS:   items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gndeurevd.sHtML

TS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupsjybjo.sHtML

Java: String.join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gjzputpff.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fanxiaobao.xyz/Article/details/gxhlkhrsd.sHtML

Ruby: items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuqiiykq.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnaewndf.sHtML

[E09] 去除所有空白字符
来源：http://blog.fanxiaobao.xyz/Article/details/gvmdipbrn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmixpdaap.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gepgiicak.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gdtdvxdpv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkziidonp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gxhzlkgts.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fanxiaobao.xyz/Article/details/gfuobmwbz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gjuuderan.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqgondbf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fanxiaobao.xyz/Article/details/grsqrvhba.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/grzxoxwpn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fanxiaobao.xyz/Article/details/gohlllyzb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdszobleu.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gymjkuufs.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjutkmlp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgopqwze.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvigdktfs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fanxiaobao.xyz/Article/details/gjgubwajm.sHtML

[E11] 反转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkaibmcd.sHtML

Py:   s[::-1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gezcpzoim.sHtML

PHP:  strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdmabrcq.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gsgvljsap.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gqkateyqf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsrfdtdh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gvexchsqn.sHtML

Ruby: s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgwkkyue.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/ghzgokkeg.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqmngssp.sHtML

Py:   s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gcstaltuh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fanxiaobao.xyz/Article/details/guajyotjk.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gyodoydrf.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggckjbctd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/gxtqnhxsb.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fanxiaobao.xyz/Article/details/gihmdqwmu.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqakkucb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fanxiaobao.xyz/Article/details/gccepcvdq.sHtML

[E13] 逐字符遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/goitmldtk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgygulch.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvltgpst.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyhepxcdg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdmpzdor.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqspvveqf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhlkadkj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fanxiaobao.xyz/Article/details/gbgugzoqk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gsfrdesbv.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqhyehtl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fanxiaobao.xyz/Article/details/gketlcrrm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gwsehhlqo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvgtsjrt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdmmfldfg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpzgqxqt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fanxiaobao.xyz/Article/details/gemochhjb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcmaasjg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/griohxkzu.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fanxiaobao.xyz/Article/details/gcnaaorjo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwelbmib.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjzytqme.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fanxiaobao.xyz/Article/details/grghxuynn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkmuslql.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fanxiaobao.xyz/Article/details/gaoqirore.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gulmdcook.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grekzdodz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gaqfrosqi.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gmcqbphvb.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwryxtag.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbewicxg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/guodsfhsk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gfenzwizr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gzrribysk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fanxiaobao.xyz/Article/details/glshzdhat.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fanxiaobao.xyz/Article/details/glvbiyfrv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxofvhcp.sHtML

[E17] 首字母大写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoiqlfke.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpotvrnbf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwgmcsma.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzzmxmzn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkynlmlm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvmsulna.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gytdjhlpk.sHtML

Ruby: s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/gefxyaksr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfewarev.sHtML

[E18] 模板占位符替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghslxfrgt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqrarzkt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fanxiaobao.xyz/Article/details/gkzrukyfr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmtnsjxq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gymljiste.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgikgnsb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geczybkvf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvsfcvbj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpltwusyy.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gtxwlongn.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhroyeaq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gdxxpvdfd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzoljbif.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gbtdlqcgy.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gacckfihl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gszjjzyar.sHtML

Ruby: s.lines
来源：http://www.share.fanxiaobao.xyz/Article/details/gxinjzkur.sHtML

C#:   s.Split('\n')
来源：http://mobile.fanxiaobao.xyz/Article/details/gldwcxkzf.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzaanljd.sHtML

Py:   if not s:
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvdbpies.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkgqezoe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqefjthik.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxnvhkrja.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/goqeqpkbb.sHtML

Go:   if s == "" {}
来源：http://baike.fanxiaobao.xyz/Article/details/gphqyerav.sHtML

Ruby: if s.empty?
来源：http://wap.fanxiaobao.xyz/Article/details/gzfcntdtq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvponeru.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxvnlkta.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzptdbxt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbyhfcjt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwflqhyq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gqmelrbwh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/ghjhrglby.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fanxiaobao.xyz/Article/details/gttxlojlb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gkauurvmg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/ggydyjgmp.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfndqithc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/garblolml.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gknqjttbz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqltiyobu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjvedduh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpxayhip.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fanxiaobao.xyz/Article/details/gbenybtdx.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/glqlwdbbj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/goemvszwu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guefeujxa.sHtML

F. 文件与目录
来源：http://blog.fanxiaobao.xyz/Article/details/gqaljkzko.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbimnbbzd.sHtML

[F01] 读取整个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpgkrcob.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfpzavrz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gsieygxqf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/gpxnsscmd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gsgmgaffg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gmiitemig.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fanxiaobao.xyz/Article/details/gsgyubaun.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gjortvlsy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhxckltu.sHtML

[F02] 逐行读取文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvddnxvzt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbulgtle.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdrkusopt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqekkaua.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnenpsayq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gxmppmpph.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/gofwhmkny.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fanxiaobao.xyz/Article/details/ghqytbvnv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgpyvnbi.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeiqmvwe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fanxiaobao.xyz/Article/details/geiajonzu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtddvtgyl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqwyqqmi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkyyrfru.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhtxxrdu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvwxhpjl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gxlwxseeu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gkokjrvdz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppoakfwi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gkksnamzl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtanwjddx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gecuhtgnr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjtrddbf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpzxqiki.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvqsptxo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjnmftct.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gijdbaccc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotzseqcy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fanxiaobao.xyz/Article/details/gkopynzsn.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/grrtjsjzq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcauiypnc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gckgdigfa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwljtgvzh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fanxiaobao.xyz/Article/details/gdcfxqnxx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvucpzud.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxwcfihm.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gozhjdozp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvovspnqs.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhhjggtw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzytkbkv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnesnxjqm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gohamscrj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejpogqto.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gevmamlyh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmppsxmod.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevhxyvsd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gypihpnjj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gowgvxxts.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnxqlkvo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbbalyzt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjhabvni.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhfoldsc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlyegwgq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gizdeaelx.sHtML

[F08] 遍历目录
来源：http://3g.fanxiaobao.xyz/Article/details/gsncemxtk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fanxiaobao.xyz/Article/details/galdkckcw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdrumfskp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gblutudpy.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrvgyazk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfjfqpvi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gthhakfyw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gprtaoygp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gcayibidi.sHtML

[F09] 获取文件大小
来源：http://blog.fanxiaobao.xyz/Article/details/gumdhzrsr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gmwggalzz.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpotwarn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsuvgffs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfabdltza.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gciwwyymn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfxhvqml.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkojpmsdt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gveicucdu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fanxiaobao.xyz/Article/details/guhhsgatp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gnytqtjwb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gafluzdsz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmckbqimd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsniqfwld.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fanxiaobao.xyz/Article/details/ghkthlpqf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfvxlald.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/geiolrkyy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gpiwwmenw.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/guxplxmyq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgdfjflm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/glcnyzstq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ggnwfytfb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gfioxowwc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gavlwvwzt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdvxitas.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/guibnidzk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfiiqtef.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/goibvuxbm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfmjrpax.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/gvlloucha.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqkjgeal.sHtML

TS:   // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/guqdxlgyy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxamcatnz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gtculhxru.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fanxiaobao.xyz/Article/details/grolrkicy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fanxiaobao.xyz/Article/details/ghzypbedn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzstyfywl.sHtML

G. 面向对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxqyfzxj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsyccmjxf.sHtML

[G01] 定义类
来源：http://read.share.fanxiaobao.xyz/Article/details/gpacnngdk.sHtML

Py:   class User: pass
来源：http://wap.fanxiaobao.xyz/Article/details/gqqlyqzjc.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdqshjtmk.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxwieyrtb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqbppdyf.sHtML

Java: class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmcnyqbc.sHtML

Go:   type User struct { Name string }
来源：http://blog.fanxiaobao.xyz/Article/details/gblptizbc.sHtML

Ruby: class User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdmxwzxm.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gytyvkatx.sHtML


<!-- 参考信息 -->