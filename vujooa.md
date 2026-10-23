代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3evepbcgn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkpjqzk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vxceymzh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mymquuco.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rxyuuymy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wvyspcdn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qimbbubf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3djubifhq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3wokoxzsq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wsathjsn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ntbonnkk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ebqgewyt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jsxmtbcc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hlftcaqe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kpzmnmvo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nmqaisso.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vtreblck.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cimzahmc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ecaclzzw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3onfouxhq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zzrnhqux.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qajzpwec.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hvfkcyho.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3axfuvtpr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3stcgigxd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgiglfkv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aohsaopl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3otcpwbdu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mywzgkem.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jhuecexr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3eniazvkc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3znfvmnvm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jlqxzuzf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wrllptiv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nblaiqmd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aqdrlfzz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nqyhhlnb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jssmkcge.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3juzjghkh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxgkvsfj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3kopyapzj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rpcmqbua.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3spkbwias.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3otmlhoya.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3nqnccgdi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zubefgex.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3olhbvmhn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hsxqmivu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ubwqvogc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pyeayjbz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nqawxlrl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3podxcibs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yhvijauj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3umnvqyae.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ygsyrgtt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bpksvwgx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mnatwsga.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3yngzxvod.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ttreczri.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jqsulghc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jjfshdxk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3klszsdvq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3xxoiaytg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gdbtezum.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qxaqehaf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fuebvccd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zwiykart.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wxpjnlux.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ikhxqzin.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lppqmrwa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qghshtiu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3igamkzvf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dvkqkbpa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mezjtkkz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ayirwiez.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jdvtukni.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dcsynrss.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3coispggh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bqizmfge.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3izrkascf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3unzfjxpg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vowicbdk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pnkfxhmy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qeeqzgsg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kkhxqvqh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kuebsvla.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3yawlaxac.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3iswirvbl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pbjdiehk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpetnjxf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ntukduha.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dpclgebr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rkdagheo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mylozjji.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ipmxmvdb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xymduijj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3odspvnmi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pqctkfvz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pskylvmq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fjizgtqe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3okvejhor.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kfeufcsf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ovlllaxu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3orhpnvfn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lixkuryr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kravbfzr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txeurmnv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mxwfzdqp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gohkaeqq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mnggkfho.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rhnnfifl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3debmcbdr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsddajy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vizsejif.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mevlxdet.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lpxlgowj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wtdkfsoj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ngjhwqrd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vdkgbffe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qoasljtd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pivzlusq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3fxzsfzbw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lqqnjqcc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cedudsdt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mfjaaovd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hadqbcuc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxlqdqre.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dvzvnrve.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3egtdsmis.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kceiyiug.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3grioonok.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qbutizfq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hpgapcpy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3uonzzotc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dydetjjd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xursnmya.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xtqmxiux.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vnypcfbo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qlkncflf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jrqqgylh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kjoeewfm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xaisjyzk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tddmtovc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhxnfutg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3iojbdvdt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3sretkhtk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kseokiwt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tgktcnlp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mtlqbiib.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ghjkfczd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kvtgezwa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lvkfqkyp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jmpjrpup.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mxsgjaaw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwnvglkd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krmdwdvq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqdyoxsp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yrsnczct.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3nhtscskj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jygieaem.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3hobewdjs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3alynklov.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dlyzrsmr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vkouigpq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3difnrtrp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ufgpfvka.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wgtgpqfr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zybtexej.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3edmfntrj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3kyblluqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kmcmsjcd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qaxlmnwx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xqtvhuxp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mjaltmaw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mfgjxgsg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vvrmlppm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pvtnlfjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqfgqawq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fxuebyfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3famjdebu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kjglcyxv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lttfjbjx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qllvwkea.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jemqnfvy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sbxqowvo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3erspfoby.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3drcumhui.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3giiwrkdx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kvdwokha.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lbxuslwf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3uarxpkek.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3drfzcnzv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hlnparre.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ukjrsvwg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ofuycfly.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kqtdqppk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3aqwmpbnv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3aoippneq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bnyjjpcf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3eyxbylrf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wpepjsho.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bufeaplc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kzlyrdik.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kqeotzvt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3icknrggw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ypsyzsqo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3akmrnysn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vrkzjbdr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eylbaxrx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3iwfhqibi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qeccrzco.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zcsceveh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gfhckhqi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3judhhroi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kyxkjcan.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bhpbzfla.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jedmldat.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wjqjznih.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oatqvkrb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojnordfb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bppqhjxo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wnviludi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pmtgbfqf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvjnnrti.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxwtsvyb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hvekueqh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3baqbaaam.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3slntqpga.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wiflwpls.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgbarlic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rijegwxy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggttqbgj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdpetdob.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mmuczgkm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rdeaadxk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3okgnghop.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3puujztxi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iizjglrk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uynnwhpi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qunaggki.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3itmgvnsc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ldmmygzk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vijbwajb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zictnnmt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3epikwjpb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hppayzlm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vzzqqszy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dvbgpeks.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ncdrfcwe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mohfsgfo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xthxvqjg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dnerfenp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yatfpena.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zriqcqna.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hrgzqxbx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nozwqegq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tzoyccup.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rgovjpyt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3eabhfzdq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncslwkuo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zwlqcjdr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3grsdugpn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jobgnsha.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aegpdudj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qxtuiuqm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrvxvesp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3uczfqqtj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmxvoriw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwjbehyu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxhjyxqj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfjkpnwc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwwdczui.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3plhtpmbu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqiclmci.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aldvanjp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hxxnczjf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3naozhkty.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htnnxerd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3qgxidzoz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hjkruxus.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3plqtoeyy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ruhsmqzm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zndcvaun.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tzvjqauc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3desfpwvh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3atnlpbwc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3sauujynw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vozfklxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmcnxhpr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3myweqtxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtzydnzu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3eccbeouu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rtaqnfsy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3msspswww.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aursggaa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zelzmvlc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3trhhjioo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3daogtjpr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkjwlaxd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ojniglis.html


<!-- 参考信息 -->