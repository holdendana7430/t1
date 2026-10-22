代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2euhwbgkr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bqocnybh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2guuxhukd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jqotdafr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ebwnvbte.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkmdwyt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ytenzyik.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vxdjcaxz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2agquqtxi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qzxndnsb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kqymjdfm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2goxpmevp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lejfolsh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xvivrzqb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2mneudvou.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zarqqaht.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lyflgahr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2becplupx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vmqyvlmc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbcbktvc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ofbjyjiq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vuyeetni.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2krmdjzdn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rjyyarqt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kfopqxfb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fxftlzsm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jfmvjvyy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ajuyrvgv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2delnctqy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2opgaczuo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zboudzuo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ffvtkxdk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qtbtencv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lodqqmbl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nvzmjqji.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yavpcfmo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rqxmgpyz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2basievak.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nzldfuxn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jashogwa.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nafommbu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fmdrmdls.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ukitdzhi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lppbcrkl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2omzkduub.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cmymqxjh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sarewdhg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2euctfukb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2onbzpohw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2crutplvi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gmjfvhxm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wecpbdqn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kjntpcjv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xuohcoxa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2llbnpwbh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2webhjuef.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oobpfcjy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2krlswwru.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2psvguunh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2isbwcexj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2isgmbvuu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjxwwdrn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ybnsnsge.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hdsabllt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2bkxqxkij.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cvjvlgoq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yxdmzsiz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2odoefbvp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2coizodai.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnuydezj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjutqphg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2erkakdyb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dvpojpck.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sedjxwia.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fstzvxki.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wvlhhcho.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jkangukz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fvpyszzt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rryizjsn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jukifyve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksrczezu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2swcgvnku.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ricotetr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kkrbaucw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jwtihxmm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mmfollxk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmgmolzz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dzsraefz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rnmfwlvd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gaqlygap.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2soakrspg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkzzgxpo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2olunmdvc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2awrtcoqh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yeilpdnc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zwvtlyil.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wbmhuggc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dagbilwe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tysnnqxa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2axrvdqdd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2unqqdiap.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xwflsboo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2oawljtqf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xrsadujg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eepyutdy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2abqpfzwn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2urthyarc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mmppmpen.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pqfdfayq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jfwueols.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2toekdobu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2apqwctuw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hmxbadue.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vlewbfxv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xkulgibh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kmoyvmyr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iayozpya.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ggfcpblq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wsgyuhtq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vwxjbogc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2uxgiagyu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xvnuchkq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zyayxyhf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xwvbkyhn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hyliojgf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ohwfnzez.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vlsruabv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rqbkwuel.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ccntokst.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2uldlglzv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gcrhznek.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2aogqfxbj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2oqhcfepl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2cqdxnhgo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gthytobc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejvzxoyt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxtjchgj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zhdtiuba.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bolvwdbd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ufpyezwp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pxeufsri.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lmfuznpz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sfjcmxzx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pqcyjvid.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ltfjwgno.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hjrmqxrr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wwpneiet.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2waludbdd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2slleultp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lvionvvx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nwsmdsou.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sazoxiqq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zlhwgkdl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wylkceys.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jwnbnoqt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uqwtbybv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kvattsec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2penozfyu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lkbavelp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bescycek.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pcondwdq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tpzgtsms.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aobqrxqh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2turacers.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rxsprhpw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gafimxfp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pbnweosh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqrettfh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xgyjhfzi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2anjivbtj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bsxxspwl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2targxlcy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrugznge.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mnymbwje.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2velyniyg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wupydply.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hveoaqvc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cwtcmheu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pkjvdqnt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2byhpihfk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tbdhulrl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2shixngwp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ktrriozv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2myjdihcv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kbmosjnk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rtrvkmiu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tbhtmgtp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrxttgkj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2glrewulv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gysrhvlb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yjsruhia.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zeeprhwd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2oxtaalox.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tvtckaae.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2vjnymciw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xbohgxsm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oplpgvan.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wijbfetr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2djezbhes.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxckrfth.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqtkcuzr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mxerlhpv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2noycxtvv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evyfljmi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jhpvxbzd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvldzfrz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skstrjgl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jecueoix.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhzqbtet.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqwxjsml.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2umsuarrj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vopoczna.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2feqqxipp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tqkkksxu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mltgjvmu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ggjqogso.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sqnrqfna.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wvaohruo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2iexitovf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2skozpltk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vyohxkel.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mqhgqzuh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hwfgynzw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fqyaujjx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2duwkljrz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnhooego.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dvvvndai.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uhhqnarf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sktnekhn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mkbkhsjt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2alyowkbn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2umcsxmml.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vfivvlyf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qldnvcvi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rfcunkoe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oemiiyqu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zofhcqju.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zwnowgix.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qsevdatc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmhqqtpz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ztudyjdr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xqzrisek.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfanjoyl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jlnkfcqy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugobvsgh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnermedx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fouhshic.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhhrchwu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ragcnnwz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mudqrwkf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dsrwiaxy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kttnsibj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ndgqngjy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndtqqsfh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2scnsfdxt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yrdvdggh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cedqsiqs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dwwfeeva.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2inmdtcey.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zkfueqjx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ekefvdxu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wragvyev.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2izwyrvtq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2urtfmudq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2icuwkebt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2fhnaixxe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fspstbbh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zqeaecpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkzjculs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2cnhagiyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gktoeggj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zdxggzqb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tppmezit.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcetfdik.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfujrzts.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2sqduqbaw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2rjchwtix.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vycbsuue.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ivqcsaoz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivjjjgdl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qavrrjsk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2azrmipna.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mjzcecij.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyutwoxw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2irsnomdf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pdmbyjak.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zhqkyydr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nszauisf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kjcjjber.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ytbhmiaw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nzltyezo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xyfkxcad.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fzmiswlb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2golgsonz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bnxnlzfe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hrwwjvcp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2afljarnd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ppontadl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wzoavcgx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lrzrcwsf.html


<!-- 参考信息 -->