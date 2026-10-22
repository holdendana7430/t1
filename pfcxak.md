代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uaulrejt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2avgwnvku.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bxkwmtln.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vdkwqwyc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cmpmblpn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rxrjyaxn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2drbumtxd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dncntmmx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2exfhwsiy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ifziwwnk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zxagjsdt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ddtmoniz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fmsuognx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2anmfwucm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zbubknbg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uggvjphg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tqzltrdn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2eyvfykjo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nzwhcqsq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kbitxipq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2tkplvova.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qkfrqhlp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2elscqdfe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xrslxbis.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2toywsvtb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qhnqunnr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xweunllw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mpeojegk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gifleoxx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zzvbcbuq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2obivczaf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xqhfzxjl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mkyqrlml.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lazkyrfq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2imvjbnbr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eqreeuly.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uonwirpn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kwitdiwu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lejzsjqt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hsqilpzy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bjdnnimz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tbwxuwbu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tcyioxgu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2silnyypn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xcgxusui.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zpvanuep.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tkklvkef.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tcndtuqt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wnootean.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mtwcasad.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2suvfjvrd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ycnjlxvs.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2uibzyazw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gaftensz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nobwmqwe.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jdqzugnq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tjossizd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bijfvwvy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jzjwlcin.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2miqtqfwo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xrqyxrao.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2klaavknx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cjmbrfax.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eilwdedp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wwghpjiz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2cmoyykrr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wcukozdt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yjbxkvkk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hizvjpak.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vjhnmxhq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fggvdbmr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tzdspbze.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eqnpxgcc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nwzrvqbp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dyhkapse.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nhmxtkwm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jyieawga.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ietwleah.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kowzfdby.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xzmwsfdr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mwuxowga.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zsqknpbg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xsplyqmb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kazjmazx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2larfzfxl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uddsjgtj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ofnojrpj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uwidtvwe.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bjwfcvno.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fhbkecxn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eoitymdz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wsomumyp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kjetpycp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eamkylgv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ituzleeh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wjninxkq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hzbevahq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2sdqnaied.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ddhbrthf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2putezozb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhytixut.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vmbvjoiy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2yodxtspy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xjfqhwxi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2uhbusgnu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2brwnuwrs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2liiygwxv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2llwybjji.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bonahzdw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2phivaulf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fvbrhdcx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fsvytter.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tabdbdxm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bshbdiup.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yaxjowek.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahoqvtgn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzijdgqn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gdmpvwjq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ljaequpj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfldhjf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2johnlsxd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwsubjli.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2olfteimi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iawkaiyv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wmooxonh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2svqnklyb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zsmmgiwz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbgjzct.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2cyzymexj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ljhjfesq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hmuocuyu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wdarvnca.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jrmojlfi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2bjidulff.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2moeurbxh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gabaqajn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jobcbkrj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kyvoywgc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jtjbblak.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2muliiaou.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2frirsnoz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bhtxyven.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fhdmeucl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vfpataxa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jniznhar.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sxdtctxq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cokialyy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qqufxqki.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2upkpidhe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jxrcxgfh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lhpwtwsp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tnsjusnt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uqsowufj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dsdluqdu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jcyzdqlf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ggnbelgp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ztwcvdgq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kszqeoki.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ciklzwhq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ixuwgowh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nrwhjcii.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zafnrkxh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wjbcorlj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ceunbmgh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2olhzvbvd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wqkuutly.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axtajcmh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2skhennxh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2urmmhuvt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rufitckg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tivqydsm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xbjkxjun.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ixnbnfwk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2giciakvw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2edjnsetk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tfnhlxll.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ztkhkqik.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gyaxzqzh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jbaydkot.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rgsczcej.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tqayseox.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dxsvhecc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ttnmsmxz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jfkqxyql.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pjdcbxgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcitrgig.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2gdefsnxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpzgzctw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymooqguq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2mcvvkksd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ddmfdmmo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2zjxyjjhs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ftboupij.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vtmxiybj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cikeqaco.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtosbafi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbmjqfbz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cpxjubft.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2zejajmav.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfdamezs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcremfdg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqtlkwhj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oyowgmxr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mhzfepyl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2oespmmvt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dswxcjrb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gmbrqoqp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qnxazgbz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fryafqxl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2frgxpkkv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wzcbdyhb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dfybvrvt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gxuenqis.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ylhtftyk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pdszswmj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2crzqsxdw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zmtabbpm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2uxpiveok.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uywbjosk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wzrghrty.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cryclifq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jpkqwdxl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ezrftawx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jpoduqqv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fgjeqksg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hihspolt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wnpdgmli.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khdthyfk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btwcthzr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2loesanty.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fbfdlpxw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejanwaqq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjqnbquj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbktvros.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdcdmsnv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tajznoqb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqcywumn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eoymnfhq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwejgryf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wsqylyxt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlogwefv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dlxxlznt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xxhhjyne.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2onzyuafk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2epktlume.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2voyrhmqt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ryscwkok.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ednbpxeq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ovcgozjv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lkmyinwp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wsjgpmok.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2poomzwlv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qbbiiths.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2szhpakzv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2doccgxtz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cyqyjgwn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ayqcjvsx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2czoxsfos.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iyppwpms.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2yhnvlgrk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jvgjdgxl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xiuycayt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vjjbiyqn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xbgqakyu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bqnassam.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vapjtbbc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qpgrbvhv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebmuhkwj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lwhwybgq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gwvamgnp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjlutwxz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hurkuhck.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2juwetlyl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mifjjkdw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mxxgqtlh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euaswcce.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2amyiqcmo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqmjboqz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gakqgqrd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwggbekk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nsbiteqx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtzkxbju.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lyfjscne.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aoiaiehg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dqtnscdf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iuzuwpxv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hpleerne.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pzxqrwut.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zfxztwtq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qljgbyau.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vqnhooau.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2flusgmak.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2lalrfiaw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zwjepzaq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2euvvbean.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vebzdkui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lymkfque.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pwxijdpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cofershv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qrxxgwyg.html


<!-- 参考信息 -->