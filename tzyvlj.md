代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tqlcntov.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3oddwhjou.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3uimwsxkb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3kfbjojqk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vfcajmrq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zfuzqxvm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lhlpmrcq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3derndrtx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wxcrjxmv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jabgurwr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dfkbywzh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3soechkis.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vrmupwuo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ljozwmpk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bcanbxmb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pkzskmiz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xajdspdd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3frvhgwdb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3sthhsadc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kjugzbma.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3sznkgmui.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rywybrfi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tlihzvmd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3umlyzfnv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nseimnlr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uyxlugfx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sokydroj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ttcowojy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dfghnook.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tquhhegk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kdyyoinj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ebpxoypr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ocfvgdyj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lkaztrba.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xejsbvrd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jzoethyc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qzicnvub.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yrwqdfqq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mftrumxm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3svmisspi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3slbtaiel.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3beuhvyha.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsbvktfz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fkxezixo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zfqxocui.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cjpbehiz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lefwijhp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vruvfjni.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3onrawszn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgncvewd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwwlewqk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iezxyimn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwjagefs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ibbwhqib.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tvizooyu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zeifujgc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zwazlulj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vwhuntjp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iibkawoc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3yaeiqxmc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhsbhhvl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oibaxxhq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3kgzqnzdp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yitbjmky.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iwzgvfaf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3iyagwzue.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrvpkiz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mjmgfdgx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3awxerngx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lspopjhu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kbpghbis.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thgvhzrj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3uexspird.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zkwkhbps.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3iqcspksp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3aqhpxepj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3bddlpquk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3huzwtvic.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3klibyegl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3eumxgwge.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ihdfrhat.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hvefhkgz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wlzaksrt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3fhtgjxki.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3oalconwp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lqdugdhs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dcciwqkf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zggfsdsp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3qcagplvl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kdistkok.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3enshvwog.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gwmtbouf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wqgdcego.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3trfwypmv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3sdicjkzh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rsltrmdz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fftwdjhx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pmzamqux.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uwtjmhme.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mazrthxe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oekjgxre.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ftmhoknu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3lubtwmmv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lszbbeui.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nskuedhd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tbkxxeaz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdamxwau.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iaqzzjjo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3waokeafb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xkcxtuvj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3exmruxpt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3iqjnwind.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3vvctiurc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvfsvedj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqeposdl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qjxzlocn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3esvrskpt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sdphjeqz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uapujqzv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3zjzvawsy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3prtrxkdb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nckpwggi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vujcxgim.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qrulccdp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xgezbans.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mgpkdacp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ynlyqqzu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uoyexasu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jsjfatzj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xscoiobb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bxbjuhrb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jifwcgbo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vlbrlgkr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3brisufnj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kfokqgxh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hvzgnplw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kqucqtwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjjzgnxo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jhyuuprs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzxmfdil.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzmcvijb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ttjmjzvm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tkcpxyft.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pbpvhwyv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mnvyljmg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mqbvqilu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xgzjnkhc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjcqdums.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lzgzxqln.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3tnophnic.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jvdzrcgl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hedwmzvl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oarmdxgi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hsetvewn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qlidswco.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zrrhcusq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3iagwgrwg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bteymetv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dlrihctx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bzinfpya.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hltqpugb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3weobbbpv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3shrhgvkg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gglblgah.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gpjkmmsd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tdfdyuca.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3awssxxyw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfoqqpek.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dpsvsuta.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uxynglve.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xjgngznm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vdbecluo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dxiseffu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eeolwrnc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3iaxyqdmw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3tqyaeppm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3omrmugye.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xxeeorre.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nlfmwcbp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxuxqive.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kacuezpn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wyhspssm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3iasujynx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dainjboo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgbgpsvk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3njuuddnj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgvvcbyu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cnlutmcm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrizczbm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bywgbuaj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tguldbwi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctlnwmjo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pirruwss.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pxtonhsg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tdkeownt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ogtycgxy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3typbgead.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rkkeuhxg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yiasxtbp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ugiwtuwh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ambpeznv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rqxxqqjp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hspyneno.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cyhdglji.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jkbbkczn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fiowpjpt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hcvxjotu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tchrjkrn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vlbgjyio.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3foplpycw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qiplkqmc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qbxzzzjk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3thjxlnme.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cipaauav.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gjndmuhd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zptjnyep.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zvjffblt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pyazmtkb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kztknmaz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cahqqrly.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zgspguxj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3oyabeflf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bcexzzkn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3puhapmlo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwoovrwa.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swftfdjr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xcelcliv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3immkhxnv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctbhnzwx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ompgghwa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dbouthwy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njjdfrpw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ghqlwogb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3shcpizcd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfjsftmm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mxnvwtjb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3apitanuv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktcsuikj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hxdwyxgy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3yjacausj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ontfsqzw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lwkbiqmm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3buccyoqv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lwqlowck.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ficvlfib.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tuvruuli.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3iacbgchd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wxioqvae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkwsjxbw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3evkpsovu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxsrxqik.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kztmdbyp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3yfpyvrcw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jpmhxqsa.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmfbkvbm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zspvwozt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xnvgbpxu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3olsstwuk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gvjvvqsr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3slsqvkoa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uhrkqglg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hafoxotf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iegylmhe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tznznfkn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3maiwgzku.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fllcuybs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tocwpeha.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3btduxkal.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zpgdsdbz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kxrynzch.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zkwxeblt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ojmnbbhe.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jdojlgji.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wxshjsyf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3kywgaxpw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vbcepxxk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cyzuvhjq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dnmdyopj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3nuacntuo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3aygenopy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgsvykyo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrbhhmog.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gsvswcpd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ftxwbfwa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vlfslvvg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dnvxzycs.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wrmlwzvd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3njykppjf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3juajdkmp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3diessuax.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnflayon.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3axqyglnn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqxbxjcn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dgzmzhct.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zosgrrtw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hicnkpra.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ggrqgtel.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3veepxcxw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tvamngzi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnvnybmf.html


<!-- 参考信息 -->