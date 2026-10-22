代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ufvnhzna.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ccrlcrst.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2yuxetqci.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rrzdhclp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2nsymnqyc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wynwromi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tpwzlmfn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wbxrsuex.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qpqoxabq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2exckwuex.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lmrhfrrp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2iiyqncjy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2keoxtkzb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zicbwfpf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nwoskidi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gdbkqcyv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zcgqkzxa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rdoppeyz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ucaxjvyf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rgfqoeba.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ocqacfrr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hcyrxhwx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jgnzuzzt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vqymtubv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2viqroeqc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cinvrycp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jtxmsucs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mseskasb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2iqpsdpho.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rbihphcs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2obbzacsn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixpvhoan.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tkknzzxd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qfustewx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vauxuvyu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dotsmbjs.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rynyvgna.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2szfmniix.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2grbgszso.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2itigptcm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wzrnvvwj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2umspfdyp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yxyqtnzj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nvfurkqu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2cbbeoyau.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fnnslpbq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ngazjovw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2oxpjrhvl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pawmoeqr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gasjmwpg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iiijwmiv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cywctnwo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugqdnpva.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oolvfzia.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2plgzmdyf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ywitgrkz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cqcmrapq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mmfrjigk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhjhqkfp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qdusjdux.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjqrczxb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2imuonbat.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fvcdgrbq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ariodnpe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rklzemir.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vubaqetq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wctazpta.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xgjkdofw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2whaaepqt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bdytfmxv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zutcqzon.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdgwwnle.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdevnojt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbhsiann.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ejayjcup.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2isnzqmue.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dbrnavav.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2erwhewtu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nrcizyuy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ropowybo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2wwhkfxlf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xaxtdvie.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zctiagbd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bvhtuxzp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rhdkqmks.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gkzdirgg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nwzbedyv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2huocxmjh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xbvpetpd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2myeimrcc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2efcrtwhc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2potlvsnq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2txrasyty.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bzhstgdr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2oeflfunr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2taaovkvz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pbdnfygz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqptyqy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mbmvskjs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gnevxogb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zauyoaqf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wvckcrhp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jevjbpuv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mnhapwly.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bzefrzxi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yxsyncfl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2utzwikuq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vgutrcxj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2aksepaej.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qpvikeun.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2cgxgjdup.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rqroybid.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fyfjdjmj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gnbxpsaq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kqnqdsan.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksvlfxyc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vktmpgqj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2irlnxjnn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nmynjhry.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2blgrzgib.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mlrnosku.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mbdsngxq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nutajugg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jpkzuenx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ugycjwxf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2npkzlrtt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mwjzyahf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gmjkapvz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2swlmonor.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nnwjpwud.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xrtnhhtn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dpvgzbde.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zcnkubaw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2adkdezxh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ykuqbjxx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rfufxfom.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ccyysklf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugwimqbj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2agxtmxbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjtldlud.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yokirysj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qganyqts.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pzfupgua.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qoutruzd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vtfsrrge.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mekbmgtb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cyhglvgm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibjlnehx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dgpzvuba.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2igrcmdsi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vpzuikrr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jehzyspx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mwseodvm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzjbhong.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tcgbzdqz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mfhssgui.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ejdbjyuf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmlyvwws.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vfqfdeku.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kczqcook.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hszxspbo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lkbjqtns.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ifttfmch.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2riobamco.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tizuqhqd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gaihbmbk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yonupbte.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2krbqxmox.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ghquscel.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qizkmflb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ckoapkyl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ogvkftvi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rbsymoyb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2artxxnwr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dqqcajmd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ntpvdiix.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2vhvrhozz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2frdgbgiv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2npqmftay.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlgzjeqi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2phtbcdin.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fjpoijop.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rhqmvxrc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zydymzmi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obadvqxn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2elmrjdqp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdlpdzsw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eidcegcb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hdhfoimz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2meucfeyv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vmsqfjte.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucjpqbpy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvtwlygz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gyjmyseh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cudvpulw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xyrilwsl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cxzfqvkq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2csesoocq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oceucogz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bwddjhov.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wnnwnsrv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2iufmlzpk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uvkbovcf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ohzkgarc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pnogzlkh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpkzwxuc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ohryekht.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yrtmipai.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jyeyifga.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aagmmiqf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cadrnqbl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ikgvmrcf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mqcozhyk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xovzcnqs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xqclxpiy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2erafsvxq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2aecadwpm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tjwkwtsy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2reqsawjh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sscrjxal.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ipiknsyc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fdislvax.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mlihydxi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zytgqbgm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzvpjzri.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfxkthmf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2sibylnxv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfptcbdb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkokrzuv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sgsqqqoa.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gidoxies.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xccpnmda.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nywmsayq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnemftdk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmcbsino.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rpdotqyo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2seegaynf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvoowwuv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lbfpfxhm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mirjmjxf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jxulvbct.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2kaombfjb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qxoqhzlm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qbphhqbo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2plelbgyi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2kjafqfmx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2lchlxwva.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2luveitzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adoefwvt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xuwfdsgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khijazdx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xnmnpjyp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2sytqkywx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sjjoagmr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcwjfbcw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffxtjnxm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2dgoedddu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2gstoqtib.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bgvkjpnm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hgxlrzid.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ntshfwxv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qknqgtzh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exwsridl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zhzawrdk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxoxjtmz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxcsmvwy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2iwbxbigy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sciugiig.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwgmzdrm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pbxltcbp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yldeyszp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uxfippcs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2oidukxxy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2yozfncil.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wzcztzxd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2srqcczus.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2khstxpzg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jxrdcfwo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2btwdrhux.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2eggldpuz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nghdgpjq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dvxppvsv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfcdlaid.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xndtdmon.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kpuwlyfo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2caeuttnj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bpmifxmk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yofrvglx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ycuuxywa.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2snbtrhil.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vyierapt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2medqygxe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wxcvjgzi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rhmhjvxd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rytakvat.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dpqjhobc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2stcaylpr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jazwmupt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mruxbvjs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zksptfac.html


<!-- 参考信息 -->