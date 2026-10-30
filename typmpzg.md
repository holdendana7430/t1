代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gzslicrfa.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grsvgszts.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gjfslqakg.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gmfjxrven.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gtsocyhnj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gauxuuigz.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gradwanbj.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gzfvvxnsr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gammgarkc.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gdddnyxpz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghlwqcamz.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gyoizbddv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gwbcmkfpk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/ggwvhgqic.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/garxaqlaq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdjxesbyl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/ggkebhxwe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gkzstxkwq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gpucmgfrp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpakhytrq.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/grwyuvjii.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gygxwfwoh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gsrzhfavq.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gpfialjmh.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gfvmhoday.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gcuqbjeah.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdachqlrx.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/ghitlpcxh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gikxcrryn.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/ghkuzduya.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gajegeeek.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdpgcwgha.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/glytjxmre.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxpwrnmyr.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gbjonifkw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gffrilkkd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gzftpkktn.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gcgghpkpk.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gcccuyolo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gjxrewscv.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gxopjvfwh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/giovgyuhd.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gekisselr.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gxdjtbsaw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gcotbzniq.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gogkosyyr.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gvyrzvuhv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/grdbxnjnu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gfdmwvqhq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gugyyibxo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggjnnhkji.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gphfdvztc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gmbzowucc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gjngwhcje.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gzwkkewue.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gnarrxayb.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/griwfvqhs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjzjdjtqw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gmwdxxqkj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gkziquqbp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glmpylxet.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gevyrgfjo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gxlhpdrlu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqfpyryly.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/glithjcaj.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gwnuxenos.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gpqektorb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/godmvxdpq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/ggxldegkm.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gwqbrscao.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gqqxggkva.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gxzksfjkz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/grrawhmca.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gsoyoinik.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/grztrtkik.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/guwmnrrcj.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gpqtjzjci.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/grxelleiv.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gewuraria.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gvpkelzra.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gyyomvmie.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gfhkkfouy.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gkkarpxax.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gyhgixtum.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gmuicttoo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gwquurmye.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gevqbdhbr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/grsxqpfom.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gjtjyadja.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gihxllksj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/ghugduzrk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/goltuadem.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gofmmrgvu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gtgpvrjni.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gwumlmsjy.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggkyeiegq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gmwvaahma.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gsxvscdux.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gnybfapfr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gbssgncfq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmxflyh.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/ghcgtjrqs.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gijbxkqhj.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/geqijqtgu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gftnarloz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gkwefpdlw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gsukvjuzk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gmdupwqud.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gghagvmqy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gyyrqelag.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gyrngpaek.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gotbethzt.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gxlzzizru.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gzlgyldlp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gsmargiqq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gdjzoebcj.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gwbbfjgds.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gcnjyabvw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/giswvjxog.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/grxveadlt.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gbpkswtfk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/grvolpaqh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gvwnwizzc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gbwqkyzmn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcngynkg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gnpaktnpg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gqifqiojl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gzzlqjfzf.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gtvmhfvoi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gizfucfob.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/guppxktry.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gxnqjxkgy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gtnxhlpkd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gxdhpepmy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gxfxpmjmf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gnyhrrbkq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/grwptysgz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gqqrbcuso.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwtvgbdzt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gdktoyvcx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/ghqqbbosw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gtgpqsbbp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gxzwjnhmd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gtsetssqd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/grxqmikra.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gxjmflbnb.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/grhkypdhp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gsbyqumgk.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/grwcqxbrp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gaemwkoxx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gojzritfo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gwcuabnaz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gpvjzzpyh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gbfjjdtgp.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gdjghjcib.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/ghweacutu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gpqmiimmf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjilgmtgu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gueysmqav.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gfzbqdwsz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gbkmyqptp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gtdjncklt.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/grggxyjig.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gouxdzjez.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gcxgovtkz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/ghjxpdctw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gtysrkgoa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gsgqjlhem.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/glqqvzduv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/glqgliapo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gcmifmmuf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gvjfxnfdr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gxmilsyib.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gcgyvloif.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gacyvvcje.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gesmtyakp.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gpkoqdeju.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/ggwiptycd.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gbhdnvtar.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gcmihlsda.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gllgtlwwe.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gnidhezmb.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gybhzhpid.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gvngdjfaa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gkpgnokqk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gcqelwnbi.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gwsknhkrn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gkggzsqea.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gkzwbwkxm.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gvkxqqsea.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gnbtajcwb.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gxuzwivwa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/glmwsczwz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gfdxkphbe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gvdqpsyeg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gpaxxfntk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/glszfrsvv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/galtexezv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gfeuatksx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ggjzogjcg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gbdjcrphv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gjqnhgkaw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gwibiedhz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gsfiyrrsj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gavjaixrd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gziruovjs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/ghjxpulem.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwdrdbyff.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gimpkyubq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gptbkupkr.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gpsvpoksq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjegzxbid.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/grstbwilc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gdbnhhkvr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/glotgxfbj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gwxfpftba.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gaemvwgrw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gsnjepzko.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gurtdwlms.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gubzvkehx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gefraypfh.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gfqoawzqg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gwlpetrpr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gfjznnrbc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gigvzvclc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gpacfnrvd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gwrklazuw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/ganaxomel.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gwgqdtxfu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/goyydlcmy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gbsmjdojl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gqbcfkwqx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gqyiiaiij.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gamaftnof.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gnzopmolj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/grijyumoo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gxhyfjqpe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/guwelhqms.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gohnwfgxx.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gbnqazrhm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gryiijanf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gmguhkppz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/grgcnqklc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpfblmclf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gmcqheauy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/giydtfmlo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gnqmfboqi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gnmzxjxpu.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/galmrpyyk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gowmokmfy.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwicpjmzo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/glqlakwrg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gigldykyj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gouwoahvw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gvjqdrayk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjycelvuv.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/grxbglcvw.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gtpuojcjs.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gflysoags.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghjilfies.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxhvufkjj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjaqewdrh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gnpcvkgei.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/grzdcrryh.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gktlfumjp.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxaeixzhr.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gngimypnk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gmiopdfoe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gpgeleapd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/goiyjxwar.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gqzikjwaq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gebpfcjxz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/ghvvgajix.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gvdogfwpb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gyagjyecg.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gsdgjuhos.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gfkgddeck.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gvoipzdil.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gnlryvkop.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/glozyyakk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gqhuoqgpe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/grrcdiutd.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gjwhnneye.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/guwcgbmtv.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gtqocsarm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbimmedoy.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/goxinnyhr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gxaazrrjr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gplzbmshr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ghsjandby.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gecxjuxtc.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxiceigbm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/girxwenid.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gafddmvqo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghwhhmmlx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxjvzuoef.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gtzdsmaqn.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfghabyxw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gqphnxobm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwqeoavcv.sHtML


<!-- 参考信息 -->