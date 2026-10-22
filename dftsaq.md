代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mbbtqypp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wpfzcmpt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vjqsjvsp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wiodnnbp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hsnjcxdq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2kjlvvqyj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kapnqcel.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2awcctbmp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ehgrhwji.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cnfiqfsb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tabkbwdy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jewlagsf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vreymcju.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kdvhkbei.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yexhwrkg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sjeetxqd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ilmvtnij.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2turnwpcl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aemkjkln.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aocxsugi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ydajmrzq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cxtxhmgx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kuzfoagg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rsxxsmtz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2suktucbd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nzvxsjqr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tueswfsp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxzjvanl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wuotbreh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2csgjucno.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2inqlnnmk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zzkayczh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qmzrvkyn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wgglebsf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2opvrwglg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mnbmjmxy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xafsviiz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ahcumnvt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bejagvat.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ligtiwqp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aizyrmio.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qkdlregm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wqeteuez.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xhsltabe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ptqnqkul.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hwjznecy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gwxjmsho.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qouiropi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cjemspgj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ewlxawjm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2csisxmpf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aspymuwk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wokjpvzq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zqukckca.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2auiflsbz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ovgdleio.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2iyytvben.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jqgunvem.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2spmjxtui.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xawezvon.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mnfgqhfd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dgjswckm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2houmndwo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hxjkeieq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cdhysmei.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2udmrryrd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bjwegbjj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2syiugwnx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zjhhxnbw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sdbhrxey.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dxniwczy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cpovffqu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fnpuvzit.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uksnfefg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vmryxsns.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pxxszkar.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2uhepvsfe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzgwyuhn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jcsshyky.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jryikwdn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bhiuhbty.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ilqtyeob.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ipfyupbc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eufcmsfk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dhqysoqc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lpnnwufg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rytkpigg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dtyxdujx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ayctmfqv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zhqzudgd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2bbawpbbk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lwtvzuff.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xohggssq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tikcqjqc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wzygbqfx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ppjxcaex.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pyvkbaoq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fmnfooya.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vxfhsodz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2znjqewpq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2emyvqbfl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhahpke.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2afsshjmo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ekvqrfzs.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yihxgpip.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zftwvslw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lytnnpat.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pqmmxeet.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2okaielsx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ehcdxpag.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jgltqknd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fditlyns.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2urvpqvrc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2oebmhivj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jtjgcmwl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pdfournr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmcktuqo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bijzkvxm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nxljdpia.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vfofnjdi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fpoaqxst.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kkdiaggr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2usmjhfjf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2emdajkug.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2djnqujaz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fagilfpr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cyxyeqrh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qzkgqcow.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cdmuctfh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2tclafkjs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vjtjzdgn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ickdewsj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qiocogza.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ozrbuegc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2stsqegaf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dmrrncie.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xkriyqac.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ccgqwjsu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2zvmyoyii.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rjwrsiye.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2amcetpzv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vwscajpw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaguvole.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qmcheoym.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgyzohql.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nimrnhwv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kiujipwm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lwsbwjai.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2elhfagmb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kmovpmkg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fndsgdba.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2popsixns.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nfbpwsff.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2edsfbkxn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ufpprjzk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zexwnvsv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vbjfosqr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2laynihao.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vxilbhjx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xpitigsd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nyosogxy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ptdfhkfi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dcrpmrej.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oykireiy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yxgyzjvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iudalrlq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vvmurtad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzlhgmoq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2poklyakx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ationpjp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bqcotxah.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wuqpkvbk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2liaftsun.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jjdivqck.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lersprdh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqlvzjqi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kthjpbbk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hzdbqiot.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2eoahudaw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2exenybnl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxboiwfh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwlucbhe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2maadkyna.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2aompvfvl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jzjqnujj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fywnuotm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pndtzdfr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zcggqhip.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rexhulyn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tikxvzqj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tzkpptrb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eqmlqkll.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fgkwcpli.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2agabwpap.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ywxwebua.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwscwnqn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dvjyxoxt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ambwlduy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lartufus.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fvstxyky.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzsidyp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ecaajuho.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nqqeywjh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ymprgyni.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2arwwxlar.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wzwcsebj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wujuhjbp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezkhiyon.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shxlywub.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mzkaqgar.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2thcqkdqs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhxvaapv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvomtbgs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgukmyva.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2suwaypnn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zgdaaqvz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxqxfbdg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpnmtrnm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dllumghr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjzjswyr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgqewnaf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ksiquxqw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vaiorfae.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jgkpnyfo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2obsrgizr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nfkgmzse.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cccxnqce.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dxneorqh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fslzzuuy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mrgvfszt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2lqhdmutx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fosqwgrd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lslajgdv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajisiezv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qdahtnrz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2syswsmrn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fqfamzgx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dkyvxpqn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gkuxvyka.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kgrrrayn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ncugkrlr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wecnsfdc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2msyxkpgg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mqpnkpiv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gattyptz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fafdkyxk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jdfruxvq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocfypkvb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ervmsxgy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bsyfusmv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykbcndsb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jnjljyki.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htyfyzqt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edfinjhs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cpapodfj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kzjvmikj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gppykikg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwglyfgh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xwqeyiji.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyflqrth.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2syrtnboe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzsjtlxh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udnnfpul.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tqevzxiz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2chdinxiu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kaiodynr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fidbozge.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zajtpeqw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2yeetxvcr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2izpytmaq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ylsclnom.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2atcagcfu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cwckbfdb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2odwzyhlz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gqgmoxxv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2eefdojmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjozeovq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ufjsgucv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljgvaueb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2khwljmdm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zaslbgud.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ymxaxywp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmolkisl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhmchbvd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzizmtyb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xjzuvhta.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dcungmvd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzozbano.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bkncjjfa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jbysqqcq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uelzygmp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rdvldywq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxqofeqx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoghgxuy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ltkxjnqz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ybmjaiqq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmitntsu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bightsuv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hucakrdk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qllqjiuk.html


<!-- 参考信息 -->