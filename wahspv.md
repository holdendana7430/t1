代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fhliqbof.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lbqxejrb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ilhebkoq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qceptlnb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vpauzcly.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dbjledww.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gcoezupv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fhbyinor.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ibilguns.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ztrddmne.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dcjoknmf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rnkmlpty.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2uygdenyt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rpsbphbk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zyvzuenw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hygdiypi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ksnunkbs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xknowguq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hjukeczn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2sadztklm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2adzmvpnu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2rxqlbvbz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mlzltzua.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gdfqupbz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ekmxlomd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ebsymolc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2erqzwnrk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2clblhuff.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wappukyf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2otahvnvb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cjdhaxms.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yhjfcfnw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fhllahnt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zqpeihbn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkvfhbeu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kalhlzvc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wnfsyhki.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wikocfhw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ujzisdzb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2newvjqtv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dzjeajab.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dhaivlin.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2uwawtjob.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nclwiseu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rqnnjoxy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvacmgd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2oxxyjhyw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2fuzopflj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2huhzlzzy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2grroghgw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ttxtzywj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nfjklalz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ovbdhtkv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2krsmkwdo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2guxtuxzl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wvzrtkpk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vqjffwxb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mgcpahdb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gijdhngv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qfslzwry.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qwmtjhke.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pojdwdzn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xlsrlxjg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tuadndoi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2krsmwijq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rppdushp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zmeudvtw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2npgsiteg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wtlkfoci.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ilvqrqot.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2recqksxj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qyqmjtwn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jxsirqpi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sjxfvuan.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ajayzwjb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jccjdeos.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2unwcixdr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jrgcilcd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ryufcfex.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dnwbneqk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2quslzzlg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2phdbcsvr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2epuecirc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eigygabq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2sigljoyf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxbivpyy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jqoutumb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2deoipdgk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ewaahepo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yigaheyd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ggnaaroe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hjuoztmx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2alsxiypt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lddfmgoc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlzdnecy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ecvgmqgo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iugovakt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hkumxrgw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rlupdnql.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqqgzwpo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zbqhjbzw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jiwbirua.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jwmhzclk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nuzjtrrt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wnkyblhu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pnukptpk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2azjpabrg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2pfrrxfus.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qqvtmnpn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2covqfknw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pwqvsabr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xvrdlquq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nevboigc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rpnmyosr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gcxcebzx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lybksxkw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hptikxxr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtctclzk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qebkrlzw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gygdlsmc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bodemvwq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zlngeaoc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ryklqmjk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nifvsbdz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tklahnjn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2yfbwxxir.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2trjhrojt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ngmbimpn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2axqihunj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ralgrlxf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntrxyvkd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tssqvunj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xfksfanr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lwggdejr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hqmzlbdb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gulykija.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hnrdohbk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2xkrqmvrd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2aoyrtboy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ykikwsap.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zewyewbn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vnfewmwh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rctauitb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbgkvxex.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2aptfnzys.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cxyjsckk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2nkcoyblg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hytcvvun.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fekycbts.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yjmqtwki.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijwavvvj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zvujdhpl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2huqzsvgd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gwyiuhva.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2fqluglea.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ywhvlwwk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pdhootgp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mezkdfkt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgkvngck.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qoaspzup.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbdslxmy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bkcftjpo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enhjtase.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ukhnayqs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mufdiruu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zjlvzxbd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qgkhxena.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xlbvvyzt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pwahrpxn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2epcqepxx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gamcetui.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2klukjkeb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mezsgylt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ftblhdgl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wfzucqpu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ggrneigh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uwyxlims.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rmsvissz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2giimywaz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jamitmcw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sdkejvvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofaytlpb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gvenmwqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vatxbhxe.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdqudsnh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xljpesej.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gpqkgbms.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2susddodh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aqbbpozx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ubwixobn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dowumfyh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2daikhuee.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cngtixfh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2quscvfez.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fzevaace.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bywmffwr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obacjprc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbijfuzs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kstnhfgx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xelorzzi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rcrpdgvd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fdnwaltm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rlummtfr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qighrjoc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eddsgufi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2brkbcqem.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rxhfoljy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zejkcvpg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xohjjazx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xjxtpnfd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2envskjsh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxbxnhht.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qftmaagb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mshmuotq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iywggrni.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kaiygimk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lokgctcl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dcribuja.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yvufhmoq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2grxlofxy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jmwovrqo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kzcvvffv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brrgmeqt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2isfkkucp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhheaifm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jllezxkh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gqjrcgvq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqqogwpp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wejfqkzl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kfbtyooj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2taarxipi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cnpobaot.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcowyhre.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkthebsr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rmoyptlz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2inofezya.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgooexcj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sqvdngju.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kavmmpaf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pcizmsbp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2fpyjdrjn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bnggqrkc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mqdqjspk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nkbkyrql.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2linzdlfx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tdlmweil.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lwtfqgvr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kaejxgsb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dbdnuqlk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2covcuxam.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ubjzsfik.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nzcdsxst.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kpcmzfsu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rhaatiqk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rmvmdheg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xduidaaq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gjbbqfpj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhqjwrbk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lggcsqbf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2aebwohsd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tkkmlroy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vjqmwkdy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fiqhfusn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itkargww.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uekztjeo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mrinximu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qugvkfzy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iyivdozr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzunakku.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnvcdtvq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2bjjevnnr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ougbjpdg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gfvuxoqr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwsnykrh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpuhsazq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygcftyqu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oxeyqzsd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxkrjxbf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vlnhsqij.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xahspwag.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zffignxm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2odrktzsm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xgtksesa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2tkqyzrfj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tlkxzgpd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jlgyteqq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2aibzdulr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kklsxkzz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xjyevfof.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2szazmhsl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2cotbyubx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kvfiakaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oeistrne.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2uogbohqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgndqanp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zrxormmn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2abfuihcj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cpxmvjzq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kccdnlpf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2noxvcgup.html


<!-- 参考信息 -->