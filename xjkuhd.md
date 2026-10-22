代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zouonqep.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2qbibhkak.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lfmnslve.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zubuiosi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fgvhjvxi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zfivfinx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2afamjpyq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rqtqjrxf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pizettrg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2avoqvtzc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hxmohcud.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2skdpaumn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tyanjbzg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tksxaebg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2krdglfrj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gkiukpjd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ammyksrs.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bcmzskyr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2blbxvjdx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xhqqcgrk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dintiqmm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2eyzzvtqf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xdqqstsj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2skpcspny.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2orweaomb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2xtaztumv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yocfgfeh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ojwsimqn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hwjbhdvj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dodqqlna.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pvcarlbg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vrhgtpqx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qgmomelj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kkwhearr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oaotdzkt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rbdqsiyr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2olkysubf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hwgqpzkv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ovzjzwtf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ttcvpukj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uottgvoe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uuzlitcb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uadyiqym.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ebtfbfrd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ifkungpr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aqluqtex.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mmehxbsi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2parvimfn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2abmkavto.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ekwgubjt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bdaekdtn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kdvenasi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kqckkrnq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cckkuvew.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rfmjryaa.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2shcrugqm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jmlcmdqy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bdsivcpz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sqnattuu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jbnwshlb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hjuwwmto.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uekxtkex.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pmpxxmtn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2urxhbygq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rpprwrix.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rhcwnqnp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wnfrmkeo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2uplwalfa.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2piwarkox.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2turozrsm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fjiavfcu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qertchvb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2djjeyicq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tqxiclmw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciexuczq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpehxmcj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2krtrpunm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ncyvejky.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2malirbup.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejetqyjt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hzxdscer.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2bxlgyhpf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wfkupqyk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gvkyokoo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wklabttz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2guxuzgdc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2yihlxgow.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2glvrhlpc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cohfbgsc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gidziwdo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2giftjycn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2stwxectj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pxginzrv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bdjnbmvk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2selwnedx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbqnpxvg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtkquyuo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mywirqug.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nwyzuhmd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2uqqgjyyw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lssvsvol.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zmtxbycf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iwvnpukn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kssfczlo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bpugoldu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lnzellfx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2acmwizrb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lnwuzxen.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2sjajoxhf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wyxghpqm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ergitaaz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dczdgpui.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2veielnbf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fqvfuhfs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nrwakppi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zpzpnbha.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yclcnepp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2yoadpzeq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vhdoelfi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xvprzgun.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2regripmx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kjmgwbyr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2necuixqf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vnoypqni.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtsogvfq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vuylxmaa.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2aqwuhogo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lfhuyjpp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbnoixid.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pszxmmip.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vyicgyxn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2maqrcobs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bqedrjry.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ahsrndhg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2efifsubx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ubtzajvl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pxanwbfy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ttkjmlxf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dsuyugut.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbgjcnqq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjqhihyh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wwxrnzmi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdewdgsn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2adahokfu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yaitdkpu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2letjlqax.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nmjmmjsr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jspnpgbd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fbxjqqoz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2koyhlxni.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xgipyadh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2apvetkxg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mjlakuvo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppaqsjep.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2znmlnrth.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ffbhhvjp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dvthohnn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2naunpeda.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mmcoyiib.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2geuqtbla.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cblckure.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyckmctj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rfbxxayr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhxaakdu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2uivfwwmx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ydlpzemn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avakrscv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ujyknceb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uicievgg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tmbpqpxu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gdvhlikh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wuoxrmas.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tsfoozdb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2egltnenh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2vqouibbo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2copfesqz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2khhgfiym.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwgjbmtp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jhkukher.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vnfxygao.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2uzoivvze.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvtwkiv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fjoyzedn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dnambzqz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gzjufvtk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xftzgdzt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uqaphfrl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2wrhaafdq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2npavhvgp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2oxqozeiq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2btjybedc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xcsflqiv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2egyoowci.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2umixavjn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eahbsdmz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uwqlykan.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2agmvlqny.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fjhtfifs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmyvvqgb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dmrxydub.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2iniykrxj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rfsfyafi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rmppjfkf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djpmoifi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhwxbfgj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vyfndwtm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2twmmqsty.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kimlombq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zvcznduh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2epzifonl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqukjfol.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zbojiwkc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2goqozecy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jeqfplfx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2szeynrgk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gaxgepys.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmbzwqvl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nbkaucpb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pdnaohog.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2unmjcusp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qpagsbsr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2adlzslfl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bllwzfgl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vqpvtwrk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2tjivhzrv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lmfqtrfw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lbiapzto.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ydiocdlm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2envqpunc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2flsrryta.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zpmynwyf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2akpoxqaq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bmxkdqvl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2chytfdyb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nausbuhy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2njwecfcn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hkghbgox.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yofljvjb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fkdvanke.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qiywteis.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pdemuipj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ygjvaebr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xtmggzhl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flvhchdw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2cgtmoquf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ikjqtvkp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxsthpdh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ctmannac.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uttktmoe.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bfenzvij.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2yqaztlvj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oomshvii.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxdldvch.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zifrrrmc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rwubxbiq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqxdmrjt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lccaemec.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iaayhgjp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2unstwsru.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cxvtunrq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2abveakzk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wpfmujrj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pbkeldyn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2myxknmxg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rovohgyd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wwyfcedn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xvizvygy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xmwzueae.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qpsnsvum.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dagbmuch.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uqwkrsif.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mxnlndzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcdjcuek.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2sondiwuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uctdrnod.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nbzgfxoh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yvudnllr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfwqvrno.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkxzmoam.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2skhjxhcz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qhlumfup.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qvaqdgei.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kbshtzka.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2smnfdzre.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbqrjblq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2axgjlkiv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frvcudme.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ynrqcmle.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihatcbei.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qszfyaki.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2slbgxrhx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zewcwesu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2znfasdzj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2drpbatcb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xtohlili.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xpyvndmm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ineopvih.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bbzahlmo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2svpuxjse.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2mmksiivd.html


<!-- 参考信息 -->