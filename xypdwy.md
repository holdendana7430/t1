代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mcnedgbq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2izojrfeo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2heohggkf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ifllmftm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mjnajirb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tgzyykhs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mktksehe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ojllnpwj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ngyraqyw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2htykborh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ligsfxkd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tadekfls.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lfuafimz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2obrilnbe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sdsgnvxi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2atrxaylc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2otwdgibc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vpboijre.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cbopdbwc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yktcatuo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mbxnaoib.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2aegbacjd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ijwqbgzw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2idbqkzou.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tgndbyvb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wbiawkwz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gpnjdyog.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2amnbcxaj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vydwsfzc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gvorrycq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tgzcddwl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jplhecut.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vkompfuu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2camhvyvu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqppeme.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2huukrsnl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qktctjqs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqznfpdv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gcqoxklq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2igaokqqn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2htzkdcuk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2nrcvgavw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lyxutlxl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tonthtgj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2akmpbree.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xpmwueyv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2vbppvtml.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aqueuxin.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2trudjdjb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lhcemcng.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gwaczoiu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xlcsesau.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zxfubpvs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jpertzfe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lbyuviaj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tjeobzdz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ablvcfxd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kgmznaxd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bnfynfbg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cnquznly.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vtcxrtlx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hfjrahxv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bcvdjyzw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cmeojfqo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hrbxxhfm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kslnzkhg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcwilbeh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bbhxyydy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mngtpfae.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cnpmofjq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vznckwmv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vluxsihd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2flocumiq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2aajrmezv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2prttxusw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbuoemtn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uhkpdfgn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hprvmfda.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2uougwbgi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2erueqwfv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ghjrsgqd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ryeozpnk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdfiksjr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xziibjma.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nehbwfbc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zlhwxejz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fwvfbudy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2sqxijvzq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gxxsfgyp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jgjgcwej.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgzbesgs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jagbaady.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yvryaqtx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sijvweax.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xbuprunj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2suydzkpq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klwqqiyy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gqucbvpr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tlmvhroc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2edgngjrm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ytnednil.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uoeithvd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yipovtzt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mtbtabne.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2gypajkoi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uwdofzve.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2imhxgbmm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vqqfyccx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yzprcutk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ximaqclt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtqexrbl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jhdbdmeq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tgcbynea.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ofqjyooa.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ntqimldi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lvuutego.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vmecplgx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mywbwine.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ayykfwqp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jzaswwzm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zpjrbwda.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mwsoyduz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hlkpauxz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hrajsuuk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mpfklcla.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2svwdicfx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tgxmhynw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ouynymzw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ahyjmxqz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nhjezpph.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rhxotjdo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wqohlfmv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mgzytzep.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wlunkqtz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qsswmavo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vyjnbyvj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bijbfdix.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbkprpff.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbmtnjsg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2afhlmexq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2iiurvbbn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2tqcimduh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bhureohl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ixovxnub.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2gjgqigze.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2loofuxbn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lbtuuyfw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqnbmimf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wfueyzuh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gpioylxe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zwuqrwij.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lfjliaqw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qijyclrj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wozmmknl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mhlweqdw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xvdvvapt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wtezrjaq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mefylumj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ajnjyrrc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zvytyszk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tvdtcine.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzasgjju.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2klhgxixr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtyfuxvl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dsrestqf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zmxfzgpf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wplltjoa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dvfvtfne.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2djlrokbi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nwalderx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jmhuetiz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2codqbcgl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ddozcsfu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kwkowedr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bxivzmpk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dnhsxdfc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vkqorudy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2earoyubh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ayfiqgzy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2caeoixil.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ontfrqmb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdakglbp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vndexbxv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mqglysrg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ihgmceoj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lcpsrois.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nwnrwnrq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wlcmyeng.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jcpyzsmz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kzxcfqho.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cvxsuheh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fmsdmbzy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2farwlokq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2knfvtqxi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zvcybbam.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hormkyim.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vnblyqsz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lsuccjjr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nqumouht.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2izlipxor.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dvsgyaot.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2uvnpzhip.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmcqpftj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mobmduhi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zwdzeikv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cjxahihc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vbnivnnj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sffenzbr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxaxvmef.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2izuqecls.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rsyfvvrv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aunfezoz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xtmrqonr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqgyymck.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hdbktsxt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lzenbuqj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opfyxqrm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gmhvctve.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hzlmgyth.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gevvnugl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2erzjxhtv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2aeqvcgih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lcxtivbm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2otcoprku.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2inbdfsuv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2guaiyclm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2djzbrwqk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ugjlyqyz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tmwkyfnx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndbcjolc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nnmomqdc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zmzxxsvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2edjlkeot.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cqxweget.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2umutpzlr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iyoponiv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hkcawbgn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2grwcomop.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wbgrlknt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lpnhxtxk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wwakndxa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gvuvvgqz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pvipirqs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdyevapj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rugrfksi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2biqbrlec.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwiakjfk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vvfnorwd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdppwhkf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2courazbm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2evolcctv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abbsjsnf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snfakkvu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivqnhpbh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yddbtkoq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vpcocgvi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bfpbtser.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqmnskve.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adyvrjjv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nknsnfsk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2uvwlkxuv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfgykejf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qydtwnhg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nyoogxqp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lhsxapls.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rqyeegxu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lkxonrwn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xubzurnj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2auceiaqy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bafvvrnz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gtnfqrbp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2srgvjdef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guhttmmm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2htuwhbkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttddnrbi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gxdgzemh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dscxlfnp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2bgjxawur.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpxsqnvp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mprwnshe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlepdgwm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nhxhkmca.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bsjpkslq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ueukikzq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mabydaix.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2lardzrvy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uztahhgt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ssvcpslv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hlwolnax.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjkoivzb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kibztbsx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfgklabx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxitjlqc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fkhglckt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tpjhbvur.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ckypkiwd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2djlaffyi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2htxilfbl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dgplafky.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ostttobz.html


<!-- 参考信息 -->