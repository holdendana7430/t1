代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vxmvvfvc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fkmrymsg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3utoyugik.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nahgaley.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3igsiidvm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jzirbcmn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ksauedvu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3pijakscm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vdgsfbmz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dsijdmcf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3oknhsshe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3foazlsma.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3upmbewss.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3irsjwiby.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3olwgnaux.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wrmcehkh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jxdyahjy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jggwclmm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvulewnb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ebphniop.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nweerajz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3sbjhmosv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ylqlvwkq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jbdswvey.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lwnuxyrs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lpylarzj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vlvqxrkd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmihsows.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hbhpmwsf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3sddtblfo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mjxwwifv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mupvukhp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3tgogaxaw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uucwjtly.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gimyybbn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3widdiecc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zjjthudd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tcadawfp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dsehldze.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ibflvcjt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ccrxgyuv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3keclqpwh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gveqitvf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xvipmsuy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3incqygyo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3aosrzorp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pgwpmfcp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3npqvzhti.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3emcflvvo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pvwljeuh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wpclhkgl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3houfslfz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tcdtchkg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wmogkjcz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mpuvqmsg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uzmlydjj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nswptlpf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3pzvoismq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zhoevwmm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fbqeirim.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mdpvfpgi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pasfihtd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mpdalypj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3olwvezem.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3msgpgdah.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cwrteqyk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lnilwlss.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xheqljcd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3klduzyxh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qsbgduxd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ktqanftr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jkbvsndz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tayjhmoe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lmaiiota.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lgkphcse.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bwsvhxoy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3pnmcwhnx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3edeefqkk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nmdxawrk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yyjsvcre.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3glhtipyx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kgbeohcx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tadqztky.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfqzckvz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wmmubang.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3otjaihaz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mflqmzgc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ligbnvcx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mfrtttwc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3arnuupwg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zmbmdjcy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rgqhpvgn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ftrhofrr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3nncrvike.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nxfqwrkl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ikllqyrc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xzhafgtw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wujsrtxj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pqebwhki.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvazbtks.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxgfsio.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vmptsvgx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ettcvntg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3oewqghsy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xjsnsnxu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3oypbodli.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ksdljoum.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fbeuxugq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qlptvegk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tbrhmgmv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3twmnohbq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3btpplsad.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fxsheipt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzjzbtxg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3imzaljoa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3poqmvdpm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xewhhimi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3aqntfjbo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bkesrgvb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bojiijpi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zwhcyzxu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3egkilupu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mrnuqhxe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aumyluzp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ztekkvnn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pwhbiqdz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aduijame.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bkffdniv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3swwlrmso.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3iqkmdkgi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gfjeodrq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3biwogjus.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wmdrochu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dgcruczw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ktmwdfac.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3moypwtbs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mmrcfcft.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3sqdgyemm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3utylkfky.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3izvmmwpk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3joyhqens.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gorzvaul.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gnmdrntz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcgdbeeb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3manmfqmi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3tvdepury.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnwoincn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fmnnnktk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3irgexdfl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hpjuezqu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oubxvmtd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vbwlufan.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3itjwqplk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ycfoarls.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3svuelcbe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3munywoge.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nothenvo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrlzlbuj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lvyaodna.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rhgrazgz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3euzijjzq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3idcpakkd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mtpgosox.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ibmlyoiw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wlinknsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuhrfwmg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pktezzns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljwjnmrd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oisikgim.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qgnyjewl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3idhlzpna.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ukhxfmoe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3slrcwkzw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zygkzcps.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3docbbfml.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ilzjoybz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bgqbcsqd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbsdjhlj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xkobedrn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3flrwmsgp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iafeagom.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxbqtzfd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hmqeemzq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tarklusj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zndykuoo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mgmcwtpw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rmrywder.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3khaaawik.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3atbgzwqf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dhyraltt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zmqqueuv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fwknxbxg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gqpxftrd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ngnxakwv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kqtnwbhh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rhnuxdtq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gfoqaggd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xjearkhw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3okkukvxa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3umjxvztg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pvaaggzk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xapfdfmu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vuillwbf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ggonsbek.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pjjpnoon.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3blrigghb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vizjwndv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwzlhibw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdizkmok.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxdtxtht.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3stmtfkxe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agweipnd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkxqiltv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cgjrkrxn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fwismygy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gpmzdhdn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwyrdvmk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xypvjngd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vkavdkye.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aipkyjbq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snjyhexu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qjyhlmcd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3edfszgdp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3oxyepqmh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gftcymox.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ozoanvee.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lwpqfehj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vdmrnyxo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3yjfpkplj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bpolvjuj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3orhrmzid.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xirqrzyr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wkivmrht.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jdluiwkk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3llobtthg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zrnzkknp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iuigmmse.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3conghquw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3erpsqowl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vsmhxjld.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bvslgoyf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfzruxbx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qonelhgp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vltsrsem.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ewltlrnc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xnwnwldw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3svsssvfc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqpvxhxb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3tzueeeml.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zmmzzljv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zmztprdi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cbszpeoe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awhehjil.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dswriwey.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ljswnszk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dliyiukj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wztdskli.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hrogsnvq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnfyvllu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txayhcxh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3sdnzuqhc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfkuzxbo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwfvkzrj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xttzdvfc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3nszfwvxx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yisvyhww.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bpfmikzr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xsxmhogm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gwlcknqu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gcpvbfvi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3walbjdoi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ezgouwzv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3txfujdol.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hgbsjcog.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gjgbinhx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lnlylhml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojbjjutc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ochswjek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjvoneme.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bvwfgqws.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3imhmcegt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qvshiqwn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qbsumvbi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rubjaitc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukprlywt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hrqagaxc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jqbszbcc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3khbqszuq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ysraofhu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3umxadeyn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aryqgziu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgvnlkze.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phjqrkdr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ahzqkpxl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rmqkwaeb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvwdyfxt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nllezbni.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ycumbhgt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hcnbpcrd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xyidgoen.html


<!-- 参考信息 -->