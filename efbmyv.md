代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xuyuezio.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qgootfaj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ibcnzlww.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gtzzkzol.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qhnpialh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3oqrpzjcq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qpkzcaal.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3imqytmnv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ljvlfgpp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgetjfg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iqqfqnef.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3avquvwcl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tbbdcjzz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3whvblnro.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zdklpyri.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3feiqlumb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3noeebjsv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3povkmsil.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3snyzxzvq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3rodjzdub.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jbaiurcd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3yzsprrws.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hlckazhs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vqnvllio.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vgucbuxj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jndsdjmw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3snkgdebh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gpzyahrh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lumuhfnt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gjrlgvvo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3deetxkbv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jrroywdj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3klwnsauc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kqrwgidw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ylqcskod.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tnnzsojf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pnksffzv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3otypafzw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lxyliwmm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gkhvamkv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lfgfelco.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zioheyzk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jigngnfj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3tlbhnmtk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3tpmlxulh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3niscjtyf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tqlgrwdz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3diylztvv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vaqiohmz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jrsfxakc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3apakfrhy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3aytdxhjh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkanscko.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zytbtzei.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3expqupwo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mljlmtmb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3imugyale.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wdkkqhug.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3watljzzf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pagxmcbf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zedggseu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3scrardiu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vkvxcfcs.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kwxrvdfy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pfkuaqla.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fjkbwpao.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3muohulvg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pyiatwxr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kusqrppv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jflkfbqv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eohovmvd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mofhppxk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zgkvpzgm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hamatkrd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vcnkuvnl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jfmcuegc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nblortua.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sazhvozz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dwgijnnu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3thlamche.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ynsryolf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kcuktaqx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ehumndyf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ziprawur.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ficllvzi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kznizrgj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ftvxgeey.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3jgixejkw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3lynocwxy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dvdyyaji.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vheafmic.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfztregk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyffpbds.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3eqvnlqyr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dfeuxiwl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3enqbqsns.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fkahoypy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mjlolrvm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3boummtms.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dgqcqqmn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtokcel.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwmrxcq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bapxypdw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mzfrzfft.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lyjwzzfi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hvcogvtz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3piiozpuo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3izsuawlu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fercyhzw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wglikcld.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ymhrbquy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zoewmgjm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3usngqhse.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3iojibnim.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vkvpvqsp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mnnsbthu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kxezfrpr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tvwttooh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3haesndra.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ccfgdcgm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cxjcofsr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3efqnciqn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nyraiupm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mkiuhwvi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zfrukzzb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zybkpdmb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lscdfbaj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tlxvqxex.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xuiegsdt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cdwftxqw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nfsettvl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ipbjocae.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vtfutizv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hsajlwgx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3oahmowpw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ddbqgszo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xesmlzph.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ckziljqw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3osvlorlq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fetdfzjd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qzigvmws.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3junrloht.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3emvnmhhe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tnxynvtn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lojhzizb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vbezqigs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wrzygsed.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ajhzbohd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nbhvxyrg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3irurdhhg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3eqcnarzx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tjbmpvld.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rkyfqtxg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ikatvfpc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntmwogjg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsibssyr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3blkknooj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sytvbxkg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qlmnbbsz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ynntrimy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vsrutnfd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gtquxukb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lzhxofct.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ummkemip.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bgtjvrxn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ykvubsgy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dssxmmsf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fpufwzwi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3noazrffj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3imyctomn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iynkvhqd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lgkfoedt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3whwzmajy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uorsohye.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qgethhxb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yvchiote.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3itmtaccf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfsyfjlr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dssqlzne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqiexhix.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmboebfu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3juwizlfi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qjtshfbj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3efkfzdvw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ympdwfmb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fshzxurp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fkeojpan.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trnsnivj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvbdyolv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dhvfomfi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3plwfizqq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3khdvhrrb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hnktmenh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3csjcbtji.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vctfgmko.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ipvvfxxw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hmnvhbok.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngwdvxsx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3fxwbaptm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xguctrlq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uwtdiofu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rixzfrni.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yqowtgjt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vglcunzr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3pqunysqx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hwgtfppi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3okzosysd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fnbeyuoz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3khiaygdw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zcqlnyla.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wkqapohs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mcxftdrg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3sjftntgd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hthfnprt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jxpdyryv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zsojxpsh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3seycjuwu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jthtomlc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tvmpatfj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtxzcxyg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frlkhdtr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hnsedbat.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3sawxhzai.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irsdjlvk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtzuccrd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dxuibhxb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncixavgm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vbifkihc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kazpxjlc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjlhuolt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qbkheyuo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chmmrpwo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emjzzhnv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bobfuwap.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3pkeikzbm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dvhztprj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gflvzwtf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mptywhpk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xpoetwat.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lbdinbof.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3rajookqd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rmdvqsbo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ngvnxxzi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ofldejvq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dgcvlfnm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiajoeoe.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ijsrnjnq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vexjprbu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cphokaxd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cobugsrz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rqsyfeyx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zkpzkhox.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3iauregys.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3asxhfqvh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hcayqdkm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rvwqeifg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mjavulhv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xzmvkfvr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mzbsvyse.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcimygtc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3echmvdob.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3meertpag.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjlhxzrn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gujofvom.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cizvakuw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3optpudjq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3boseusaj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3etdmvlpk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zuurvxtt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pludlglx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ssysmwxa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfotxsno.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vxihavmy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3swkuyqqf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iruyplzk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mcczrabp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3sstezgsh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytjdhfbg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dcufcsej.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3iraylbww.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wxfwhenw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cnripwzp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mvvkcueh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3izauzjhm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qdsqsfvc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dahnhyjz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3niumfoak.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jimubiyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqedinjx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rcqqwszp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuwoackx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lcnklvkf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tzdtslwx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3flrayckq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qajtwudb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sojwwfcj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sedvqzsm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3urepiskw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qpjkfbmh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3apjvtkxc.html


<!-- 参考信息 -->