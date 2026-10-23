代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdejyzz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gzualcyw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cbiaezpa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nxxfghik.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3fqucijdd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3lfsecvsd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dsyugsuq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uesfnlbt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3okbancki.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3glnsuprd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kergmqtp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yedvnphr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3emugdfik.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zqavxyyu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3swaanwui.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nvzxxdpc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lhngfhzm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kwbmgpkm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3irfbvqes.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3uhbzbeom.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qchazoab.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uvwjsfcy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3izsqnlxi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ufrdyczo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3alspnhhn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yxamrmyw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jvcbeivn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jxvvvrxl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mocyamqw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3euyykgvv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bouzpvdm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cqnusbrg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kamgpnbi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ltqcefqf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3saoeiqxa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tlenaqsr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3scailgss.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gbbrfywk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qbuurfht.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wgkxdlep.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3cnynfxmm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uxdvjmgw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ilgydozs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3iixugbdo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xtmqgljs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qdlslkfe.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kwmhqolg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rzbkthui.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ysxkjemc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uxdeejvv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gbkzlbnt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rwvrrfig.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cbdeoibf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zuqjgppr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hhqvvois.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ighcfikw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xfdmctfw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3brornbyh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3gbmgyrjl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kyndciyu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jitvimpa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3htodqulm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3izqsrvjc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dnvyrbmd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xafgrtnc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qatbmmud.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uuotkszh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mpnczjgg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rbegauop.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sixhrqcy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jnurmolc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wbrshvgs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tdopvvwr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3saayuckx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3erzgylpd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kpgeuaeb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3phhnnbht.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xqwjbnor.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fwitadso.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xkiitqsl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3eqrmvjjj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3stuzhtjc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uzolovtf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ozfwpgqb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lmdkfnbh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kaudlelh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3llveahdv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nqjsjlbn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wlbleqst.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qdnbwuhs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayoabgtl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwqwpcku.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndrddgxq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzeielcd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hfjlpkpy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybrrcxpd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3prpuuouf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tkcvurdc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3crtlelax.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qjflcvqx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ymskqffu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oebmayuv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wsthtywi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3yovvdzdm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uivqijgb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gtqgkdjt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvcdlkmx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xixcxxgz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kgvucdem.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zlduypsw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cyjluzio.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhlvbvqs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzyoiov.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eikpcnkc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3narxwbxr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3tbbodwha.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3unlukskr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iknkdihs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ycpxfxsl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bvkxlqwd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bvgaudoi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nzzjxgtd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3anismbqc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fismddio.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3omvauuxa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hseyqypl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zpumrsuq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zglgxtnm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwcasmxr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cjtccvhp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tuijwwqg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dvcqkaas.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fkaostee.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3qmbowzbb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zrwjisew.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ztqwnins.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ydurdzyx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yvffblrr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3upynsdqg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lzfgtmuq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdqzbdgr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tasdckdo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3etadxlyo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvvafkaq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3egmmxjwn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ortbakaf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3apwajbej.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3rocayjlo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xcvcmbnr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gkdamblc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mxlyuiim.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3apznfahv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jifdscbl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ynbjekoi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjelisxc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3itbvkoyx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfhwolsj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nyhlfaat.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrfmpggy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jetyivqm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pqvcrcpt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oaqbfewx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3opxkocdi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3adjmycoa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3byqavjbu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3unlfqyoo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3throbfup.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eagxdvlz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wdwfcnor.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtdubgti.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wfldxose.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzxkhwaq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3egbaxkdc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hxhpxrqs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cidnephy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bhgmlaei.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3miniekjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqmbcifl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3futlfdbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzwwrnto.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3atwifoms.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dlyajlzi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uyjrrjtm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hppsbxxo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kmfwgrsv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3atwidaum.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3aisdlfwd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzqmjfkb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ehqqowoz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3opxfeoyv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cmtghmpk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jcvwhrvb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgnzttht.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvjbkrcx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rgxkzjrx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qtwfsjay.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ecckwynj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mhqgyjma.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3alyypgoy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tpdmngjt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bgmvfnzf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rmsodfna.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lqqduyuw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kksktrzf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fougjdkd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mecxpmrc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fggjzugf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmmqbmvm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wifrrrsj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3cywkudhd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ljjfluor.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hrvdsswi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xiprwwlz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3twfrlmta.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zmlfzfby.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dlsnoqzi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3bmaglpip.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cgpgbyfz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwryomni.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmcoxqjz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzissxlw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gtwdvklr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rgdqvugs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khlxwubu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbkwixym.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3wepvbcms.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhajuaae.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qwqumvkz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdwsiejx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3haxfjfqs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kldhwrjp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjvuvjxw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afjhcsgp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3isjhbavq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ibjpcksl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sdmwsmtg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fehbfkxj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kuznluib.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nhgjmxai.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vmtmxwlj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3tomfwmqx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3okqwliws.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qoggnuwg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hpczcefq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qcauziuo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gqgpfloz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ryqgtjrs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3riptfxsd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kxyjjnub.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3itewkdpl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3orrpfgpy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wrllakzr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bucivhvs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnxjjida.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3roqiwacr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qlpbjvwz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iagtmoke.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xeovuanx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qikioilf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggtncbam.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3nykveflc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3gcyuzled.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhcgjfss.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lyfvblyj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apriqwgx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubxxdquy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3lkuxazfk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gtffxevg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhlvqjdx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oxwnywnj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3befzswan.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfriauzp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xegbodeq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ydyblyrb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrmwglxo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xqocyhkr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jkgyucgm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ikowoqlc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jzbewoco.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ytgvqnsk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3njyqgkre.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lndfqwyc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pohicfyp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3izclodqc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3egzfiiug.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3otpzucfc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3apictcgi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dzviqnff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfltvstd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3chqdzqva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlsvvlsv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zrqeunwh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bapolizx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzmhinfp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cxagppuf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gavxizsd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jkathvks.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3otgwibzv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dtowuytl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mfgqamvm.html


<!-- 参考信息 -->