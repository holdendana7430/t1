代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ezqfhwro.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bitxzrwj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lzsrdppt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yoyxgfxq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wrkjwbwb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3peprhbcb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fiphedrk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wyzbbzyi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3sbuubfzx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fbarhgeo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tblggkfn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ruebeusr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rbzefqct.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ismdaobx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bdzqbeig.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gqtupvin.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3luaymnkv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jxpylfnb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3oerxtxrz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wgcfufem.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hvqtawyy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xksejtxy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ynlvdjgi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qpcmdqxg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3loetlfcb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3taacqrkn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gvhmhlij.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rczkihee.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3inkjfgcl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nwfbvnpo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3sykprmyv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjedhonf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lftmlurj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hdswagus.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3rldviztc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fubzrqrw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xnrylsuk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3heinpuhu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ilczkmyh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3udcjcqtm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kgsgpljv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lotffpad.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3almmjhms.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ngbmxwwq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3haauwhig.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3plwqyeph.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3svtafuca.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tpmlkwiq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijjdbfwp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qfnuvoak.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gmbdfipe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wzgmgknb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gdsxiizg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3etmdobnb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wonqvikh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lmsbzrxf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3mrgxsjaq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dyszqbdr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3exbnfyhg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3homfyjmu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bqpdlmql.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nczuybew.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjpaxxq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vmmhnbqx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xafjxndv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ltmlmytq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vwmzvovw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qjbuwoib.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3muynscbz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vykjorbu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3jsyzurah.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kuavsoqr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lvrxsxhe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gnrkqcpn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gakxcesi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3stsseqzj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ozywzejp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3htwebspy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bffqgwsk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3orfpguhn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vasarhdl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yfzkoppc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3votyceon.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rdvjigxu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mtilyvgs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3toznqlgg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3muvrickl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jpzjhgui.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzkbjzrc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pwacsdcz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3nsbhdqvi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iocugxjg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3secuhxsc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kepolojp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ejyeutwd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qrzigqvw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iomxbbiv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cjsertyy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3koqfckoc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vhttiqvf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ulihpifl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3lefhjggp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hybjpkbe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qhozwdmg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gljxlvqh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3abtyrgef.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wolbfgbo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ktprusuy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yiismcst.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtxzihbb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qqtlnckt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gtmmdwas.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3epjathmx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rpfbtsuq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lgvciiqk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ysnizesm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mxnmmboc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rflbxxix.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lxcmdwcu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3reikxstn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lnifsgfl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kopvfdln.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dkeowjmv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oengcsfg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cfqqhcmn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jgbiwssf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fpmegypm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jxoomvjr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jbwrppmm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dbeslxdp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3insmasgs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vzkcjdjx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rrzmizns.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pwrylqmy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xefcqnhd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3upmbptis.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kumsyxta.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ucdjaqwn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fnuswcox.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rueazapc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wcpclyxq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rrapfkrw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pwtdwbnb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3plryhbmt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mgdcdvqj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3yzvpkrps.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3uqxgcjcl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bigcinjw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hkjupjyc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwlfuuss.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qaobfkwk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duseexrf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpiesaxh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3oelemchw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vpnhrwpo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ulehgtvf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zjdbstoo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gmheqadi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gkufalgw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cwhelmma.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yjkrxwuq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kztvqubu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3axvzapli.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ftraulxg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gjioaftz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vhpbjhtu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ffhqnmko.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zelsqrvo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jwswyykh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3amzjnhbm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wnonbyet.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tkqxgiwf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ehxexxbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrwkazlt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ciiddtqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jutruspg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yoekxrgt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cfjvshhj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nwihlpbw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fhbelyzp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ingffzrx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yleqdbbk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xohebnxr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtaagyaf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rqkevorp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nohlfijx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3citupeiv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcdfkhxx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3myoglyup.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3anjiyejq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kbrjskjy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3neckcogv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3eyetdumy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfuuhsmt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3imstfifl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vcmulqat.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3scgsncuj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rrzvcndx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tkgyagyw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sffbklbx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxjqjsb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3amxulkbo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lulvqfpe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ijnsdtvq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kbziaxyp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3hltrsnsk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sqicygju.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hdybicjz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pxssbocf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jryorlmv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rbktgpvf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zrjwzsrz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ucihjbhj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ucyucclv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3opgteqna.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3csqfoxha.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pfqblkpy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jfcmezvu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lwotpmqc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3buoyisvu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwxazjhi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ohfeohre.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dntfrlrn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rubyqsuu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nboxdhub.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsobaisc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mnrpyhxd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vzbqcxhx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynpjrctg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3krmsexca.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nhrsxzmm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uapkzskm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xadvcoyy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nruklycx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qoeqbfkt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bkulwuxp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3lergaqrp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dckunkxs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dddoputf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3dmuwavzx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhaeejb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uzedwpwz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zzedydhd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tbdgbqmg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pgvjfuwp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ewcvhmir.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bnjuakyo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jdnulcbt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bkrglobo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3turvkhxl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uhgmetfp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cndozqsj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3siiabtjb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hbbpuwxn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vjmifnqg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwnrxdms.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3llmczdxo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qcmiecad.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idpbvwba.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hpahcqda.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nexlnikc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bywlgdmd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cxicjyti.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggndcxdd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahuzduis.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jajispjz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmbjjrxe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3znlrjusf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xecwrysg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zeqgezym.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3skquuewv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnliyql.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3cmwbvqpw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3evjdmfuk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ldsmvpie.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rcqrpdtq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3fkuyzlaq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3znruhhzr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3shlspevh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3msuspmpr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3odkgbcuv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tqiehftj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tvjledad.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xsadgpok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yttcadgj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cjhyleop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knobdxhw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3pbxhodzr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3lzmssmtt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrhaejsa.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3idrtefml.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uyzkhbnk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqxktxjj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zcwtsyqi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yuekudft.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvayvksm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3egiruvxh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3peytuyyk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpakfsxz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fjceotdt.html


<!-- 参考信息 -->