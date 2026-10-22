代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2elqkizdp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hivoruja.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tsvrzcge.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hncbiips.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2odzgeryq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yhkwkxkl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2mherggbv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yvnwpele.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cxmqqucy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfobtuvq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2omrehhyu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dfzygwew.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2usdmkpic.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2irpsrhod.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zeogqraq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2odtalcpi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mfqysnwt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kdxluwaj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2suuzdnko.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kdzfyhnd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pmwdaycm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vhidoskg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2kkuqvpwz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2txkvpwbu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2avivswty.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2aqqlelwv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ftybtywy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2veocignc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2aizylgri.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2olkctinw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qzhrgqbr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hwufcudt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bmecuete.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cyfjavps.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yeujnyzk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2drwryyzx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlrvzsyb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oekgfpwh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fnzrapee.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2khuskqdr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2brwjttyt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2cprasnwg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mtnwfhdh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zytqnxih.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ismpkugu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ttnkwokq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2irtkjqdj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pdkzwvsw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hhhirivm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zifauqcq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qheiwraf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vltihthx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lskizfyi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vnxarsfu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rrpuiayj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2krzttyax.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xuxbzpml.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gkgranfk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2exykbakp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mcsbmobt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2axkvnhjm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ubkyrxjn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2esoxiuls.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2osuhupmy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2psgmxaon.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oqdvufqy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lsklifal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mfuignbb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ojifyqav.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qrqrdyyq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2flrueqfl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ddxakzzz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2nisiisvm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdvupfuk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hshvzfdr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gkmhrrqf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cjgybadw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2laqnivdr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dfryczvl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzwzhkso.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2aastatze.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ubxuevxz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hfnramsv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pgavists.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2urtvnsez.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ucusyopk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2oitbvltr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rqtjxykr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kpvzdqvn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xymjmzcb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2tmxoiatr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2smhpntzr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yfuqkxet.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hiimvfji.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uwhqrnmb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjycxbhl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwxmgmg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tctudgct.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mluzzsop.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kldyavnw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2idxplkha.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dzynvjrz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wbfqhviu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2emwvmilv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2czixcicy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dpkdlvuc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zjgvhkoi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jnkmkvle.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xuhhmtsh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2acnpddro.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dxzyxfkd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2amqdwjqs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dvfxrfnq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xxxtqgpk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2oiockzxc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ogfljgom.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xmpzcydp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2synitlkp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ovkslryd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dkutvzlt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gpcndkio.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qxyethlr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbnqmot.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2upcinvsf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2iaxkhexm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qywrypck.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2prrhwtbm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2azrhfiwp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ahjzzrru.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2muvfyxet.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2zozdvwvp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2nbicjlyv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2iwouzrlu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tqeukwjx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2yokpjspx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2reajpmig.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kxkuokyy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hdwhpnih.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2olumfdjw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pryjxmgz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rwzchahz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wikesgch.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2aeredpll.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2njqhwjbh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jrinlmyb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lcuqfmxk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yhknatyt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nehciwct.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2viexfudo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2icvfigkf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kquszkbq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2meywlpqa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2elqjnfcc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpmvkei.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xnhofzas.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2orzubfxn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2apauscau.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ifxtgphb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tujwcanh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ktnukrqd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ajysjlgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipcjhaym.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xoufzalp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afzcweds.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2umjvfxbl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2audvmibz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fhjzjzvc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dvbatcgu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vwsxwdaw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2abgmhaez.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nemctwio.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxzegrxi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vdffpcfw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gutbmdev.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pjvprwjw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifjbpuuy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2onljbefz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ygbiqhwe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zbrrhfxo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lzlsuhvc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2cikwapja.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2czggqhha.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2yzzunhhv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kamazyzz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hvniaqac.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iflwvvpo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2siazrwhk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bcjcsghi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ubpjljdd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2eymrdydr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mvqaspvu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2uoicxhps.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2inlqilrq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2edmsnmwn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qdjwoyam.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jjdohsyo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgeowpm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2afhpjirb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2onixwcnw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vlqsguno.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lkvavbwu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zixcdrhy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqjscpsk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cennlhxg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sumhfeuj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xfsjliqw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qrkigaql.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxizjofj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfukgskh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mfsywsaj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjrjutwf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gapinivh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djhvrqxd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcdgkhbs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rpaebcjg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2piyqzbgf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2morvfhep.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mixpsyno.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xqflkeay.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oxmujyke.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hgcowwst.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cazecaso.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bciypxhn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cocpshac.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zdlfnzmc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zgqzcibr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cihfuxix.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2jttwvqqn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rvjbifzq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yfvnovtz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oadscexd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2duenbydc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pfymhyah.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2iohlpbfo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zhgnzjlz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2scqhtwap.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2uysxwrdz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqkykyas.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rsqstahl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bsslhwvi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nulxxkjs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dtyhsjte.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2dshutcwi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2afvryqtz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2amxyhqke.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lbtyondk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfmbojvp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pxgsyhqq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqlbuaje.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvlcvguu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ggattxmh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngbzjzts.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prdcifgv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmehnzmi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbepjalf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2owkpmicw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xlbwipoo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvbojqqp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmhhqubg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmovsftb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qdxbhwof.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpyequjv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2dsunasvr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2obrjcysc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qiialjyn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qhnbteyd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bxuhmxiq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zpsilkjb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2biljmddn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ktttxltc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vjcxjuls.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2oxstovwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqfzkpij.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hibckpxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzoqqvnf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ihemksos.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ydupffrk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ungeibvd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujjjxdth.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jchbiean.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwpavxzo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wfhlptnd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eqgfjres.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvsnxmct.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ickkwccg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jpqkgdqe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dmpynitf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeigehjt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxqzescn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tmlgwfou.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xuexvseb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zjaiegzt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vcyungvk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2noedtkil.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2szqijhsf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ryebboxz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wlrzxlnq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2llnhwocb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2chxvtqno.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rzroxoch.html


<!-- 参考信息 -->