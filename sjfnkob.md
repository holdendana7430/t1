代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gsxywiufw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gngmkjfwr.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gfpmycoff.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gegrxqlka.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/glszjdjou.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/givgswpwc.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gxwdauphl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gpdiibypj.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gqbdohbfq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gtewskqtn.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/guokndszc.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gtmxuazyi.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/ggufkedkd.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gdgykytau.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gucdpjcpx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gforxczwb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gelbczitn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gleqszsbe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/giwhzteky.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gafsniqmg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzieojfxf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/garlcovnu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gnmydrsgk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gjdilpgti.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gwmwzyizj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ghqjenadn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gldwbaypc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gbqgikhyj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxolwvf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/glwnqpqru.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gglyhmcdm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/grymjyknj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcooxhzip.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gclmedxxr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gnsplsexk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmxpkxrdc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/grcvbndli.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gocsykjli.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/geulptefu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gglgknndy.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gajwkuxfe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gxhtmojvb.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gynvxpkcr.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gttuhuhfy.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gfdkfbpyc.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gpdcsfejd.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gsjavzmph.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gqixbltur.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gwszzsqex.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gvcobzyit.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gazexootw.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gqhjiawnd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gjvyqhqum.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gadueueuu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gqwnnotku.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gjqdorebq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gmnewtyax.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/ghhqlhaks.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gmgnhsiec.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gzhbdnzkg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gfloatgje.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gfyguzict.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gavbtullm.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gvffheixo.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gfbjnegpg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/guccxnsas.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gbnaiwcin.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gtfapsdtw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gbsrkghkt.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gzuydjhwt.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gjmainpld.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsnqwjrzu.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gpjnnuhjy.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpxezgcma.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gsdfqlqby.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gmzkncsej.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gfxkivjtx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gduatwehe.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gmvhgfbjn.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/grlqxaxug.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gfavbbyvh.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gcvytrnbe.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gnxkyvenh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gsvoeocgk.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gvaceupxo.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gxnugltex.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/grktkkeby.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gvyreqfxp.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gqrhrtigk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gwscsyvyh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gkhxtteyg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gnglduvjm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gcxlmewno.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gquqxqsji.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gnucbxklt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyzuztngt.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gghtxrvrd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gdwwnvyvz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gnrrmuulm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gzpaaqoio.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpocujuqx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gzfdpzxms.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gcvqiuwzg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gerggnlmu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gcrrcziyh.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gwzvzumrr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gyruwtyit.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gyhqdexnt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gfxndiono.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gcuudomcz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gyvnhxdkh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gveeywzhm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gdavrengz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghonnfsbj.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gfwolsskb.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gfphdamdf.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gtwyubixv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gsnsgmrhm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gzlfcxbml.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gaxbcigff.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gpacbsnmv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gojvgeqzx.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/ghalspxce.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gxytdtjzt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gjgcwnrkf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gycwdbraw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/ghfeurlnz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/ggwmdhiqd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/glviffedw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gvuuimxtc.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gfjymfuqw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gzssqvpnm.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gtjwlltvl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/ggkgvzbup.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gzxxfpzha.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/guxvinxih.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gmzxpsjab.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gkuycnibj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gatebfisi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gmwdlgfuk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gnnwwmrxb.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gtwdhvdcm.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/graodicuq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/grhqorevq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gmmktrcwt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gwfeqkolk.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gaibopupf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/glpwaojqo.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gffiryttw.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/goiciosmh.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/ghtmnjilw.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gfwqxyykx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gksvfnoaz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/grewoyeqr.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gwaarzima.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gjcfpcnth.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gijbinskx.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gbfbieiii.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gmqurtxfq.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gefzvkfim.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gkdvhzclr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gwtlckjvb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ghaefkiyp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gonkuwtrx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gikqfhkyt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gyidhdoqh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gvzunxohz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gvmprgcph.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/giddljntj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gfjjtoffx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gqzwxllcw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gjlortdzq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gfktvcrfe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/ggqyhdfyx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gimulayyn.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwrfcwtye.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gklegxbky.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grvnslasb.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gqnkmbfvg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpkyukifz.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gqzygtbuq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gilrofnuo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxojyfpsj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gwhxbquxd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gvnzmxwcv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gyzpbbpib.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gtjpkwvmq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gixjcetvq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwopdpfhi.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/govjuxmii.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gvtvtfmnk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gqyhdcxbj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gizqpzybz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzimmfbdy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gzbihqmjm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/ghileyrhq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gkwczjhyw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/goivjrygy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/ghpegndyl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gptahsclb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/glsxpphrr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gtgyrynvr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/glrsjhtnr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gfmbcysjw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gqxhlqxqn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gciexcegp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gchdbcpjj.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gbvjagivk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gywyqhkra.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gnyyijqki.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnvouxagu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gtsoxsgha.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gbduidinn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gcqpifrlt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gxuaoistg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gglnjshzx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gdpbcnwoy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gzrqustzy.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gddsigwsk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtxngcjnw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjlwykrbk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpjepbmdr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gighkjpjk.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grmfbbdda.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gplyznlog.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/geefdnrcg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gicrutkrp.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/geaamtoou.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grusoxaic.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzxaoahzk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/glrsghwxw.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqmwwqteu.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/garnskxsm.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghmaiyxkc.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gudwamnim.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gybqskgyy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gedfhbhqc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gewfqcgvn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gewlfjyrh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gacjutfge.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/ghcxweruy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gjmlfompo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/guvqbcwfn.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gmivzkbnu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gwndndizl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gtusvnidk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gelhoitco.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gcqdxhqca.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gszbgxwgn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/glktdvuwc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gswhsxkfb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gqenavfax.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/ggzcpijxa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsbdysxgg.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsbswjrqr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gdlgvvuox.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gobnslzkj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqdehchsw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gqdvknqrs.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guewsnzfk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gdoctussb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gwgnwmyec.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggobdwgbs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnnlwncnw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsdatkxba.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gopbzwtxu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gsatnyewl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guqjdgfpm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gysmvutas.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gtqyhghpx.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gvlxrcrah.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/glxgobwqk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpxpaarzk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gidverhcs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmqcbkbze.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gdkqantih.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gkqjzsigo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfnigdbla.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gtdooqhcs.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/guklhlfly.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gqfbnamby.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/govdcodzb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gegtbipnd.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gwhkpmgga.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/ghxzgisbo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gaexrmwsj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gmrspyqms.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gbofadplc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gahgnvqmi.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gvqxezxjj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdzcjymyd.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gnejcuexm.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gbphmfqzf.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gsbgdxmfi.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gdzdddauk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/ggfjnpkcy.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfglywsfi.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/glryrdgkz.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gzvghnbcf.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gdafydwqy.sHtML


<!-- 参考信息 -->