代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3murfbmbf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3njducgak.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ceihknoc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sgrptxvi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tspmlsnz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ovyecoay.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3adpbsjoc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3euvssfes.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mofukylb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3fprefamu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pdpconvv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nssctxvi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3iqstkyyl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3znrzlrrc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tgasejxg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zbzufhwy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kuzchynd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3udtwpdpy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3czcupieu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3buouaktg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hjxhlfnk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3trfjdmgo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zwhmduyp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ryhunpts.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qnchrbkh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3angnabeh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kskaguta.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jnsdxaav.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qzkxbysh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3enuwsnav.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oywxidpf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bmeqmmjp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eeqkmatk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vtbevprd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3pxmmahqq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmesugwp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3oyyyhbwv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3csrzwuea.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fbcyigsr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3czwxdksw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3juvrewjz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3iuxyhdwq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3tndohwvq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3bywfcmgi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wagplzzb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yngcuqyh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aciwizqz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vxsqvoum.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xocanhkg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pneugjpk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rfblienk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mpcwsybf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3nrpfibsf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mvnkiwmu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jjvqlvmz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hchiiwmp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rjnqmucm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ioqgfwsa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dgncfsiy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jesgtbor.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jystwken.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ccmtckcc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3baltqaql.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ktydczxm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vhassbdo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mdcpyuzu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ifcqergn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jrukqbdh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xwozzlmc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hqizjoxy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pmkzfcbm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dhykxtmi.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dfsrpvee.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rjaxuluy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wjsimlqb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3blvpojvs.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tomawfpn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hxfwfxdv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qxwzfckn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jvtfocqy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mxqocgma.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3obtgyaur.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jcexkcur.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hrskcjvp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pxlsdoxm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mahdkwgh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fozpykqs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3maxkseem.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gbxbqccr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jnrsdnkf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gxezzldo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ozwsqznr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yvkmgfgp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3valvoknb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rimqxlgd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zoljfnkv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3srooplyq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gasaxlzl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zdrpugog.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3osbutzot.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3luntpbsb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rtdakthm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jbrobtbg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3eyaryefk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rvojjtsi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3brdivkak.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3fbgffpmg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dhsrsexp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lcrxunpr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3malfseyx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wmgnrzue.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltbvoifx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ateszkje.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyjuoheq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bnpfpaza.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3sgxkilmj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3apybezxy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hgybsbjg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rzbykflx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vwqpoakh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ystkuraj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vhdhtmib.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lfjdgerv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3afplaxbo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3brtyohcc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvvintwt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3aujlbczk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgkubrsn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wmeasklk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ifgpixat.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dtszimjd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3guophjpj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3oqhxlwdj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ibzqfnei.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fqbpxdxj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3umzkrbnk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rdcghinx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pkxitetg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lrlcckkl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zumdgdjv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3adbgwzxe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zdurlslm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3eievfymk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jenxvfua.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sjgvmrig.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yzbepkbo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jghifspi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mlytmdbi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ycndptff.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mpcqeckf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3redjblzx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3geqheglq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dqceodyr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rxhgorey.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vscpdinm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrqibjbg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivjtrvjg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lsgridkh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkjogwiy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wplpujul.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sihxcdeo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rtfbijqy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wjfasvym.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3raoyvegr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vhjftucb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ffjtvasc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dbnkovth.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nvcapudd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xcedrdqx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3prhoiqan.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bauaedro.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oursabno.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ghsulfil.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kpkeczta.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rpynuvbu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fnuzuulp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uvqcnovo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bahbeykr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xkamrnix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mssxqhgr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wrjmzfpn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rxsbyugx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nfowpdtk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3orqvyjim.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gugdigki.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cypgfgjo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gmktiubk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqsukfaa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tyeggbzg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmsyvmiv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3eemcsqad.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zicwjwut.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3njvbxcsi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hwwodqjr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fsqnqghn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3owmbcpwv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3pffaipse.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jusyefjv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fcljxjwc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3iyyilidd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qbetrkfs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qgsvphbw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xzbndzuh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3usxjrgxr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zoapnzpc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cafgdebh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qbfzrshv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qdoertuz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3njbzogsw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pgizlbyc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kpzbioym.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3atxivxqq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jtmwhiia.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ylgadvcx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yjogdgqf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jwdhjxis.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yaismqmr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ekiecjbm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3izdrxwrz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwgtsfpa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxletjih.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3revvwtob.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lmswgqso.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxgbtdpj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifdefzql.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tnzqrstk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aradfgsg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kgqrivuh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pskiqbis.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sprmcysz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3erhwzney.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipoxoefv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xazvumya.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qciwthcw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vdyksfom.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xotmisjp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3etyrayaa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zfamovkq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sohvpqni.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yplvgusf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gcgfxpzm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bxpcivjo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3yaljmhzj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jkgnejvr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3yoolypmk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qrhyhhld.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rrdhtuyk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3speweezn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vitjqpoi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rfzmjrzc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3znepikff.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pzwxyqiy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yfiulcbw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iopjgxkn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ensnfuab.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3epjxclin.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3psvmbsgm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fcmnierw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3avnvcrvw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ritdbzgs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wlwinudp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gplvgxpm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3adgfnjlq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wegnieqp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3akbudbth.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umagseyt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zjdbhrca.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tortuyac.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjsstgjw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3naqzlmmo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcduvbcx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrynzmrp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3mlsookfv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfisdacv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydpkybas.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3finuferx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fbrocbua.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tueepudz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jmjslywg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ehpbavfj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ilvqplap.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3furvsydf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xopvwvnr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3htcfcmbm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ifqxdfsz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3wwnqndxt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3cdtlbcjx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ifzjrnki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcfwetlx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3aztfcojh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtufdbfj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qoqouhfj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bnjetbkx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjisirub.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lquxuljw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xxscjobz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnefsjud.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xphxmleq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdwvyuct.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zqwtvohm.html


<!-- 参考信息 -->