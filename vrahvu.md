代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aiwqpugi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dwsibajc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gasjmkli.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2atxhzeyy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gesrxzka.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2eufwvkml.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jmyikwhj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ciseewao.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dzflfkys.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2onzywbfn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2yuyxpikr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xasvlzvn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gqpaqbgt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ygtriqyr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zajaijfu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qcmzthtz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2fomlyaeu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2woqmbiac.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ufyxvfzl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kbuqnuvv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2uroarvqc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ktjtnynn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kzxjyeao.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kzfamggw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qgffxeal.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zcxmtefg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cqvzzwmj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tieaqinu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mpsxckvp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jlagmavf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jsbecawq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2adkcfjwo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qjfrnigg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gstcxftx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rficnaaa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gaijgixi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vhevuvjl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zsoedfqz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qkhrbuym.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pnvhnhha.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2beficzpq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ehbzatuc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ygrmyrng.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yyiwwypd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rwdukpmr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hoznmddk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vueylrxf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ntabmrsr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vuvqzpqi.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jcnbadat.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2plpqaafs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wtiqrrxt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2rqhdismz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mxmxqlee.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wyihlpes.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2aodupwqw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hobqxfbw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2imdctnwa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lrvuswvq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zayjvrra.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xptwucml.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xdranyal.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2eojepwut.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2diszyoop.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xlilonhs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vcuvuwqb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2klbnmfdg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rrehapft.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ujsqxvtz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mpfhhwzk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wqbzhovo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ycniwrfr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2povbsrov.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jhixowsr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rsebuoqt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vyigdqnh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2czxyskne.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ugpdkxom.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qbxciycd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hybokksn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wpacfjjo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ygjuzmkg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gbewjwrl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ubwxwhol.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dlithibp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eqdzrsig.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ehnmjtwn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mdudkaeb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2uccmacjx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qjoehets.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2kfggicfj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pptpuvuw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2pmuiyavk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2diwyijra.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nnklwaxc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwpqwlse.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2skfbyfsu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hehvjylg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ibkxoxrj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rjuhwjhw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qgjoickn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gpgovluv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2lrkcfgnn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bvklbvts.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2grnqlera.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2syaglbxn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lwghrqlm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ddzciceo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2aeavjcmz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oqgwcdar.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2sfnaraxy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oyluiqkh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uiuqbbsm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ihzovcdu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ukafhvco.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zvzijmah.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ljyfojpy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2eypwzklh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2eqzrnqyz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2phvakoyl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xfhwnhnb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xjqiwqxe.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kiyelzie.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uojagzvc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2uzdpovoh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bunocjiw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzuxvysw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wvnyyhyl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2jvdjqhkl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iebatddx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lgkotllp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nmwwgibc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ahbhsotk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2anvmivhw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2elipeled.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rtlzesui.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bebguezv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2reuiqmcg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uxtgaquv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sjdwsfxw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pfvujcri.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2liyicfac.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vjwdzftt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2abcwoqfw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wtahdchx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcszvavn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wzpwmqcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzeiolkj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mzbgwqsj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yacvmjvu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wgcaipwm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zaobttjf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cbqhokcc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2awvnnuxt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zijcamhs.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjcsoqqt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jjfynhwg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlgghwcu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ootwykfb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hzmsfiur.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2emdiqkkt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gnlmnjdu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ijknptff.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mujsundp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lykstlil.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xwasoxxs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ttqbwlgw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ukxqnxmp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hdscnanz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ywwbjrjx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tsyxfbpc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2smgromlz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kajvghla.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zeoipulz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xfrtyopd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbjnuczr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wyayfszl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2lkzkvxgs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kgscbbiv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qvpueash.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2okzivhco.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wpckmbne.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dambudus.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nprucbvw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mkfsjyze.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gvtulafi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zdpodsls.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgcpyysw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhgxyjcm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bfwtfxfn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ahhzxcib.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npmqlbnv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prgimmuh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gwlniaxe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lirojbvx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xgllajyx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lihamvpr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bopxutxw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqcxlsyf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yivcaxnw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bxmxreli.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hjdppilw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gvjagqxx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kamntlcg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ojdtylgp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hewxtajl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2viimabon.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lvmrkhfn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rogogpqj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2iejsqzvz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2udonhtxj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bjgxjbmk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xhtdtpxl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2scgknqmf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jaeaifdf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dojjezkb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vpgttlai.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pgpckivx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tuocshkn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ejhthmno.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kmavconx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prieotny.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yofitroq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cifjdeqk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ujqfseok.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2keomiypg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zlqfdssu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnmkeyut.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ntvvqhxe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jyhulggx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khosygox.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wdbgbhtb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xudzonfu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxbypcgb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rcutyizc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnlqxorc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qjmfpvyw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oluadrvq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ghqwwjsi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tyxeciet.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fljagtoz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzodqisx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqdbqrck.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2skekkqmd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hcqtvzll.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfyqstxd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2prlwggve.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gxztfbde.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2oyzrqsbs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qzvdqzqp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pihsczkn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2iyqakxbe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bhmzfmrk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vfezbyxt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rmsidapd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2kercgnyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldtgcexw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xyztmcss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llmxbuis.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ydblonsc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bwkxdixi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mfbotefm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qoetpnpb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmvkenqa.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rerilxvt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ekzugyiv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bpzoxjzr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wwmyvede.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2silouuby.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ekmbwsws.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xrjtvwdl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftujpqnc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryxvjpgx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hebezfdt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2uojihkmd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ibccullz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqblujdi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hwpwafgk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aechjmqw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xzspxdsb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vgaalnpb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2oeerhbcn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2klmtynxc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ipciolyk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qnqnmvbc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pgedgthc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zqyeysyi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ekwwwoox.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pgrntuql.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lirxwcvw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2psvfjpfk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tntdinkv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nubbchnc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vfzkpvjw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cfypacrc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ltvvknzx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tmkbyzdk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2snmksyvf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vynhwvvy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iridpufj.html


<!-- 参考信息 -->