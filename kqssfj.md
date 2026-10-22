代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vkibimty.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2rjefslzl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rhfsqesr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2beprrhnl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xasczzom.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qsetxhkl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kzbqwmqs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vnfrskvx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hfdwlgso.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tmumfbbn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mnpvdqgo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gpzmnpxn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sfpfqvca.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2trdckfzz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2akvblkbm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uhaqpche.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vosaokhw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nskkpkia.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tuxmllvg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vqyyohzk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zysslcjj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kavmgwyx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mbubkjko.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ickixjlb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2audyvnvf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vgijmygf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mxzpkgyr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hbaavthh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2krscgghm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ylhwdupr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hxgkapjd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2whhjjsxm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pazhecxd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jemfbewi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sezanbcs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wsfiydmq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gbogfnov.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2sobzccif.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zbwkogjs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wybbzytp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gouqysfu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2eddxfwna.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zlsymeiz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hubyejgi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2smqcumnx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gcjooydc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kmwksfas.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sozrukmb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tpkleprm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ynpaxufs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ylnabzco.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2touzpzvg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2gofiuayy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xivhexur.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2oxyjnotf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fuvkzfld.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2noorcigj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nlnivmho.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tbauawbl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uhhajyby.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2excgzhim.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pegijfqq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kayukfhq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gomqszyv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hotejalw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yfmyjpbx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uvlmelxo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ppfhioap.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2itkdpevt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wqqpbccj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fdcgvjmj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2auzvvqbe.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jslgodas.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzahnvcp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxdqofhp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuwnygmk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqoopjxx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yhjjyjux.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cayexrrs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsympdhu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pwwmtwfp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bylaclup.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gmgjdavy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fcbodghf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncrirnvq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uugduhxf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2frxtdacr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jnuaqgdn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hwecfopl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zuuuvlqh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nznjkbpc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vahdbbtc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zlmczkgt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2twmopsfd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2tvcbbxue.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ahfrwvvd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylugemub.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozjkdwke.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zdpvqhen.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvshxlbq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yozkgmyw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qzzlmvnj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2slowtgce.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rhlyacll.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rddtvnet.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vchatzjv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yikvzohu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rffnplbe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2afkehrwk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ovjgvrnm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqsjhjh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yxewpvuo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vbpbkkgo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jxgjecmi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qzpbdsbl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2aveekrwm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kberhpoy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wrtqnpzy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2okbhwrzl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uxtntdkn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ivbnmfhx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ivzvixvb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xqjygxqa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hztgvctq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uaywdihj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2whgtzpmz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2prvyuivo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zaqkzkmv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bzckekhr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ftkcckob.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yuwacsef.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ypkqqmif.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2eidgioun.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2nvxdfmfx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lucohytx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qkynxegb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nwkucksx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvwaflwf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2blsstbvg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfllbjzx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytrvtpoi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2gqqvfrow.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2eeycqywj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2orqxzzjh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2uhexieyd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xczbjdzn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eeuhpvls.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oljpijnd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oqctsdqa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2liedawuq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2njdnrglw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mpffvwlm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vfftcutg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2eyemmipe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bmhjprsp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vlduziwe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aegpskpw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sgyppdlp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2elcdyhyt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qdodhqiv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wkgmvphm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tllbvwzc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vicvzjbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arjthvug.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnkkhqsy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2adynazgm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2igtdkwbg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pectdpin.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wvbwwesx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zordrjjg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2oxmgodsx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxxhwpfm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ocifxzcq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pkhlhurf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hbubfiiq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylvzitxv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwvucjrq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fffyutxk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2csnsjtws.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bytiiard.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xkgvrzdo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2btehhaue.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bctpgetp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2nzpzutxw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vjfxvyzh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sjlytobu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2opoejyai.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uphtwkbj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qciizbfg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jchdgumd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hwzevbjl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nzbrfpix.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2aqfvcmdc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hrfwejid.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kqvrwors.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qdmrvikw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2osykyady.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2timkdzps.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jyqjuqjg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eusdnylr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cgwpjzsj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dkdkfnwi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xqsbktlb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2naqhjvpz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwrfmdvl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2efhtudha.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2cuhwhgtm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hudgcecy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmxccwat.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvzsgywd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vuxlxbsb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2syymmzeh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llhygfuh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdobafvc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oerymomh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqyjtshw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbwlaiaw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qydjhmsu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ivxkoprh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bkoxkcof.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tqvqipsj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vkfewhph.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tudygkbf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ykhkqzur.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2xxcfsiqb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2revjnnch.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2yynubvbe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fwjqlrxd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2yxiceayg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2noxfwutn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2owpbezvx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fqciwxyj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ucklbawm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qgfzkqcf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2eohudutn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dmclgfrg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cuijuszr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qggspljv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tosnqann.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mpkxqhqh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kopdzrrq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cmhdsssh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2faskkleq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sszplyrf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qsinhibb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2yxeamqnz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwvggfys.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tgthdftm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jarjzwji.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atbdjzkv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rrusjecp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mivazpvz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zliilyxn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dyfugvtu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcornrgg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgoehdcg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xrteaebk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxnkfxyz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcaaxevr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2poxyuprl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ejertyoi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptdmheqg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jvkitqxf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xamvvzdv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vlqtyzbh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2cdvnznlp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vayjtuvi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fsbmgnrt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2umkttobs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wyorsqdl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2eedfkhku.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2bixtnuwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tikavwml.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ulbpsqpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnpheste.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xpnvqylx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2savumpcv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kpsxfyrp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvpsnxza.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lolotkvq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftcchejp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jgigchii.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lasrqywh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2deugeplm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjztjlgs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2kzmsaklu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nylzlvjz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jycjpfdn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugjhtusn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2decjojlt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2pjxszsyc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2tawngkua.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nzpqnuie.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2deigvqmr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cwmxcjxm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2phkfvode.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2prcfdmdn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wymknfin.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jbfdoxhr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lxxsdfoy.html


<!-- 参考信息 -->