代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3murxarpj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lkhihxie.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bohzpwso.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yjcaxube.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pvwoqxzd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ssrufeda.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rysyzqtw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3flwkmkks.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3syvxbdrh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wkuudapj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dcsnueuk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rqaofeql.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xwcsblvz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqtxvbxp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ktalkcsm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kjeiqpct.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pwfjmdyb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3maqrtbbu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3brumlsyv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zzjulwqe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wnjgqupi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ycyercom.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nvxzcgjl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ijpxrkrl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lzajitcd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ujxsuiwr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zdppuiqd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3uttwsxba.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3okglygww.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tkcothlt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3uwetyobi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uvjadvzw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3regzftcs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tneyicka.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jyucmhqd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3icizhsdk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3abkznlob.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nlcrhhjl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwhuecwo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lhuehnjz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pwoajgqf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3caztzqyg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3skueljxr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yezgkbkg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eenmpbpi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3igrhyeax.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qbgwniwz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ahsnbvzm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ipiueeml.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3imkwgrvu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cyaocxtq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3glyadntz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ynasboun.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hmlaloox.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bqdfedwd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3imopehsq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vuijpozc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qvxmqpsl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkhbpbr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ttkkjaxc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xeshfyht.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wlrjcqau.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yhqwqxik.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3aozyaojt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3arhemjhj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gtdizmaa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jgfdwiwv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yrsqlvva.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3giokurlp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ilsrrcqr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dkwkernj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gqcaqgij.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hytjsdii.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hhmftfgs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3juyelnoh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ggqvihhk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3cixoqceq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ervojcir.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oyjjolxs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nihydcmj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iykmhlbn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mlbfgwgv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vwhxvarx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3amhtgone.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lakvvcli.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fbwdufld.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ttwoilkc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3axpxtsoo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jjwdbzmu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3idzopqxq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ckrgpfmq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3sftkgbfz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3umdclvvc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bdgqviow.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lzioiaja.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3slnhnzic.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3svieuxrp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdddcglh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iujvgclz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rtzfxguy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3afieqjdx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dxfkzwaa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wcsfhxkf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlnqwqoy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bpbwposj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3aphvhspa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ifraddph.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3epxritcy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3npobvapu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cmbrqiym.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bkzwjlvn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ucdsybyb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xvyuarbt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jmkqrbrx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3keeuagpt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cajymbvz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wxyavfjv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fbrnhhfi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3bdkcwagi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3piamaiyq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xbjmtjkz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rhjfwsvp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3iqwdutrb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ytkvmxpp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3iufblnvg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3spxptgpy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3caxbyihp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3aemzxngi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3agicjprn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wodowigp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fiyucxba.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tjqmwwjt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pumwhbhz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zywmmmqo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3culemwym.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tkwaaaxm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tkpftedh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jbpamdyv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bfincmqq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mtohylcr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pzdvhwdt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3okyfwcmx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3cuioxjyr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxvxhzak.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3movawkpi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rinmtzwl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3imtedcig.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xneiidls.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3frkzojoz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jippqrvs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3dslcmpua.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ukczlcyo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rtgzpdmm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vwejrrdq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3htsddtou.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qvkoiqvc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jauzwyew.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tluueart.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zhrdjfjo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3uqvzdfor.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bpvhwjfo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjansgan.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zakcehdt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jukouxyg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxklrfby.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dihuiixh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwauzxqz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jragxyfz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3oucjvhmc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rtzxlezm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ljviyzes.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3spbkbqxr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mtvuvksg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qwzvscdv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fqdeciku.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3euinnvcl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfenymlv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dhedpbrb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xlnitztp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mhersqcs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zynzbqne.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cgujjnts.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bvyhoera.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eydxsbof.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vbzmevuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmcmjycr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wnaaucxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3updfyeny.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ynlipycz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lnwygnvg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wobkrixr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wgehtfqg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qebinxlr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mhvdqbed.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kwetcwmc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ultgqkhk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ksutussg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rjnnsddm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xryizarh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ddjcbzyc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abgrrdhm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ycnqamlx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3iqxpkcaf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3evhwsiuc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3uafgcblg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yvgieabb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jewfjwcp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iitpwqap.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3odyjgtvp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wjexeuho.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ovrweeqb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3btgvgque.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fhzjlrig.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bmrpzlfb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xihmvktj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3inilzxnm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jpgkfnne.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ikdtaaqm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3muqienhf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vdttqdvk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ahbctnyf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uofqtvla.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nnflkken.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bqxaeykc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3srtnjmcf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3bmahgioc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ufdqrokd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kuuybqcp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rznlvoln.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bvliixlk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3iskckyyw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wirekwpi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ynutrobt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdhejjdz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcvywurw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yxayxgvi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjfvbdqf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjyexmvw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mfgawfzq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrgferkw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsgmwskf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uspbtemu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vodajwop.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mfclcreg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sbseqixm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lshmufym.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zcgkhknq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vpnxtymy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kzoedluw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3eebxdsuu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pqvppilc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3stvbvxnn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jqidffma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqnxtjwq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3goevowaq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3iwvdtnus.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yqjeesgd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rucydmjx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ssvvhfsp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3radihmqw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mlmexqbm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kytbblig.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dvhsvtqr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kkvkkltk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mfnkibqn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fsmvggei.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dvhwbbdp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahccqkiw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3khiggpcl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ocpgpyyd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcaeijnc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idiggcep.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrjzedqz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ionpycob.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3abdvuiac.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mavmixjn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tmqrerdp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3issazjvx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zsnoausn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wltekwlx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ztyhsysg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scilydry.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oegxgkra.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zxqbpktb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3bkucwsgg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rgbwlcdr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rwzjxtva.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bbbajbtm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lrshqtbt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3beyketxs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wcsotilb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xbltstqh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qpbtcmpz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pylyqxqd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3drondxsh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rnzhnrex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dymmuoam.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pvzrnuyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phiszkwc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jdywnqqm.html


<!-- 参考信息 -->