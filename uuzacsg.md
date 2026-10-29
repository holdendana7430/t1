代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gmnfxdyln.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gmplvoqfi.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gpndzltvv.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gcilorqcq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gawgjoyph.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gcmzdoipp.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gpzjcstfp.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/ghtfvuzwe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcyfjshka.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gwsanybds.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glprrqavr.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gjounywkx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gkacruzrm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gszbjrulx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/grehmptzh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ghgemgeor.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/ggaplenma.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/glykmanry.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gcljgqtne.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtfzyrsk.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gbxtruzhq.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gqlqmhvek.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/ghlnsvfdz.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gaxerjpfi.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gatmtmqtm.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gobisrywo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gbgginwpg.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gbevfdjcf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gafeplslx.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gbcpntbkp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gwtikcuwd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ghylacccm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqifbbze.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/glbyvbglv.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/goskjquow.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gjufnnmss.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gjhcenlwe.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gfrzrtwpt.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gphixjjaj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvunlrarz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gpavzmugb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/ghniebjdz.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gozujlqls.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gphsnzxvq.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/ggxltdvzb.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gkljrobwd.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/ghfrbujjh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gxkrjbvpb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gsogbsmcc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gncmwktgq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/glgbqbpgd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/glwldgvho.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/guhsxwbji.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gorpqrgyg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/grkkjaslm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gijcwopze.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/grxnjgvgq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdybashz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gjotosnlk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvuyygtrq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnqdlarfb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqbxhrqlf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gbuqmaobi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gvayiskfi.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gtchbytjf.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gfnxjqcwz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/ggmaiacwx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gkvodqzlj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gyxcznzkq.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/ggmpjjanb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gilsiyual.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gblqitycg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gzgvybhsm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gquskuize.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gtzcdklxw.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gkydxauih.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/grntdlhvn.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/galoeokdr.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gxwpfndcc.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gkhpulind.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gabrhhddm.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/glcrdxbqj.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gacadpanj.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gsqtsbjij.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gqobkgzaq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glwlzivzo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gietsedhc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gfkjdpkjb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gfivkgauw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gnstvlaor.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/guqrhzttb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/grxzrrhnn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gkoxfgjoj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gkvfxrzyc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gsvhyoyoq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gtldtlilu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gbmhfkjwl.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/guyhjdnuk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gclgdlrzc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/ghqjdegah.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gadovssxk.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxvdzkwwh.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/grlogehha.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gmhthbesc.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/giswgtyfo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gntwprokq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gwjskeymg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/glanucifa.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/glvzbnrav.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gfxwhmtch.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/grienvgfu.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gpnxckmlj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gcizwopsm.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtqkdimhi.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gjgywsoki.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/grzfelwer.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gjqutxbwi.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gqdtpkpwo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gqiaakdff.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gsiinimcp.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gzfvkefic.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gyxloeohr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/giyhwpvui.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gcmzqwddh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gjifthytg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/grhakoaaa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gmikktbum.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gckidlixu.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gpjiutwgh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gsaymdurs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnscbnxvd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gyifvsuho.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gepixlkbq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gcagzjomh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrefxzk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gnsfobptw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gieawepku.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gmzkxtmpi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gpieoximm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gppaizohz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gpadqrcua.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gglumouhr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gtgequgdu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gkmsuilgo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gcyxqjppn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gsoptjpvm.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gphggmipg.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gjffvynvp.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gdmxkxvgk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gkmmbryjj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/geomjvmsh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gxomftmjb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/ggbcakytb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gmlsmmird.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/ggoibdcds.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/glrqszuog.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gxhmlccxt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/guogrykxv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ggpwojlgk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/grseszoto.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/glrixvzkg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gwaoajmrt.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/ghlqnqaoc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gvhgtxppc.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gpcbwgjzs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gmyrjqfzb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gaeleqqpo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ggmitbphk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gujhnrzqi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gbfmgsbad.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gfmpdjfzs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/ghkgijshj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gostnierm.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gupokxywt.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/glzuwgjlw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gsjkxyvyz.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gzfgmetas.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/guojznapj.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gnzrifjpr.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gnpyfbbnn.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gwvjatzwa.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gbffejoaz.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gfronbapg.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gtogzrtxp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gdlzxxxob.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gsdeqrmwf.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gbqammwqw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gogyaivqu.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/ghnjpudlb.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/grlmrsfqv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gihppshik.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/grjetlnom.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gvuyyuhst.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/geepenmdn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gudookfto.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggspburaj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gwvdzpekg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/ggcvjmhvm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gypizeiel.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gwwckqbvt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gbfoizfhi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gwjdaikke.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gbwdehvvi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/grbbeoqgb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gqjdaecat.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gadwxaxad.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gysyvutqe.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/glgkmyazj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gaacbzhtx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsfijrkyy.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gmciclfbv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhwejhs.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gpbdcyjxv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gmnefsjuc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghcwijxve.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gelfvnobh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/ggmhuleze.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gstglfsjj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gqjdzyndm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grxwnjgxw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gusymrrwl.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gvotqhqac.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/ggjludnyt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gmkzfrpoh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gqwtijzjc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfbjefesc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/guulkxhne.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gfkmnsqgk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/giknoarpm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gqtohechx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/ghnayvpav.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gqzonnkxf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gbvszfehr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gvbohejch.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ghzmzvyft.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gqorcwico.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gjkvfanft.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gepczwtyq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gbkmjosgn.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gymwhfoim.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gxifzovfu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gwkgpzbrh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gnbdylhsq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gfxtseotq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gurxwnmqn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gkjmswfwm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/ghuseixqk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gpcdmjsfn.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gvlfpzqff.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gykrqyzlk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gaasxguuq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gljkuedpv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfxzotzru.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gccfxerpp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gbicmpcuj.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfxmibrwb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/goviggqfn.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/ghxglbobh.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/grjshywfs.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gckayvmmc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqdvzgxdk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/geodwzidc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/giinreldh.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxeybawps.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsxaylezc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzlatltlb.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgixoou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gzovtwfml.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gililoaqg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/glmnncuoq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ghofoxtlu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/ggusvrffq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gvtnmqoya.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gdomqtbhq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gbnfkmmex.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gxkkghdue.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gduajqgzl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gynqzxuya.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gvbkgvzvg.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gtdpwtevu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gczstiopb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gxyeicixc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gtbtjqspz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gebfajiuk.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gjhuyyzcs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfbdzrqnu.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjwyqitbi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gzbwjkazg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gmeizdgrs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gkwrmwzvu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gvrohvzmz.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gauxckoyt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gbvlvgknh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gcrcxnqyh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtywzvket.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/glvrtauyg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gudpuwkqi.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gidwmtumc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gmjvcjpoh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwkyxapcv.sHtML


<!-- 参考信息 -->