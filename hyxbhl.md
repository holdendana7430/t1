代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jxxjuhyi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vvzzyozt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2midaxhmb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ulnkckej.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2stfxyuzu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwfbdnbf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bivdojgp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hntiwdnd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vaxtpynm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dekdkfys.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dqihukdv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2irgxlddw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2slssyiby.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dldosvwd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ixscolzp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jpsqmtif.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rutpborp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tcnvbkch.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2abmwrmvb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktialrya.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vbdrdstv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nytxhodj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nvkrlzri.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bxkefsjp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dmojvzcy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dhbxcgnu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xmmjyxfw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mnsqmuqg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sxcdcigs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hoqrbgfj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vprthmel.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vrojsspj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2trwzlyal.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2drpfgvpv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rbbcqkdr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ofnavvhd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wnbgfubx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2joiiimhx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2epziayni.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xuornmvc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kipewpus.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gdehmwqb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pfpsutqv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2plnxpwzw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jzwheykm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2atquxsel.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bblawdqv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ythpqllx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2twwexnxa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tpkmhjyf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ulwjmdla.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2awqsydji.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wmklfeyu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cadeorlm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ugjiefha.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qmegeaqs.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hnjepahn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kfqslvyt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zxvvztps.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nzpghsmt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vnoqrvpi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbhianoq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xshzahgh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2pmulcxfj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tlurahor.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vybadphs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lprlbjqe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ycaajfxf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hnwxjaze.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qyffhgfw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbjqevqw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ceomaehe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2keggqdbt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rnqlwnmq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tdehtwpk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuulobjs.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jyzuxgpf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jbeyyknv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rpoaszaw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2yobjgzxl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xquzhoba.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hhevnnum.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qlaalfgi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kdtdirpw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dldscgdu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vxcvdycp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hanbscja.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2frrmfpnt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wivrmtiw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lqhrqfmp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2blxrzcnh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jfjebiqw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2edgfczbp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ifwcxwbr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gdnawwfg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vztiedci.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dkovzbae.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vxtzilki.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kbaiudpj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2thfsowui.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jnzsbnhi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ogaeizxv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ygtwdxuu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2irpxzwfj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2agldkbqc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kzzyfcil.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzxrjtwu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eopmmqwe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tojnnddk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qkbzntih.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dbeunuhb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kjztmkgk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xpoiqgfw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2xkbpxlvl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2bvkbrbmq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vuihybqd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cgesndlo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2llnlqudc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wlorhrah.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nbpuyins.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zcluwnyq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2cjtbggvx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2recwadez.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xudatwuh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pxokgwxs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdwokqb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2naysiwtz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2shsebcmc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2unszurzd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gaugrmml.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vrlaxbwq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uoadisav.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xkxlrret.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nstjtwak.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkyvxckh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2inztbdmm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2emupfabx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mcbdtigm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2zaiooxsa.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2pmihhgmk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2soavujuk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hhjpcnek.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2elkdmajh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2crpzpaua.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pnzhgryw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ywsplovk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ulmqzptu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dswllgam.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zkfovntq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnbqwrwy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cryxzbfl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hnpsuvcj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bjcrutas.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qminoycd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2beznyehl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dsyjodap.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2aueibvqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfcvnikc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tgwtlblw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emtrucbr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mytgyrbs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tokttnaa.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jhaehkqo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bvwhwpzv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bxihqgnn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ouqingxr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gagflouo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npntxmtm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jxghspse.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2furgyjyl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2alzofdkq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2owjyjwww.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2igvlfuwc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcjskvof.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lydakivz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtxtcum.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2evfoprfm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vfuddoby.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2yxqywfia.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2isgfkcdd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ccocxgka.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vovaclvo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tkvjiivf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2wrdrxoja.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2azhpbuqm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xumyssto.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uiiwruiq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ineiqlzn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nzqlhowb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mihendxd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2peofelys.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jkjudadd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zrtmpang.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qtabdrry.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2siikedhp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xkajnnmz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kxmqoxfo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xnztzjys.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eshpoccj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdphhrta.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gggjmifp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ehpgnpna.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wqqxgusn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyzfpdkx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhadivbo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2drssaohx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qfjtlcpz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2longlbea.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khhpphhf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwnvzvzd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hnxommks.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnykdicb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lopmhmbc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jklghwec.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tacjehpd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pvzizsxg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2rhahexvj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tftaxxmn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mbranrgb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2maazvctm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ranygsmn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wmhcnlwr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lvbmrkxn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gyltjobh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gxillron.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2oauijkxr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cxtnirqc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ebbkfpho.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vuujoihu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cfmgsjhk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qsdkhidb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sarksqvu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2flrttqnc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ybakjkbe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pxqpcuiv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bcpgsioz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2beblamhi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2egolqpxq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2morsgjoa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzxundcb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bpytmgkf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2suvfesss.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vreqwpje.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ibisjtbg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2begxkavq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jjlwppta.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2xnrnvnpg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nsajrwan.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wghozmsh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kitelykl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gxumhsxa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcvbiuau.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2mvosanpz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkfadoct.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcdzzoza.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uvrcexxt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wtcpldpm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skxjbams.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2sorpqqyj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mjkrpfjc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pknrawfo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bwzaztba.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ezxoxqfd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2inqlntwi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eglfjjlo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2adiwytph.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2purpgcjz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2etsbkhpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewtnjolg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2onlfrozd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjyawqcy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ecayxtdq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ojskfhol.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjpdyyup.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2smmlssog.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmvlvlgu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wwlwxnco.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2olgicgxt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2djlzvblz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uksywdxr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2netxyzwk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2uofdthvm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxkvkepf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jkyaybvf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzdolvsp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ctqvzhij.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vdebnnhh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xupcvaxq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2roiojflz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kructldz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dmckmcej.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2elmtjzxd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2baeplfcb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2scrtnjgl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ivfjzufa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2bgmpgeqz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fjyzuhux.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ypenqjgw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2cfjmplqs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gqcdrifm.html


<!-- 参考信息 -->