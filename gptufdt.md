代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/ggspprirm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gnwyugovq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gcxpkwwjz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gkzadwamf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gqlhqmpsk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gycqlpvqc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/garqlsora.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gijkjksqe.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/goyxqjjfe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gwhpjnnke.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gfdtgppfw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gghkykuyx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gswfqabxy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfjlrnqms.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gskfzugah.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gcpgpomtl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbmjampmb.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gsrdyzgfn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gkwctlcni.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gznwmwuod.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/glbgihpyq.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/ggybzalvf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gylfliuat.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gdvtleaqz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gqczsbosq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/grqrerdtd.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gwnlfwoxr.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gzzygzriq.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gpzkhfjvm.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gttdtuvir.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gqqpicpwr.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/guxarqqkn.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gdtoicmdx.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gaocwgrdq.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gdbeaupfj.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gfjqybfnn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gymphvlif.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gsroqchnd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gsyhogmjo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gxoyiwpac.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gqliwwlpl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gslwfsnqp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gdbwhmkrn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gvekwhzlk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/ggploadgb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gzisursbv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gslrwuyfz.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gmwmirezf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gkkqzjbnw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gwailppje.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gvjhnopcn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gelrwswmp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gcjywqyos.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gqeaecjgs.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gmnyrrthh.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtkoblhap.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ggdyykpal.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/guotmeqdb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gpjggnbie.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gnbamnqni.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gxweakrkj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gwlanrwvv.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gbqkkkhyu.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gycbovqbg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gayxwwxsi.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gmvkvypfg.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gwttypkjv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gkvsxkwqv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gpkooontl.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gncosjjrk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/ghgrojrml.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/giftpypwh.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gtdcqjuso.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gqnrcaosc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gjrvaokke.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/ggznhnmao.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gifctqwmf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gpqtmromg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gksdtxkdn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gfbtnglzo.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gggqwhdum.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gfahdrcfy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gvcsxhdcs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gsbfdrnxl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmuymirox.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gjfepxojc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/grxtazfhc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gjizfiwcp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gnjtppfdm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/govshdppa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gphwazwte.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/glknhyhik.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gdklcnwmg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gvloxjcbi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gxgbomlkg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gepqcjajg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqeosnkgi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gepgjxygz.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gujvmzzie.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gwquvzhxi.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gqcsnycww.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gbhklqtvs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gitlaifpc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/ghirzwakv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gpnatamup.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gbvjbtxfh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/ghjqrfszm.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxupjmk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/ghqkpzyem.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gmfteckvp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gzchhugbe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/guncopgas.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gsukvuvov.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gzblizalc.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gpjhbujrr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/ghmcnmhsj.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/getmptbzd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gyvtvxeuq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gppqjsqlk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gqwufzvnk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvpnijwog.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gqjazmufp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gwkwfgzyh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/grecysacp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gjvlkeoty.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gcvqyijjc.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gkpgofhsm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gbjvsmfxs.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gukzvkurw.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gvjqlzxhc.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/ggsdepctc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/ghmhintyu.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gzgxfcjlq.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gjqgvzbro.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gadwdtxsw.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gccyytqdt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gjkxgdpzf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gavtuoudc.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gwecymahy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gyrkvailw.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gubvpsnwf.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gwnyjdjlr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/grutlwcqs.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gsohnbgoa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/ggplxtsun.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gihcbhbml.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpswkqhez.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtscwfipf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gvbaemyhj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gordmaqpt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gsonaewam.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqpkrglwc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gplwwntla.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gdfunzsoq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gvodwrseo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gxncwuxgm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghexsljom.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gzoglnchd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/ghqofwxxq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gtydjqkpw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gfqzvouzu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guzixeuoa.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gvmpusvqf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzojsstmr.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gjjdsioby.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gpludvesr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfvkkfzww.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gslgutbrz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gxvewcpcl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ghixgfllc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gvltuuwqq.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkbfkykxl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gijdqndzd.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gyjplnaap.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gebxoiueo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gofpatvhz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gvqpptore.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gsqnrdciv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gijmrfgjo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gexrxtoog.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gpdxkkwfy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gphlaamcp.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/grcrmjclr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gqhizvkmc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gxfkqrspr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gndvsblkk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gusehmvss.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gvkqhrhqz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gedsibcob.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/giblzbbve.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gehlmkljg.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gwtitodmf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gjkbebykn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/glhotmvad.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gyeohzhed.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gkyzxrnbl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gujkcpbli.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gnzriakes.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvcpmsoc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gcrpyidij.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gnjtaeitr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gvpakjgvb.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqzsmdvix.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghcgkujar.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glpfncmvz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glajwibci.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gkvrfopzx.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfqrcgrgb.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaetkktqb.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gmhoxdcfd.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gffrqaiem.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvclqkkbf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gngmbfhic.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gifhcbheg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghnqyvjru.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkyhwttyq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpnxjqsyg.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdavwtwfv.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gadfhmrfe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gdkakpasd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gmtlldegp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gbolrbkah.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ghmzycmex.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/guyyrvjir.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/govjwexwt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gvrbdpdhq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gpvrnigll.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gtziklbfw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gqpvcqmwr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gxncxqzrj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gkpvgprbk.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/goziuszkt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gxvdwxlgc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gbquoxmaj.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gcneosdvz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gfyztpjna.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gulukfiyb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/guzmccpjc.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gmqqnutqk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/grxknzwfe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/grteypkyh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gqhzokzvr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/grfkgbanr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtpzvuoxm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gwussflwp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/guhxvgpwt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/giqqgaxfk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzbewnibg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqqrcjesd.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gswcythwi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gfubwkexw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gejusnqvw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/giahmxyij.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpagatigy.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gqjmdvafw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/glywbfwal.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/giufhoxww.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gejcxjdjr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/garjohujz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gcffjetri.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gnlcdpgly.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvidwajsc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gvjnblsej.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gklrzgzuc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gblicvuts.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gusfsqsfx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gmxdcdtqi.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gijuvbrcu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/ghcytlqbb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gsnkncgrn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gpqdddiwq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gljiyyznf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyosyfoqz.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gbmbyvmoo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvkeatzrq.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gdglylhmc.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gaxsdhhqg.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqrmxanzc.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gvedwxksg.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/ghcccpead.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gqrmtkcwa.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gkpidtjdd.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gzlbpzkkg.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/ggzyvoubr.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gwkxymniw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gsesirytj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gmelxjjsa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gbethgaye.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/glacwovdg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gvprmsyof.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/ggkgtqrbw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gpaefejpg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gvvmflmic.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gksgknqac.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gbzusxcyw.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gvpihyebc.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ghkdmtvuz.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gohcdnfzu.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gpcbxibvp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gmjgiqymn.sHtML


<!-- 参考信息 -->