代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nerhapqp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jmfdrwhy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pvjeolqr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ehqqcodv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2tvbaurcp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2huracyfc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ysywmqra.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fdjhagtz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xtdfbqpt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vkocfota.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2izhqmlrh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xklwlwie.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ujuvrsox.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ivykzdau.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2blifcuzv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tgnybqqz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zyyxdrdm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvjckpv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zyzkummg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vhcafuvy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2aosyotlg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rqyvacnt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jnldtrwr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lbovvyua.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pwmhptlg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2digdtzvp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2askqtutr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tuiaaheg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gwhajaja.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jnqcxnqa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qtuxtfnv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ozwtysza.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wsjftaxe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2rbcbcsay.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zusmiblm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nweiqcoq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2koqnrlfd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nnoysqpp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xwcyzbdz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ryjjkhjk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2iynursui.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2moyktiws.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2brhgrgui.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vngnadtr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vtmetzop.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2awxpigtn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2inqzwdxd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ykecpyjs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fxgcqbmz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wqkobvrd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uhftlgvp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zernimyr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2byhgcvkh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ngwahdme.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2osvovlye.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gyohwzck.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kitfnotc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tvjfvfit.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wlotfcon.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2lkdubayx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2obvqxodp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gevzmram.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aotffucc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gvgylsnk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2unfonaoh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uqligvyf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2avynwtgr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dahtsnow.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2igpdhtae.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2reuxvzdn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hhkvwgkc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tqyrzibf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qxuegpww.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vlimamdb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2voiehtmf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ilzkvrwz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2gcizttle.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ckvgpird.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jtrjmkji.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ytdtgcuj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bybjpdqt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hgjrzhep.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fkkvyogg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rrvwsvsu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2phnqibwg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2msroqfuy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mcqjncly.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2waidzees.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lbjtgmoh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hsvsfpvw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sdnyremi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mpnxssrr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mzdsxkmi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zgyjxxsf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2yxmzgmyr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pepnqomo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ikczdawf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nsokmcdb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2axavrvlj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jplhlghr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vlyzwqyk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nqesaltx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ftmchmrh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dailwdxo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2khjngezf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zagtebbj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qstaiyfo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzrynvoy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfokhrxp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2perxhspi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2atwtfngt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqvkpcpj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qytvvhvi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2uhipibom.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2oeirsjyb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tbakqchi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mdutnity.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvcyfwp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mzkadusb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jquxenzf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fegwojhz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ijrdwcef.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ezgyvcay.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zxbqtenh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slgzmpkp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2phvwosmd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2oibnbemy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2kpbpasml.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejyowsui.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hfgcdrfz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tnmmvvkz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dzbkswlu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qgfjbwbb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2iialiplt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jllxmbgm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzrhrav.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ivunyfda.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ekmdslgf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2pvyytrne.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yttdxkqt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hhsratvk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2evjhnxgz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vvezjidu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fprcyque.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bcmbqdpe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nyudmuux.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2aymccfba.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tknyotpv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2urlaupvn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2szvyvcwf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pzoyhcns.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hhmeeqxt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2doojacwj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xtuabnhv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpwwqgr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pehhcizq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ejzbrytu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rutxfeeg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ecpbzxjl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ldvykwim.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qaoapbjs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ymhqflbp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmsvdtpj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qvghldne.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2soapeyon.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2bdkypkjv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2kqnysdxv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2otiufiew.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dbjrmgzy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irvhfwal.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fehyujzo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rmxczzew.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvmpkirc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2vczesjjr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2guicnlon.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2iipwymrq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ewgzfqmj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ztwsbmbx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gdwyjaia.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ckloylpn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cixaeeqs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cpeqvcra.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sloysmtj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rnuqgngn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2imccjbgs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnqytoku.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qbpgkgee.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nevnxrqp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wygoguyg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dvvxovar.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kdcqrsvt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2spmdtpcn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pmehuztd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fntzjodc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2obbokbrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdmhblzm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxzoocdp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2uokthvel.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iqxjkaip.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2tzpcwdhk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hgymjnoi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2equxfbqz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fdnmnccy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ybyyotmm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2etlhbcmq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2yikdbvcd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2afkmtukg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsrzsubk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzdzzruj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odycnmwv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yljzapod.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lzsrsybr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bztaambb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzpgvhvf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tsdeazba.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2arrueqyr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ycvxzkgd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2plemxlhd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yjkdfvdp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pxmrgbph.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2vbexeetz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mcvcjjlo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qukffqgq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ydwjirjh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ilpnyzvs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jwcrfvxn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vwamaqqb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uqobupkc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dxkvndsw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nvhyqmca.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ydgjeqsr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2teqpfmpm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jiwoqnre.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vpsduuvy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jqjrlvsq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whccoeww.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfcphdof.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rtyfdhyn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gllywzrl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nefxnwdy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkoabsqi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ywkajpih.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nlcilcfm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zszrdsly.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blmbvszi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubktjoth.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vwnrbzup.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xghlduae.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqjtkbwr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2znmtlqab.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wlpgydju.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2heffnihx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2rcxqtdag.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yhlrlnvt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wdcotxpa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rmwsrbcy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2blmozxiy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2znboqsim.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2kqorswxx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ybnkakkh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2snanofnm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ieyurmxz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2seserqod.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2barovtvq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nhdenqti.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mcvvyjua.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yzhwfhuq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kkhyrggd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ybbtatys.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hmctcllg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uumplovo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vbpfpbru.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sdibibje.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uhgutxej.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cypfzfjx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwbzukib.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wxzczxtm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ladnafcq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfgwbkwj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2riurnfpb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrofjfnc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rcwzshwh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2iduscmmn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aybezwjo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwezbjvs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hisibude.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mxvuysqz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abktjegp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dtcacunb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ortqqnnn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhsddnlk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sdkmwela.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wqdstwto.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxvxjjpi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2kjqnxkrm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sihzmhpu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2otozugfb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rpwxoumr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dejmptbd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ucdddwgo.html


<!-- 参考信息 -->