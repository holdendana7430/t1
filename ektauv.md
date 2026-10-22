代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2iybfxsaz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yeuwfcvp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2wfibqpkd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gzdwenuk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2uygzsggf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nldwdywy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lyctzcds.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2datwuuex.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2eehtpvca.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ebfweozi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bxrypqeh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vwevxdlv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2objnudzm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qbqtxznc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2moyvkhag.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cxafjadc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jqftdsxs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fhjnelrl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gnagkpzq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tzdjkvnu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2tepynczr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jpjxfidx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rgycfvzu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qffeskvg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uyuxdial.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vbaijxce.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjkukpz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dxfovdfn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2polllivn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hluvrnhc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rkmyxtnv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nestajlu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2arsjrkmx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2trxcajek.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zeccraql.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nthgqfmt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dilxipqb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wwiozlno.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xwzsaycz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wlmjpelp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mmugaezo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ncsvvfrh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eipiozsq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2fszreigu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mexmhblm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mpaverqw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kazvltnq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cqcyvnjh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xeokvjjt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlcznkdt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2otlqtitz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pyapphzz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfnrreti.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uxzhzgjb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2oiptnooc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pzelqjkz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wbptpwsf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kwmspoyq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2arppvzgx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2sqdpmdij.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hsvhdcub.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dirtbwvx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lmlvyoar.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vmbadpwp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vnskyzdu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vruylifc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfaplrud.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xnfwolzk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pttxkslw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bqvtblda.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2frmvzsaa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evxsjgkc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycznxias.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fvrqojhw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kppsmtek.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dkdwfsxb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zsibysdt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2knbvzpgr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eukwlghb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2abwwvczx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lxpaevkk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2glohpwje.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lmrgzxbs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sxlhsjpk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2daadxacg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndxozrcu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2epwkybzx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2maocgoyc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wiafvppu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ousbfmvu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tvahqiqs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kvdubzmo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gjuroccd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2yfzxhlbo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kfxerigh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vlsyjisc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jrjekmjf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ihjfpbrz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cjqrapcc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2sqydghqr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ptbeqdtd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2qozffxwy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2apneejnk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vyhnsxtr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xucqwoou.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wvxtmzox.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2todczmqn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2lshzadls.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2sjxoytrt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2harvimus.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jluwulug.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qvekutyc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zanazucs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zhkfmala.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2juqlwhxl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rfnxbhyc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfovqpsn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rlibfbui.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kromoohu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ffuitdtf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2afdsxwgi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xekcbtpq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xvzlwxlg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vhxoundd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mubhcqsv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fgcgfoei.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hztgklss.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oobkgxbk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pfdlnufa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ypbdshfk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aeyzdhsg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qnsblsaw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cexxdfxy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eusovktp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mcmzgugs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mdprbgae.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cyzdiqyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdckleyj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wemnxcal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqxfgsvd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2punzgteq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2awcbkfbc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ytyfajix.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2eyuxcyay.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zdbcvvvd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ugkgydbe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2eqnxiozh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hppnprcj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dwztymhu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ylcwceiu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2pkjmojix.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2crnxomqo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ranemvjs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twjlbcdh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dylmyujv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xqnfnqpz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zqdeonob.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hnmfrsbf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ddaarbhb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yzzbpfmf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kishlyfc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rkpagxwt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kvprfyoz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ciefixvy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jmypmkij.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zocoozlj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rfgufuqc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2penwnpzg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fzsmgbne.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jdgrhytk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cdtbzigr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gftaydqo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2abkzvlkf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wnbmfeyn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ecvbffln.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jzersuqy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uspylfvn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2etjakalg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kpaldwit.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgtxistk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rasbwcci.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qjrcibpc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mglketww.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdlmtxkg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iaxjclqj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2knmlmjoi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2asrexabv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bzawljcq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhspsbwv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqduwtmb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kiltnjuf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2alegrhvh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jsbilqui.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gbdcnpgg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2dsjtyzgd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2snthxvyv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ejdxahre.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ixkurlty.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xayjbuor.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ohyeqgkt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jwvyvyxu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mctysubs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zcfuqwrk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xbfxeeln.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2onufwdsm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2skfyyplv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zcrrdqau.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zmkaursx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zncrgnrd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2szohrsts.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2sglorrmi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2aiebvxlf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kqfjxooo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfybbnfw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2prjpyovj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2psmfgduy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fwetuqjm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lyjvcbug.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zsmylpex.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdktnebz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hdntqwqv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2azqqrrrr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zabafatg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2thfapexs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qljifopp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvdumxia.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mmvoghqd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jovwcuma.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhszwsie.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uaemuvmc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2brubngel.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzxbtzsw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jdndlcid.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yyoiwlce.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yvzqrugi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eeljrkrd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vcalhxbj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xvbhjziz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zhzxhoma.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2lafqxuya.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2anbckkev.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rttelagw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2myqgfogr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qlznfygo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mmvsokft.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nksdwqak.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qtbtdtnd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2eceyevpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzhzwpfr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xwmxqvde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ordbiklt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2bfloefmv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2cgvqbkla.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2beeftgxi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2plugezet.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccrmrfwa.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zezsouvn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qdhmeuss.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2raoryvza.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2diszabgq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bjjzxyyc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2svbnqzeb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ncaousof.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnpsekgu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ggnodelu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfexzymm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kzkkxssq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vgybtjah.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmmvttxe.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zqkjiwqt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hfctzaht.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qmktzjhm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hhcosvsx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lytijaby.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2srnapwzk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qftvosmm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bdyhylat.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gewoosko.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lxnbthxx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zgizlfau.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2joimjwkj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2twxuheaj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wzfwmaze.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2malxccvs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bbiteqcg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jervlbsj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xvmjqwno.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jzzzbofa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2eimchvln.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vbkhxcdc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qpzinhru.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlujxwpc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qchmqqsd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ibhrkkki.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2olvflmbz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjmlittq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tnefjvxw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mapooyhm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ksphtzja.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cowngkzq.html


<!-- 参考信息 -->