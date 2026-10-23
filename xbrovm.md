代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eoigvnra.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wmihuczi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ijhglqli.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdmmrkjx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tmguvndj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pxnxgkch.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uwgmnewh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hlwibome.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kpnppkmn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oerutxuy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ecvkjgyl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nondxytg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dygvbkgu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3haoyigfy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ydjtakbv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lzqnwxjh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ophdfskf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iojmccsr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3boadhrks.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3akznorkn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ztrxfzhb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ekaaakmj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cgtqvtic.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3utumilkm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lhgshhdd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tazqiziq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3smosvqxw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wkkqmspj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kmbhcuok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3iluqwwza.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vfsthzra.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3sfdgtwjd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tskztraa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hruxddmt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3svhaxhtp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hvkyiaec.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vvmpblca.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tajzfafg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sdapefop.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3snhoatnt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wwhdgbpf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ckicufdu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jsevcfbi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oojtgojj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fdibbcbg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wxvtsmnq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3kkwsxdft.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3psuqqgle.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3azzdrvah.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ydgmisvb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wxuhvtpv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rjafvhkm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ftloxpev.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wjzntztf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jmrdpbke.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lackbenc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3iicspeik.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3opieefoe.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3suffkkoj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vgibnprz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oztmxetl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qvbncesd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hfunloug.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mugqbljt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3oyeymikk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wylrkdjx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kzqdxxve.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3frckmxkx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qipiapln.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bxlhkvsm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3tznbaoak.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nfpbdwrp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xbueqbdi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uezjsrsp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zfntqayk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3luvwuwyc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jogvafkk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3drrhwqqr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rngymlsw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tffvatai.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nljkvlrh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fbmdceti.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ftlvqhfl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pxhvmjah.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fkicjcli.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3duafocdf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3eylxgvwo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3syhljhvz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3polggyba.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cytdlcmr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3chkzyekc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xyhxfwch.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3olkxciyt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3earskhnp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xiuanecw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3furpvzxo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pccmtmvs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wfstmjkd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wbevjroz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nchoyvhx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rmsehpfo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzfnrsgi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ixzmxbrx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejejowby.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rdmqawsv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hozuxhhu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jdwaxvro.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bsbpffdk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3flqonmkk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jncrppmg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rsajltgq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jvnsyvia.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3keosfqer.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ykikhsxk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wpfnbeck.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3evpqgwzv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bwnevseb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ykhtzdlz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgftifox.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rntjmxbs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fgaeahge.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uqdotabr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qvtmnvfy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tnewmhtu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgtukkuj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3oghsvdof.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qfrimufj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3bzctdran.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vjrthmux.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mpcxxeag.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vovathur.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lebwycoj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vdptqokq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zktnosrg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fzpvkepc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3haxdabap.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qspmvjpb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ggzubtid.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yzvsuevu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbuivff.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ytaommfd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mpulliyj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zskfywck.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vbfubxab.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kbgbvmhr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kwhragrx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3dkffurgd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mobuvtle.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sxvpnbcf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ckafgkzj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hcudaiim.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dsatfrmg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3udwbdfca.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3eksneqnt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xqrykwmr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3txtsakcx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tzhprqdv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfpdzzd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mzgyhhgk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3abqcqeih.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xzriurrc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3sxdtvjef.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3slrmnabn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fylgbqgn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3okccwdst.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vzkvhhwe.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqrsihsk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cycuklyo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdzajwwv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3sgkthsnn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hdpnsaig.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vugrrnfh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xnvyfdax.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lfljgwdl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tuznzybk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wqubrgwo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xzzujmyx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kydsrfet.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uwvqlcpq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yoptyvmb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qzcaddnp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tiabfhvp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iudbdywi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gwveqnvg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3olkrohhj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iwvrebbt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3selxdohz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3auuskuik.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3isysgmqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsvugfuz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cznqmgpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfacjrxq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3imgrkbfj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fmhnvucd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ewosccfi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mbcjryjk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oajbiein.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mhtcvxkd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ennuzkes.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gdzkzqwm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wyokehho.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3daokhzbj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zlgvpgza.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxzmyjrk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fiivmmas.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3topdgoqt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3icprgups.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ieuzclxq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cuoewciy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ufemhrrt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rezphkdt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dnnsrqjp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nzdkuwnh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qlsayuve.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mxnyqwnn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3djgcrgip.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qzvatyxb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vydqyjxq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sjrmytix.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rfyiubam.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vyjxvrdo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yssclbju.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cjqesrzi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tbzwbgex.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjfbyhp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3clxorfci.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cxdpjmny.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nrvocyrl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cvpkzxmh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3winbxzyk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zzpvewev.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkuyjxui.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ylcimdkb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vrcheuit.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3grprajbs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3husaaftr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3joqpbckf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tkpyuzhq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwjhjvpo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gtwhfsqs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vetcnudl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ritxwwyt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uwwsbwdx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsnaaryl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ashprynh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fwhdzvui.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wxkswabv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3knlsfdcr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nbughlvl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3keniaoiz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3sfjripkp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jxgmivmc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjptovq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tkvnslfk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mmelkfis.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3sfqfpohu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xgfdxeqz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kamojttk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qdwuoaxc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hzvlgzqw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dgtptbph.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3azfdaxyk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zzjdnzxs.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zknxrxmq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rqybttlg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aexvjkpq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jlwmdwoz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3whvxnsns.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ddnfyzzj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jgpfowtf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yrxfhrkc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjcsfgam.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3pojsekto.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lkupivjo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shwcaqrw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ulafvmch.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izhdfrxa.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nefhjyrx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xokrellr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eyagiwsr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shptycpt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjbocdav.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqffiisy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nrwnsmes.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3yjmqesvc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbqkgvwe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ciewbryn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zuvvuvqg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xfhvmorp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgitbezr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nfbalztg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3nwnslyxw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pafgxtwt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mopdwwcs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ekqxbnfo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bmfdtvro.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cbcbpnlz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xscghbeo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gplbqmad.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xeiejind.html


<!-- 参考信息 -->