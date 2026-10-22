代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndqcwnul.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rwlsgqco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ispixvlh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2blgdpnfh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ximiyony.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bitnznph.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2igphdffy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vzwhjtxx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2oijozglf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zhcrnjiv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nsecbzrl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2anqvxplh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ujrjbkbi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jqazahhj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ntbfsojc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2chikswxc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gvnoeteq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2amucrhrq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wflinjuj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2urylovvf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fupjguwb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mkrjxjtk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2njyvbfqg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lskaenne.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oqixbqie.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fdynorpf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hubxembh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2staqermc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bvyxvpld.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rtnzyfra.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zoegdgek.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jgydlmpx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tjcfnguo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2svhnzvxu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kpmpmqas.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jepaqyao.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2unsadbyr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2orostilr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iseikvtq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ncmxcbyi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hejnmeiy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2svcelkhu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2evdwjzjt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wzfehfak.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2giqyrisx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wqikccvx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lfozonfw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wrddjorp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hzntzafp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qyudwnbf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tirxmrxt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xvmqkpmb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xdvprybo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hdewrqfx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wjctwsuj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jvfnuhxu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uqriyzdm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2iwamyjba.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lhymqszr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fqusixkd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cgbndmlv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bgrpkroz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2evecmjbu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dzqiljra.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kmxcfwlv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gzvmhjxb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bsgcckfb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nsxwoirn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fhdbtfkd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ixthpuej.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rezercjl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vlpvrcrx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xlgpcluu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uifkakue.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rtkttauo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wyrmtvkd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wcdknzpc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jucllgsx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ogxdxxmc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2grkyfmai.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bpajtptx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2imixpvaw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gfjfhcjg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dkqjttfc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pujcxtgw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2osqpapoh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gnivgoey.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ktzedavp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qlrqvfll.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uugcnuta.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xzjpzkxn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xxurjthp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tlecdazg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mwutgvho.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2viijncfx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rujuvvpd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fgdqrqby.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zwdjshto.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2glnhgmvg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yvyuhdds.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2npgsajis.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jdmpbihf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dfgcicwe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2oukyjuwa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mrxorjav.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gswvbugx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xocafjtr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nucjjajp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2eqiparnz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2unjalwmk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jwradwck.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jfvwjvuk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fnxwdaao.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lzttmuhi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qryveojk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qpkdqohv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dygnocko.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wjngmmyg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2sxzeufdj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayfbinza.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ddnwakiz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fgweadnt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2urvkzpnc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2nwxuiykp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcbaxyqs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uycljqhi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2elgwiatf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vecgantl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pmrmgsjg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2fqjkryoe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2uclrckus.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2qnhlbbpw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdlvkbau.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fpsbaajq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nrfeeslh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ubrogtrq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2txbfylqh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qpkyterv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jxmloazo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yyixhtui.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jnynvlvw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nixaaais.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fllwimoy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oaicfibz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rvpvwfup.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uncbtzxf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2uikoompx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wdmgbexu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mncwihqd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jnoxlldn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nehocnjj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qexpbyio.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmjlzqso.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dzvaudqg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dmcwbams.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vlrbxeqb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ziksqwzh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mvjeikud.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zzcizdda.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eblzvwjd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hiusjick.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kemppeqp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2adomuftp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ljzlqdmy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nlifotww.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2aiffasft.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zagjedoe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lwgvolpp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pkedftgp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mbcosgxc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pxlvqwlu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ranntmjw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2eqbvfdjn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2uvzrejwv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nzmcxdjb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zpmtjvdr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pygzpdue.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzvyqsdo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2humiotbr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2soxqbpqp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktxtxldn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2civxgusn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbtdrcyv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vmtucwnr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gausgmcg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wxzhujkd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nmcgfnii.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kmagitge.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zudnnzey.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vrpiwyjx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2egiivlfc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hizcbgem.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fkltzgle.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qhwsxrze.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jvtlvdzh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2khmegvcm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qvqcpasz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fhiiwwxd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mgiqzfvd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xkndlmba.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jzgvgqhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffrqfgrf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2smwqlhad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eapiyout.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fczsiewl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2auebdiwo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2enoyazno.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2oscuxgun.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bxqzdbcr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lnhlblsu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2iktxvuwz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdxzlswl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vaeufaub.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wiqwpppv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2raymjawe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rvkhuhfw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rhvjotad.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qystfbho.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2clxfvudx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dijfifat.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rmpvtthe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfmimssn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2acmqskre.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kwewfuzo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mrlvjtdi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jumkvaqf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zkachppx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gexjlqke.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xdsyyvmh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jzzrrydf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dolrmujf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2uozohrhs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kbxgyyix.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2oflktocv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hasdxwkl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hslmcccn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yqojhybx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tmcanvvj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2skduuwvh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pssjdodj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qegwbgxo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jxhnbkir.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iijzzhgr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qpgggkxi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wekxbxqq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2drngzmpt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2yttcxipc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vcdgwdec.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdvnspco.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxgylpfo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2enrhdgbm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qgbiudbi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdceyppk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mkhyrqew.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uzuzapmf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jswlauoq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppjkoybe.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dxlzqwjf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2yvdbdrjo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cymcdrjf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wpsisexy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jlslvnvs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tgfjkqhq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fpxjcxrv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mevfcrrj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rpblhdhi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ubpnzeow.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2amlffdjl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xioktyou.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2glhaqgfg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xxuqyilw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kxpjrplo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2afbgjrbr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gmztyipm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rymisxrt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rzhecafm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ivmdnzii.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrctojhs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hmbacbah.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bhqojkll.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kyhqgrdl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kfiqyzfi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cxtbziim.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agymalmp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gsphdqhu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dhmcjddx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfgfjavl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czqnmcqq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjsvsezb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbbybuhi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ruxepcdo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asmgqcaq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqnjfjet.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2torasoeo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2chaztwvc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yabpsvdt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nsxndeht.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cipzbegn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulgguxqd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2amfseuqa.html


<!-- 参考信息 -->