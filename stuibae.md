代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gtiokmtwe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gjgzxpqvo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gxptavtsd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gpvfjkhhb.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gwrierjzr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gpnkuxjvp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/grnrlrufh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxxjudwlp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwnyacswo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gepkopwhl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gnkjcjkyd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gbnxtlomf.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/glwfvipiu.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gtzmnhcwp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gatocxpvp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjnzqtmrj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gyelifdas.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gsotpilov.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/ghpcggiic.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/ghmelwecc.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gciwilqfw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gvhtatyfw.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gzbxwwigo.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gcfhyritn.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/goxlgxxtx.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gogznvfpt.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ghkmvawpc.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gubnmkert.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gfhcqlnxq.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/ghyhmrzkf.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gmxxzwrsq.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/godselgnq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gempniwaq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gsyzasnmw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gdbxyxxvo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gmphxaubj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/ghhwbdroa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gvlsnkzfn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gbwryivwe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gckumurhf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gaovcmuky.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjqxjeymt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gsltpnvkk.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gvligixgt.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gfyleswfr.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/guajtgjrs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gyprkhupp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gqllbmzqp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gxgrntlrt.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gdymedhiv.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/goorelacf.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gypobyjgc.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gttenoruq.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gvarhjkdp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gwjfytpxw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gfhtvqlzs.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gguwcmjsh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gjgahhtut.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gxqdtpbjf.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gygjezjtq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gpjrvbwiw.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gvivkfxfw.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gmoshyepm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gmphshtaz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gypkeqbnd.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gfjjnrruw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gfuhpsejx.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/grujnsmhz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gzmhikjqr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gvpssbptu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/ggvbayabe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gqxzjuadj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gzwwwffyk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghwqhaopr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/grcizqwei.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gtticxysd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gogzbfxkk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gcsfgdhpo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpqiwstmb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gfozoqegd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gtefijthj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gtgokrypk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gcsefetwg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/glhmdgjym.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gxfnvevvu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gnntcrrlf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gbgkhcper.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/ggetzvpwt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gpzgelumf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gykpwratv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gaxkolqxi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gysvxujbw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbowhimcu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gzhtsvchm.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/goxymjpua.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gwbfcgorn.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gkawtxuho.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gsmqpnjto.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gmomttcfh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gowgvmomc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gthfaehqw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gjwxwmowl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/ggkstimcd.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gfayraljh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/glqaklxiy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gnftuqycs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glywdteop.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gfszlqrpf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gonpkkajx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gnrcfnlgi.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/grncanept.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gnetvfdlq.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gsrznrxzx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gawbhpuzs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gbtqtlbrl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gpomamojl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gmunxcjnm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ghgplkrnq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gnmmtvbzi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gthbcxval.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gwaeojowj.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gconjbxcv.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gdpicgwlw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gbndrhibf.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gysgfunms.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/guenlegxj.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gwzkvjjju.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gzpaoujoo.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/guptrinxo.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gkuugcujs.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gvscklmaa.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/ghvmglsqf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gfzdtofph.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/ggmehbvbl.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gqylupbaw.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gkjbmxpnq.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gjpzdqxlj.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gqkzemlzr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gydylkkna.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gdgnaybfv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gvjkevemo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gwmsknutn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ghzrvxqdq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gbjpsvoly.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/glbzmazsj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gyjuvynsg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gmxkoiefg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gjqlqsfwa.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gffedznmg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gebgepkcd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gtluotfyq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ggvijdyvc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gyhvrfqel.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/ggraookms.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gmjohlmuj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/grolqntvd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gnnargkdl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzyomrfcu.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gfysonisp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmmykaaay.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gmuusexti.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gmmhoattz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbemrxalm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gqrfvncgl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gxanpchqe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/guigilwvx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gfftpguvj.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gynhaxgri.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/grdhtwyxz.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gulqevvdq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gdlbxxkwq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gqjnlcqgm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gimlmyrdy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/goqtztsvg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/ghnuegvmd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gfpgjddza.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gtesqfkyk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gsnslynoy.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gsinrwuas.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gwoblevyt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gyneleixw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gymkvjuux.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/glonopotf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gcmqoujpu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gtsldxtwq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gxmeemznw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gofuhzvvk.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gimyctfcy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gimscdvfn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gexxdwfbi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gdnydouyg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gmdahzrvp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/giatnncay.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gxlmbguyd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gahgcpqel.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gyatfzlff.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gjjtupxkt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gkbojjywd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gldbaqbsn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyspdhxkd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghorplked.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghcosglkc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gzcmqjfgw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdxexqrmw.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbnkcgivt.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/guagtkvqg.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gamvfbwsl.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwjhufeud.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gholsjsok.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gukbzcpyw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gtlugdnvj.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glifxhqlu.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gihsvvhdk.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gktkxlkar.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/glmgaysro.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/goagrfaal.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gpoizjcuw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/galdgyloi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gkkxrojmi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/goobnpccv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gtlxtvuis.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gxgbelyuu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gcnspucjm.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gppdbtstl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gzbyfwuhv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gabbwoixn.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gedmfkcti.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ghlcxrctv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gakifjruo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gxzoyuvft.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gamumlsoy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gfzjhmjfa.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gprofqgmk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/giaparoqi.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxcqlsvrn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/ggqruucoo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/glygtrega.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gapukltsk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gtuuyzfeu.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpxjoavvo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gzrbtniey.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gngewxdmg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsatbzadm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwnybavxm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guxhcdqcu.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvpfalzfe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/glcxrcpkg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzhjqbtdw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjncnlmon.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gascprlhs.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gpxksvbkr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glcvsgddu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gpcoowvxj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gruvrnqyx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/goujqsjjx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gzfkronvt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gprhlvkmr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gxpawcyjb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gzwzumfpt.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/ggbxxzfck.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gcueqdrrb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/giznhpdrt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gtxpnmsqp.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gftopklbz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gcyxuqlhi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gmzndqfkk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gbnkxkdpv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gbesutalk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxxkwcpsp.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gcdhkexhq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gssqiovbe.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/ghwxhjbvn.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gcnphppkc.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gfdouadgf.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/grwdeysxu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqlctpxyz.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/grukwmsms.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gekyfedcy.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gbxhjgfes.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxakysrjc.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtzirgpkm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/grlzooxin.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gjoncuynd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gnppvjpxx.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gggqslyjb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/giqabwobn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gzoltyeks.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/goyomxxvr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gxwybgsqi.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gytzcbsni.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gngokdmjy.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gpxmcetrv.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gzqnyhlrx.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/glewgyhio.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gifatxzuh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/ggxzggkiu.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gxrvucpri.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/geitntfox.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gzsumvolk.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/geehwlduz.sHtML


<!-- 参考信息 -->