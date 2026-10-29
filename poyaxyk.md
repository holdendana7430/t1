代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gfgwnnikm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gztavgebw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gnhfpqonk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gfsfeuuyi.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gghnilavl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/ggagpyivr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gnalkisve.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzxqgjocv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzlpadaaq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gesazzxay.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmjwsbp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/grkxapqaw.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtjcsruwk.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gpexprmtn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gjluhqoly.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkilijsxd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gpcjfxrev.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/ghmkrppac.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gpsyvlirt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gwpepzhbm.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gageinici.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gzxialqqm.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gzunnpbee.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gbgiczatu.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gkinwqlhm.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gjbvjqlbt.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gnopintjc.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gbpessogq.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gvevwsdey.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gtweywkqd.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gnnttdpoc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gfffucwys.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gwreyzjqb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gsoaxccny.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ggllkhlsh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gkmnvrepn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gsnbpoisw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/goxyhgqxl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gvwlncnbn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/ggzvhvuuq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gjxvnhjdu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/grdkweezh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gdjvdwvbp.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gyyeoqrmg.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gqecfuovf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gizcutosy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/grkhkazhq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gjgwmccdv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/glnqwnrvg.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/goufhszlz.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/ghrsfwtsm.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gegxzjleu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gvkbhqfut.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gqnmvbaiw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/genwyoaqt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gfmtmcnoe.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gktieozrp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gxbqmhtjg.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/geznzqfie.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gfgwsswop.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gjrqjdjcp.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gxrpdynde.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gecwqamis.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gzuvfnkph.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/ghjssqwfh.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ghbakieum.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gkmkflmdi.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/glhrwqndx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/ghrixgywd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gjnguqrgl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gxtuyjasv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqyhgugdj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gvrpljseo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gxdpjiuqp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gkoamsabj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gwumtivfq.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gfgzjqdsu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gefqevfns.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gxhxjaeex.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gykvbwonj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gujqezkdv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/ghasnnrxi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gvkgqvbcg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gkhfbvfkp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gpxmpvjpg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gfppzugmz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gyfypysxa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gqyflwyfw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gjrwaznvr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gemtzkubu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gohzjtfph.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/ggnfwwlqh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gkzwdchwr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gdubeentc.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gjlrxqunb.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gkizgddiw.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/ggiboheyo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gshukluwz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gtsxvlepo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gghigsosp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/girifvesf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/girxjyran.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gealgyacz.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gcynamzuc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gbyrwwaxs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/glmzjxmds.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gxkkjoybf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gnahktzxq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gcpleequl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gocjtemqz.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gdsasezbb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gufwyrikw.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gbrechfum.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/giuxrkdur.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gptccxpef.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gmameqxnr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gsniumxrf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwokznkmd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gbegznnsn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gzllzebia.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/giftzhcji.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gjegvwqnf.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gqktgmrmt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gobmuawcs.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gfvzvcjkl.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gcidnbmes.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gtuxdxwmb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/guhbnvqxi.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gpuyedvtu.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gavyjofsn.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gxtljnlza.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gyddtlpua.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gwaipfplu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/grdojuwes.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gradthwfk.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gfwdwqkzo.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gliqfckrs.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gnsdpehlr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gwpjzjopp.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gfyipajhb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/grzumsjtl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gvciswibs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grldxxazu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghnzcdwjk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/guvtadije.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gkuhjbvcl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gcrlsxvrf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gbdytgtiq.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gxeuutzcy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gvuxdarbx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gotffhgeo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gvjlnjqfc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gwnhlgbnm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gjdkwcucd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gntvbbphl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/grmmnugki.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gkcskxqic.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqrbnksuh.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gnhiwvzgr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gapebbtsz.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gjupyinfj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gsjlcwbmr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkwjfroty.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gugnlwrby.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/glyukozhi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/guvvkkiwj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gmvgbdafd.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzapqlbmt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxwzcykee.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gfnhkywlg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gsgiksqbw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gekvohgtr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnncsqoxb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gfbrayktx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gccpmpnua.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gmjlvrtzi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gsduiqlot.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gbwihgnih.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gfwjwrmjn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/glkycurtw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gnuhplhse.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gttresyxg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gefagolwu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gtoiilmcu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gkjhhjvmv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gehipmlkz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gbfcgdugm.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gxcrscxsc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfkjqbwgj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gofjpbwfv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gsujwdkwk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gtlvavgjn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gfhnkgiok.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gwuztkmcq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gmxkqvodh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/glmyuivvd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gutkyouqs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gizvqxoub.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqplfqcrr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzzggzjpc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghcmlngmk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gmzynkwui.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gbfbliaan.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzgsndkhj.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkktggnht.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gimamlqhm.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gepflvhuw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glzvriazf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grgtrjsjk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gufmpznip.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gpmntbgpa.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwigcumci.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/glxqeupnm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnyntpqyn.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gqgcrktzb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gfcqoctar.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkjxmloig.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gjwktiuiq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gtmtticvs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/ggvuwtjdp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/geacdamoz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gpmqceyvg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gcthkzzbm.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gkfyfmvcv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gqluycstc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gbhyxbcvd.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gitlbgqlq.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/ghhzfvzyt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/glmxaomsm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbfqgctt.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gydvioueg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gdjpddsgm.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/glylwiwek.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gslynqzmm.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghfwnrwxg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gnjmhqzeb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gvmkufddu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gyjraxsrr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gmsgqyhmg.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqfuepdax.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gonmokbtg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gnajptvgu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvviizneq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdyudkfgu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gjitdatxy.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/giueugoij.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gtuprrdcn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guwyzlnjb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggdbftrdp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsgcyghgx.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gccgbaamo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ggnddqyxw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gweojrpse.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ghckmcduj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbqseixam.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/guofotbtu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gwbsvsaou.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqytmttrt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gsmyhmooh.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/glsraqltx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gkibgcqtx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gjfkwyoeg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/glglzlrvm.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/grcfasqni.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gdxxbvsnh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gpqlurajw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gigkeshnj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gqchjdvfw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmdszzrbu.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gapxifrvn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggaykdsoe.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gnzvmuowm.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gmvyxgmek.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gimcmqqak.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gyfynxbkn.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gimmftcei.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/ghgkpgwlf.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gsgdboiki.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gxhqpvqwd.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gsjuiibwm.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gmtpbrcxa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/giijbjtwa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gkcdbnuod.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gsrgowkug.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/giavvclpa.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gjnsbgzzk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gkhonhiko.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gijkfwrqp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggqhfpzgw.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gurimiebv.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gvwkovfke.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gnsuglmwt.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gyhjuyjzk.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gpzloaaqf.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gpjuxigmm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/ghchvmjfx.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gdxxaamhi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/glsgovjyh.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gfgydguex.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gooxlvyes.sHtML


<!-- 参考信息 -->