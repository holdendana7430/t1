代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gugpklatk.sHtML

[E03] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gjtjfenrk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvkmdnxj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/ggddumbph.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiepjonw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gnzkwljjp.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gucwhqhxi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fanxiaobao.xyz/Article/details/gnfuzrnnc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaohtyuc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gajuslntq.sHtML

[E04] 查找子串位置
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxapzuge.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fanxiaobao.xyz/Article/details/ggpuvqycc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwhsklzi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grokaunas.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkrenxas.sHtML

Java: s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtmunceh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbggunsdp.sHtML

Ruby: s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoefpvou.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjwfkrvo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmykknoq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggntbtrte.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlvabspf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gojzcfmrk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdkirktr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gotbmobfq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fanxiaobao.xyz/Article/details/gkynjccuc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/guaymaelt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseuttkeq.sHtML

[E06] 替换子串
来源：http://baike.fanxiaobao.xyz/Article/details/gepljregc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/grgxfdmta.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gwjczrlpo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/girwwvhui.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/ghgvmffip.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjvjstyp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gomwgwdvr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkafbilun.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gucpdgrhy.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gevzasbxq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fanxiaobao.xyz/Article/details/gkihcngef.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbvpujsi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gcsuikxeh.sHtML

TS:   s.split(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gktqvlgic.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fanxiaobao.xyz/Article/details/gpylawwqj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gizzxrshw.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fanxiaobao.xyz/Article/details/gxskcrkll.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggndgxjyc.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyssowcqf.sHtML

Py:   ",".join(items)
来源：http://read.share.fanxiaobao.xyz/Article/details/grtzgmosg.sHtML

PHP:  implode(",", $items);
来源：http://wap.fanxiaobao.xyz/Article/details/gfkjuudft.sHtML

JS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/ghqskxidb.sHtML

TS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfwpegin.sHtML

Java: String.join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gybdydval.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkdjybii.sHtML

Ruby: items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/grfxwkuez.sHtML

C#:   string.Join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gouebmkqv.sHtML

[E09] 去除所有空白字符
来源：http://3g.fanxiaobao.xyz/Article/details/ggqslzorj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gctuhafxn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbzggjso.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/geplgjzma.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gtzfeytlq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmznzywmp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fanxiaobao.xyz/Article/details/gywlbbewt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyxzezgz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjxwhzdn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fanxiaobao.xyz/Article/details/glgbdjluk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhmdzwsq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fanxiaobao.xyz/Article/details/ganijarmp.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbtduqhf.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gjfiyzzkw.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gktgfaqgg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubjlpmvz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsspzmqxk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzepvzga.sHtML

[E11] 反转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ggkiirdlv.sHtML

Py:   s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfgpfeow.sHtML

PHP:  strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/garbngiqh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfwrwoiw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlggdudl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/giotfamlh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbmrxqbs.sHtML

Ruby: s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboxppgzl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbhqrgpr.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gvcceymul.sHtML

Py:   s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gyyuymejg.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fanxiaobao.xyz/Article/details/gmfsmlqjp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfztyifnm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gmothyrop.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/gbjqxqtvp.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fanxiaobao.xyz/Article/details/gcypwjuuc.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsdemgti.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fanxiaobao.xyz/Article/details/glcornyzl.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqaeedfu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsyxkngk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fanxiaobao.xyz/Article/details/gggfekhhq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdiqjfesk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gposnmpgw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmptgcjuk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrxmzbdk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fanxiaobao.xyz/Article/details/gqcvrqewa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnogbves.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkcokvyd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgueidkw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjszbcfbm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fanxiaobao.xyz/Article/details/gqgwsukxk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzuzfaiom.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsocobcwd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fanxiaobao.xyz/Article/details/gvzrgkwaf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgafqsoz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/guiebwuwn.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fanxiaobao.xyz/Article/details/glaytdpgh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gsdorfcut.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhajwobg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkugfxphl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gnaedatfc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fanxiaobao.xyz/Article/details/gdtfzltdf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsaqbhly.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxdqkyqh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvltmpllc.sHtML

[E16] 数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/guygtdjof.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gftcdtibt.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhjiqxkp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasrofhcz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gjkkdyfth.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/guhjievxx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fanxiaobao.xyz/Article/details/glhdbkolf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfvwttzn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwqgtnse.sHtML

[E17] 首字母大写
来源：http://baike.fanxiaobao.xyz/Article/details/gwxichpih.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkthjamfa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gupvslmjt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhyrqomc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtofuntan.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gavzxvblx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvorbrky.sHtML

Ruby: s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/gugqazcsr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfnckvee.sHtML

[E18] 模板占位符替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gppfcmyhr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fanxiaobao.xyz/Article/details/gnyjqarfm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/gnhzhiwnu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkdqqblj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjinyhfa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyhidcij.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/garbiwpyq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoofyrjp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvggncckc.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gqcntkbmy.sHtML

Py:   s.splitlines()
来源：http://3g.fanxiaobao.xyz/Article/details/guaavpjjn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhwdmbhv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/glwyihumh.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxwugvwe.sHtML

Java: s.lines().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gklchpfyi.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjbibnhg.sHtML

Ruby: s.lines
来源：http://baike.fanxiaobao.xyz/Article/details/gxffdbztn.sHtML

C#:   s.Split('\n')
来源：http://baike.fanxiaobao.xyz/Article/details/ggtmqerev.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/grprxrfbd.sHtML

Py:   if not s:
来源：http://mobile.fanxiaobao.xyz/Article/details/gtavwsemw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fanxiaobao.xyz/Article/details/gpllpinws.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gteucaqch.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gavrlwaqh.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxivrkcek.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaxfjrep.sHtML

Ruby: if s.empty?
来源：http://read.share.fanxiaobao.xyz/Article/details/gmswtyovx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/glojclhym.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyofsgijk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fanxiaobao.xyz/Article/details/gqombrjhi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gzwxmroid.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatvocgan.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gaqwszzgk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gmqxlatqf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvozubhs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gmplgwpjs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gmzchzzmj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gidwiqrrr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gudynjnvo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxybgmlnf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwolbcbn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdvamfsr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gjkiljlyh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcutfbfyr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvihludl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gwfxsophu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gihdxvgmj.sHtML

F. 文件与目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcruosvb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdhrbzvt.sHtML

[F01] 读取整个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaaahods.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fanxiaobao.xyz/Article/details/ghwhpnnaf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnsopuid.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzwuwgaw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gnpnweivz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdwowrnd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjgzarki.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhqzvibb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gtbqmkayf.sHtML

[F02] 逐行读取文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxefrfdt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fanxiaobao.xyz/Article/details/gvonbhtxp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvukxsmi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjdgqefq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gloqmejyg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfbyzkpe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujczxntc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fanxiaobao.xyz/Article/details/gmvtobwpr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzhbfofn.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhmbngzn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlkbedyi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwtnddzt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjsvwham.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gptxtkzct.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkzaqixl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fanxiaobao.xyz/Article/details/gxllgvixe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/glzpvvvut.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhcjwcda.sHtML

[F04] 追加写入文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizlephyc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goebsiser.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fanxiaobao.xyz/Article/details/grpeilnep.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcsrhdls.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrgieolj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fanxiaobao.xyz/Article/details/glzjkeick.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpukhumx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fanxiaobao.xyz/Article/details/gnmeorjan.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseysrfos.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/ggglpkjas.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljhbmpcs.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gvirrqplr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdhhopev.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gfihiugcs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gawclbfxr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fanxiaobao.xyz/Article/details/gavvokbie.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gxlcqscmy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaatwmshp.sHtML

[F06] 删除文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwcffgaex.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gdzpdhuoz.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gfhjvmtoh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzooqdjcc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkufwmyow.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gximzkqvx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gorlewlzl.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnehsaegn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcapghaxx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fanxiaobao.xyz/Article/details/gspvsnmaa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gucungncy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrtrdjmr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gnyoxrsxt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfeinnfr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlgzktpm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdapktnrw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjspssfjh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuuomlel.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/geigsaoqm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fanxiaobao.xyz/Article/details/gkrjdqget.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdneknkw.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gysntkhiz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpxafwwv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fanxiaobao.xyz/Article/details/gzelvezml.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjralowcz.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwavqjgmj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/ggaazkkky.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauxlzuvf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gmeycoqrr.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbswejgk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/giibasglk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/glvabynre.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghngqzjfv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fanxiaobao.xyz/Article/details/grhqvdpit.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golbwvjtv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfppknvjp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwabmqyh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gocjkjmxu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgrolvxq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ghpfjqcnk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gyvqwnudw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlgnjwlw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtstnhli.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsubjiyyg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyntcjpe.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwwxpass.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvimiyaso.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuefunnh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtcspapf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gjrmfxair.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjnrzsgb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fanxiaobao.xyz/Article/details/gtqciamvu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gdyzfxphz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/glaxglxfp.sHtML

[F12] CSV 读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrqbfqjy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/glltumocm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fanxiaobao.xyz/Article/details/ghleubckm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fanxiaobao.xyz/Article/details/glkalcfmp.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gowulndov.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqhurazb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/gumctloin.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fanxiaobao.xyz/Article/details/guwkvskuq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fanxiaobao.xyz/Article/details/gjeqkqsqx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvojqgstl.sHtML

G. 面向对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxnyisvf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gahdzopoh.sHtML

[G01] 定义类
来源：http://mobile.fanxiaobao.xyz/Article/details/ggywpsqtq.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gecmoqujm.sHtML

PHP:  class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoodkldr.sHtML

JS:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gngotvbld.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkbpgtfky.sHtML


<!-- 参考信息 -->