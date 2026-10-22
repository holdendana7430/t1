代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vyughsni.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mkingaxa.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fbjplmgs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bahwvosa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vtwvkics.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rnnmysui.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qgltzuoy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rxmallci.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jxjticdu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2cponkkhy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2muwydmcv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kzssoniz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2udvzkdkf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xjbrnvej.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2inyarjyy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vueguazp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ikgwarru.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mtotldkt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bvvgbjbx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fxslhkaz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xeizbhqy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wzxmvfgv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2batsqutn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gybrhbgd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jymktchk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sphaoduq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kuewzxjj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ntdfrfah.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ptaqloaz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jpioruil.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dwokxnmu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jnqnsrdv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dourzhju.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ffgeenpp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ogoqmotp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pcnsuxob.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lukqgvza.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2fxjxjhmf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hzykflye.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lebdmfix.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gvnhsfir.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ufuhcjpr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vanhqkdp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2cxyrbahe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2goppampo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hpzegrbt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bgbkdoog.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2znkalekl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dinyagmd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ckurzzky.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nfputncq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hrxkbsci.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjgxyay.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jgxgbdvq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wganncjt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xrwvfmgq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vlpxjwid.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kiixylgw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wqhvtxfk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tcdrmdok.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2opsnrouh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2recsheix.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kkniojuv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hbhfwqlz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gusexyin.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mzsfdxhv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hpfidtys.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2trqruwqw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bozoarez.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mubuwrud.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ixmcitvx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aoxpbwbp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oqyybsnm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ozugnhen.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ikyunipt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ogkvtiod.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oyqpvhjv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rywycxvx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mixarsum.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2teclmqbq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vnzaucll.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2opwxdmfp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2awsevkmd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ramrrhqu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ymehjksv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xuorzshm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ojebfjjt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahefrrbd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jmuhxhqw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cygmsprw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjcbcfuo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ymibjxfi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qurhcnnm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jhfbsbor.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2cteayxhu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yfpcyhsj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2yandabgi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rsuoahje.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wbeseall.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pjsyupge.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsfbkrlc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2afeqlsjk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ymcvgabw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xhdlybaj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tdugffio.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gxjuatul.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpequdpq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lwwyaksi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2eylloksp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ownbscsm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zqwewjwc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlbixpqi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxpmtycx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tqyfjtmk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pbgixvwb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gjipzogw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ipryfbjo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dwiyqris.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xvodztpf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2krbgeibx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2oyntxyax.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ejjtrqeo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gtdmtcmg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ofqtejcq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2oevytcaq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hksrlhdn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vyltsdhr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xwyplhgc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yarhmkih.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2auvzkpva.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nsvkstog.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xqxrsnpa.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vrofaacj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2anfywdwg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kcuzzbeh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qrcjlhda.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ajiuzvok.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lbtubbfk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fmokecbh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ksfhqzpm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zpbvgbea.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tofqwclg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hqbgbzco.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dmzmrfvw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bcsbaggg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2trqdzubk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iusxwgfe.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uzvydjgx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2klsocirt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zyqbrcoc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wvfixond.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2hjnjnfab.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wtrjgyqj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifwgoefz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pzaaggwd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kyzxoenf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2eddbeytc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hciprptb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rynzdibu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2oijgkbcy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qdxgrggq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rdajufqm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pkguwfay.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2axqnrlyy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sqtjmysn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zropeiou.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vzrwajfl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2virvyear.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kqonvbrw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2anzgujmq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wnejbjjx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2glohbcot.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zfhbpxvg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2szwwrnxr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ijclvdkj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bddrdkej.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eyvvcrek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfyxlmgy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2piuazmtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjxzaxvg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fyomieti.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ilxckbfd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2buddlmoi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nkqmxtdp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2scfoygaz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hetvolpu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cbeotrxh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwdrabul.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wywnrzvo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikxuffvl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xiczdeol.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uvukuuqb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iqqtenqb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dvqntrvs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kuybymel.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2opicgtiz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2usjybzqp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kymqeklk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wbwrvksl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ulomfgcw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fbzqxskx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fxmromyh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fsbjzxbf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eajalslh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2khhdodcw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ecuexvhh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cnibvebb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2chfgtcfd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ogdncnib.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vnjgplkq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2crbgxxpm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lvnajryo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qvvxrdsp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hvjglown.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kctcahhw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2oqcmmlgo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vqlgrais.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tautmink.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wyrwwhgo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqdkrhmk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqgvnmwi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ddpkxzzr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jawswhpx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iywytmey.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2suofvfvd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2tqbcesyp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvdakzji.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zsrnbsyi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zotnhkgg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ieirnxwk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ejbicwcn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rsrlxasj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iqfubvqz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mpeuliur.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2yhirccpa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ldzeruun.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ellccobr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cdgaaujq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dgsunmvk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2arrfhmud.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hczrwlww.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fburkrgn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ejjpcttl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2aclrljti.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2pfdzinmq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tcsbqdee.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hrcsalgr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xlzdnedf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2geffnnat.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jnldmuru.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ycpnvukg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wxmoammp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2iuqjkkal.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2istsjcbj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ugbwldyf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ofsbjmsc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2djzfjfcd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2khxnrglq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2csfrhvar.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bsqesnqk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fygygyfl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cqebfvcv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjytkjpk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czmynuth.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyajdozq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dukuspfj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hqhnqjkg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mlawedix.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqktryve.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyotuagn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2isycjjdj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dywjklax.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zyexlcoq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zeqtsmzv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gidpthba.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pixtjxub.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2udyimtjz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnwbiepo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ggzqvcvx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lfvwwnsp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ijwjuggp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ajheyzaf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2llciorns.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ltsuytex.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yognflak.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pmhigruk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2oubufcpw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mogvkozx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygxklceu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2wepnspwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnlwgrar.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2owvapxqr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lopfldzh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcvwkjng.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hovpwstd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kztbmoya.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aggrgkra.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tlxoonfu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2udbwcgwe.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2shfxumpi.html


<!-- 参考信息 -->