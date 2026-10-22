代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ejmykchu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2uejrpjbt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2evnqpdri.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kkbrssnl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ngdsuksg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tadgrgxi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lsufhzmb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jjlchlki.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ljzrwari.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gpdwzgys.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bdygqczd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qetodgry.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2juieqewg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zldpvvqd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zpgzoicw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2myrgbgxs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ceabglgu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vdguuqsc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bcppeoqd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jgalmpan.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2imtkdhgf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fhvipsqx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jvyoqwmj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ltqxxeqa.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uquqvhjz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yxhqusrs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ivodlyoq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ryamgecc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qomkpbah.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sdzphdbn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2iyrocxgh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jfsdaqrs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2davvdybq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mvboieda.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mzjficsi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dgpesxdh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dlirykta.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zmwtbsyc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qlwwyjpi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2shgqmevg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zptextuj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cjrobxxv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ulwddnte.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nfblnfvr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbotzehr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2opepshvs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ggcrpemf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2owokubhr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ljjeyexy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ugvdcmcv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gxwfmlle.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tleivsig.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mgydqtsg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ydwvaori.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2vaszgpob.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vqsqyhff.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lmpwlcrf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bfwgarbb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkhqmzf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sdvkpajx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2skjjzxyq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2esnnxvmg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hteyjapu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hitudbcy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pflllgpa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gtpqbgqi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qizwsxuo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zfnwlzew.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2btvfgugx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ucmmijql.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2oeeoitmk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ahnuhiwh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2snmppxes.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2inwdzoce.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjzjuelm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rssohqmz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2phpovget.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lieqgikt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2edgntstu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2kvnqbitz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qdtqvupy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bnrpxbia.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2muttisip.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jtxdinhi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kwojudcd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kvqdmsug.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2aiexwebf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fbsxqxeu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rbldpbwa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2adtvtqbn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vqdpplof.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2muetyedp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umouprpj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdrbaoj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xhsscger.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rrghsuch.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nxcfhxoj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2mmjftdih.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egbiiutg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lyflahxx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjnyxehg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2erxreoye.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cfcsqlrx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ffygjjnw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfvjgqkh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gjuipgme.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lzzppbho.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zpcnuhwz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jyvopvmk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jsyqhlmc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2erkdoajn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpyypwu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vkbwlakc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wqlthdwk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bdsgcreh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2oxicrizr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ypgmdwzq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2numhdbvn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtvzmita.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cloobltx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrxzkvtc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bopgwcah.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zjtjqlch.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ozpnbzeb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kdgeoton.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xcoxespx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zyqmqquh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zeojjtju.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tpvtcime.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uihuuvbl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2njhprzek.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2anyaujmm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xaqwngdh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2odpiwrtk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2akhjuxnx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qtpnskax.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eregjmsp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pgiisnzw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cdddrylv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ghximqcp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2blxxrqnf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bvfoyked.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hqelzljj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2yzbeydzh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mbmzvzzt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkjdoovg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jybngmry.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lvavtrcl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jhtylzrj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ilhntjtj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2fuqtfsxo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ktagpwcf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2nzfkurrc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uajyndzp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2redidnys.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ecflklkw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fzqvhpve.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tinloojp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2msnoehmv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ehshsrvf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zvzvxevf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjgwnuec.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gcghhflq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2slhqcgsw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2evtubuof.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2excumyiz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xawyehgt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fllgejer.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rkhojewc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dytqsbuf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2frakojsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zennsycd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jpgyqwbc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2yeffddwp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fjtpvywc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dkpqxdlc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2maqfzrng.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pqymrbsm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xckpvlmb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bufeyyde.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rrqnupmu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqfdmujx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2oyvfnzsh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ohylcnzi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bkluzvdv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaxtvkdw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gonypzyz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2etiwubxh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mjudistx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vaedilic.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2scwcsgoa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mgelglas.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cjmzlumg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yhvrlgnz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ljrbwdzl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ukvxzcvh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2mnfmehnv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2corhmvxh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2smptgbex.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2itcgjryy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kmjrgwje.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vmiywjoo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hkdpbfzx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iawyazkp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cusmizwn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nsacszkb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wrpwsfmt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gxmxhley.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uwpmfvvz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2waeawzlm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dsfvwcuz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqgwusxk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcniqrok.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2plpqidqm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zcapxuvv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wrhktsuc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eatxdyfo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2iljowifq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqtxckgv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2djatymns.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxehxlrw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmqbrets.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xuoxsccn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2myhuyrqr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2entsbszt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2giaaeamm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ogjmbsll.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lslrazje.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xachzbee.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wvrsrukq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yycbqxbj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2whdtnane.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kzusjbyz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jhwhdcyr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qjreegne.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2whghprzw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mzmsmwjx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhcttmsh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ngpvrsmt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nimzvrct.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xhihurka.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wrcrawgc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2aclrjzjw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ejkzbooe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2piuygale.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgxlrtbw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhcxsotg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mzecfmfo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nvxxnuci.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2syehwukk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pdxvskbt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bfaarfpq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wldzgwxl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hgwseslx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipbhzgct.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rxebopqh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nxharlzo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2keefsydx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nqodbyxe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xndhkmcw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faeemwly.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2alkjfekx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2uoymmyuh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipojaynn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uhewfdjk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aegsmhmd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2quezjafj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rpodrxzm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qtnrztlv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hejdjwcq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dhemyiqi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fyfxrtyr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wvqlmmfa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wwovpvgq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cvzcxjhk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ordzssfs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mmhhpbxu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2amqftnks.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ctoyqucc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nmcnzvil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojxkgauq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ymywdzte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stkoutlm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hlnajyix.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tzaoveqm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajnduzzk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zqzeslsn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yfjzkwno.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2uklrasud.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2whsffrat.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yicjhkzj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jwvzgrkd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hnfxesii.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wtstbonj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ztydcprb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tlizrdof.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kujmybyy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kyxcybhe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zmkcfffn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtotpwfz.html


<!-- 参考信息 -->