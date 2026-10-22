代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oubbtfhh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zutskttp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dlezexep.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wemyxpjg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gngjvsyp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uvkqkhku.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lpqcyoia.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2drwbltkx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sshpypcp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2hjrbclqh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zebyozfp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sewkkboi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2stzhikye.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gguzhxnm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rjeceavv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rrrghxfr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hbpkcftc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nzzfijxr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hhcyjklt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2veuyfcdm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ucreaxpe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uysrpxql.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ngaralrq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ovrejxur.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wwxzoskd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bjatnlfc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tartfjle.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jecacxat.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dtkmkccw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jzptlpnd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shryzguw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yaxdbbdn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zcnlcyxp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2scpoqyig.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2bijgrxpy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lwheponf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rghfnusi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2scsroqmy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ffwsqmrs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2imsedojg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mvgouokp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nnrdhmki.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hhkxdqhp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdwwgce.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2uxcasmzz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qpdbvtqh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2appawejr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2arbxjivz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2oopzffvj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qowhcval.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fwkxnvyy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wfsvfadb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvhcrhgx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uglgtbvw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kueqtiyq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2aqqyerbo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ysithfcq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tjwoslid.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cxlpegfv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zbmfvsmx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2sdvwaepy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gimsuele.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fyvaojvb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dgmgewka.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2glnfvjmj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sjhrxblh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tpmazmju.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jnyinlez.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bromjzzu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2smkpiysl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2weugfofd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2reahsmgd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tikarcfk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vaxcdgai.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dsibzoub.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dzllcpjr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2exwrqmmt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iunootnd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lyatctab.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fmcinrre.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2sfipyowt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cnjknqkf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2etydcats.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2aouavdlp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2spmdbcqi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cmwbjfpq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ftebpxnz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpczdhcg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cibxwksq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeakpswc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvqvevfc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kectvzio.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tucipafr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2yhobansp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2usatmsfr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdqptvmc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vknjdfcw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bsughukf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqwmrsmx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qlutfubg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kfszetoy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lyyuyngx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dpdckvsa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uhdachyb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zkewomds.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2pyclrqnx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2doswvhll.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2conadaqr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqspvost.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kcfyoqgb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2skcbtmrz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hrddnoqv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xirzusms.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdzafwu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hffjssly.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2juwjdpju.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jedmxzmy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2grnbvwis.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vvdbbcae.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hdyjnoui.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vnfsokdi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lcrqtmka.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ykmgviwk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2draqjdtc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2epufpagx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2duktxufx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qwmohhjf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ttczemaz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymkjndlj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ofekkdzm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oabwrbna.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vaukymei.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wokuwesi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2favqzinq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ysjedsgo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wufztsgm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gfynsadl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ucdnnzuy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oreiainp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2waojyjki.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fhsdnlio.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nbbdfbun.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hmdbciap.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zimznfdp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zknpfibd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pnnrnyiy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ignxumec.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mnholilm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2doneegkk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ikrhzleo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2moqatdkf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2oskmokfy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2sglwzteb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrdrupac.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucsebjur.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2caornlqw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2qioqkeju.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mueswqci.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hasyondk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2htmqoaqf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2nwvxcrbu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sjuonwii.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xmdqhanh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aptiqxde.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wjekxfxy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kgbybqfr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uvjrhqlw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hshjwwol.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qkxmhxax.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2evsoeail.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jdrwlnpm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zjrhfirn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hpdzrprb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wiyxjvnv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2nbzmdmpu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wjpeelkd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wntwacxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euzzuvat.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nxbixiup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edjwkaom.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqheoahi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jkjiwyoc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mtgctmga.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rcqlfutu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dslkwnid.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fetxwvrx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uyujumjo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwhhxqtx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xwlimwkp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2bplwfofn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2emuaielw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkrrtims.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jdjktcvc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nsfswmpx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vbijjsiw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mjddyhlp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wzsxhbhh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yawoejcq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ylxnqzag.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hqcnhgwj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tgqzapxy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2evubtryk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2panmkbxj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tpavbcyw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qvffkxtw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2sfrrfzrb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ouddfajm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjpzpjww.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qzavtyjg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2aoanwevi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tffiozpn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jjusjnrm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2faafajol.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2styumhvr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cwjcqdlc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qbjnpume.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uyviwsym.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ccbjwjrd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqawrwqi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ancgbmkt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpjmohbg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kagueogt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qpdvpgqh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jvwmktlx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zipnpafo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hnkqxspx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfcgetxd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2svqwzqap.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxtvpiul.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elhckumi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vjsakhxu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2astvusgj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqmyxhob.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lpcjsftb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lligpsxl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhgmcql.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2byzewjaa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nicqbkcd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lcubogci.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fpccpoel.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hiseqvkl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2laojdgxx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ttfibqhw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uffuorhj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nveivwjp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2feanpbor.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2stnhxalx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2odpiknse.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xhsrrcti.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2edemadph.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2sxsczlny.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nwhhfdfr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2uybguygc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2guzucgqd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ubjigeqq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fnwfpnqr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uqgaxujg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ztgbepqb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xjwpnylo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbcmixyv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zbexqqyu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fxsqbhci.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfovgves.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lgfyaeja.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vomjsykc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cisowohi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vxbwwwjt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhsscmvd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qihetrqv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skuurxte.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fijxnotl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmamkrlw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rcieujgu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmfelayt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qagrwvxo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eyyhfqxk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2acfmidxh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kimmluub.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ybcrpeoc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gwbqdmdg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zasuqhao.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tyqdqahu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hplvejli.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dtmvfrro.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eeplowlq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2redwnnpu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ukufeiej.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2iqxlvuwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlskqrdj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2nuvzvgqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tffgxqda.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2boqznbkk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2eqohthwk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2atyzshmw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2korlfwlc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hynvzcmn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxpclgoo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tyzcowob.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2thganxnl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2slnnnfbw.html


<!-- 参考信息 -->