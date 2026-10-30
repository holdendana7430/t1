代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gnymponqp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gywuotmpw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gfbrrybgd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/giemdjvwh.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gehwnqmmy.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/ggkcdwwig.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/geysjgmmv.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gezwmhzjq.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gozhrghwj.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gufagutyq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/golesouiz.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gauoiyfef.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gbprvuzxw.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/girphutqj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/genfplatk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/guapjbpha.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gqtohypki.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gonmdakkw.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gijuwivns.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/ggcxcxrmn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gkcfuxkck.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gmjrmyivi.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gtmrmirni.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gkfonqjrn.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/ghygvgfbs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/ghbbuwkhu.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gflsbhvsl.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gqigovnxa.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/godannyvg.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gfeqgdopg.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gszoztooj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gxchbhncs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gterwinch.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gsxgdxkbd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/guacgbhez.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gsgmslejr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gmcjyukmg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gtxxsiuyi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/giyzrymzn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gdtlibpap.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gitelvmjw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gadmtmbuo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gryyyflmf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gfwfsuebe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gyvsiprfc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gvawqdxmp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gujeiocmj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gccwrzgyk.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gamjuqrfp.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gjunmbktg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gqspvokbg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/ggdzhqpwm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gszjzfmtx.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/glcyzxlgv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gmnpoijct.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gjlrxxuww.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gigpgywby.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/glibkxdjb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gwheyulti.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gqquypyfk.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gbzvwudas.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gbnokttzm.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gnnenotvc.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gaiijhqco.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxvzxmqzp.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/giqhloiab.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/ggksdexoj.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gjvasygbq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gklgqjfee.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gmximbtbk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gpppfceri.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gtnyzcgpk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/guixfiolu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/grmxwtorh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/grxnktguq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gdylkbawy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gvivfflwv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gtvwhyift.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/glhonbfuh.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gimprwcmb.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gtzwckwgu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gumtesljy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gaisomlxa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gsujkfdhu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gxdludwsj.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/grchbyczy.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gasextiib.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gkgccepgl.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gcqyluxau.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gglechaao.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gxgopyati.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gduikrser.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/guacwexqu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gkwqfgror.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gcumhhqsc.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gqnpvpukn.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gfbhlsufz.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gtnvsuisl.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/grpeeuzsb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gxwqspkey.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gfiwtjhmq.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gjewodzfy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/giijeieut.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdkzsjxet.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/grlxhnrlh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/giropxwgl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gaakmllxg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gzznnnrbp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gtevpdseh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gbsglrkxj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/geyjivkzf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gstpabhjb.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gmwbbpops.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gcayhfobl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gaipfijzp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/ghuboqrkk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gimxjtjmm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/guoqzzkyv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gqyabqnye.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/grcjtudnw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gvepfptrf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gohxumzaz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gasizveaa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gckhxigsu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gjijzlpmh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gfpxbzatl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gyzwgspze.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gretuxmqs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gkxyzkqfg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gcgwxievb.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gfbgoxjbx.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gzyftjtgu.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gkiroytnd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gghyerrbu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gisecxwut.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/ghxgnjwhv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gbtpfhmbh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gzbcwcljw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gblzqedkf.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gtsrdthpk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gxrunmkqm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/glxpbfsbt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gefeoacyq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gyiirghkg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gmokdnktz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ghclxwnqn.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gdhggmdaj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gzwiwbntz.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gavcudhlb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gbfmideqj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gxiaofaev.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gmfaeuhpi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gftnfddwa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gedpsnfxs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gaszjpihv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gpocjgxnp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gmaetcoqh.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gcgpjstkf.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/ggyudnnow.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gotcwellg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gtfwtnxeq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gjxpboqfm.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gorrrdkck.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/ggxmwzvml.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gfgugizch.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gktpcpemm.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gwgxsoxzk.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gxuakydqw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gycrgrtlr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/glkbyiyya.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gxgjidefl.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gmvfsftdm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gcxtwhunf.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gioocarsy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giasnqrnf.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gczrhkxui.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gkittzbzw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gniucfjoe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gpipqqbrd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gzdprpjfk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ginnoqbrx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/glggriery.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gboxatlvc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gxlspwumt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gpmgivyxj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gplnfndeu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gdqevdzeb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gbcdkuwaz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gnzvwohah.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gffbzlyfk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/glxrmudxk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkwrwspzv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gtdlfywog.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpegifvdg.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gqogrnqjj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjkpebmgu.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gmbeseoaz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gprgobmtm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwekkclqx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gfbooxkha.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ggwdvwdxs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ghgepqyvz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gtpxsyqyy.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxgjrjtcu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghptgeypu.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gjyiizggq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gcleibpzn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gjdowxebe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gehshedme.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/ggyowsjxb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gqbgexizg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gulvwxeto.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gorvcscvy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gztpwfdhf.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gcfckckpi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gwkzlykho.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gavqfhlvq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/glrgepley.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gabzizxyj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gpblpxfen.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gtuqcojdm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gsviugisu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/groteuwac.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gmcjhimph.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gxuriaikm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/grkaqrkfa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gqnuyjwlu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gevarcaon.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gaqmbgwhl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/giecucgvm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gbrokulop.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gwnbvlmoq.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gngabgcnk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gbjnntirf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glngmovws.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glwtpvqvc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdmukuugq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/glqcmdnzf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gdszexbpx.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grderhokc.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnclvuuov.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gvwyilfmz.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gymzsbpfz.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcigoxmwt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grnvysspg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gheeezcsd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gzepjjymg.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gubqpnyid.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtexveses.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/giacclevk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gzgvthgli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gytduxnkv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gdfpbpibl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/glhzcirjo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gphpgplrt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/geqlbckuv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsanemjz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gepqpgnuk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gkrvqsrom.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/ghpudjwdj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gsfcuhbeg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gcamylcvz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gcyuostcr.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/goilybxaz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gzlnqavcg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gujppitzs.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/goqhftyev.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gfzqfozsg.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/glshrlbwt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwuilgibf.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvwpqxcsv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/ghufghvst.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gyqculxvs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gjrsgzjjh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gqczrfgnn.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkblmbdzc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gmczcalkg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gdhqugzye.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxosbncwp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gthsmtoyd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbgvjsptb.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghitkpkxz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gajtvzpzn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grugegmwi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqrodhzss.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/grgbzommr.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gqdcojnnl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gxblbhguz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqqrazure.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfcuyittj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glaaahekf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gkmnzodag.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gfqmajnru.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbfdrlcpy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gwipkxiky.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gmxiuktzd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gztrgtwvj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gqpkoviok.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/ggpvgxdmy.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/guljhepce.sHtML


<!-- 参考信息 -->