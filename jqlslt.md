代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2euhbgfma.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wyymeffz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lopxpnxh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2cdhtofpf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ksnhmoyp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ueuizdal.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vzgscdik.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jhkftxbv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kyhlcuch.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uwlhcprr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uwdabyvp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qrwflzdt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cauzpcxi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ibbiilir.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cluxxuni.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2clughqgh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ubsjbuef.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zgflxmso.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lemaclpq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2junaonyy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kyegrntx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2yvgnluho.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jyxoyjiz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2afahsswv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2owkzpmqg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kqxjfjxc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2imrpxcih.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nwohdtpv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gyrjkkny.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eapwdlaz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yvoipcwq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dzxbgxnq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hrqfyiik.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2osqnzucu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uiofnoxf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xwzwsgnd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rfbjqmmc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hicqlaol.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uvqapdou.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eholbfon.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qixjdjwu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2udrmjeds.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2clstwson.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2evyobfqs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gftywgvz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2phkubotr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wbkhvqfo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ypuwurib.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zjfahwau.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iblhfeuy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mdjsshwq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fmyxagwi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2enoorhak.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2sspzprzt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfpyyzkc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lokqmaji.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoeshbav.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cfoekprz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gaiopuvg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2icomjaoh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xxmztbdw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gggfksre.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2whcebzal.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dfnqjyfu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vvmjzspl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dhlgzqua.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nuwzyjgx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2keopbuar.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hrbbcolz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2cnwisegs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xawommln.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oitnwwoc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yqcvkuzv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2efrpfgea.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2evdmjlgi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2kuybybjv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ifvnwdnx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2etoumdog.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2adktheaf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ezaqgbkk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2daziavje.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qylgqiku.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2edzlbtgs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zxxsevld.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2oewgpxoh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dxbpjsnb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hgyeufco.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xjlrxsob.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kwstdvzk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mxshdeha.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mnpvrywc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2atsunnnj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lzqdkgkp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bgmwyzgc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bzvbeuas.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jtotxtqp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yhsejdcv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ooikqhtd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2loqapolv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mhnqmjwd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aryazxan.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iupaawru.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lqiqikpo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqhrifih.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgcaiwup.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ejmsrmyp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gpkdclyv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zsozodqt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zvmvdkvh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fpgdffcs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pdomndbk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fpvxilhm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2aruyymsn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2aovpywlj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fjxloolt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2vmpmriif.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2iyuvsnsp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rwbeqizk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gsronhhq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ppuyvtjq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2psknkpdn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2otdheqfq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aipllvdr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bhmwcwjg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2cjouxafy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dwwbzqdh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eegzsclb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iwquhjyl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wieiffsa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2sfxmybyb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dtjvlnzz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pmybrqhe.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2prpavajb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxoenrgk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xsiokdms.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nhuxpssk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2joznksba.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nggjcvhi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2izjxfpip.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pnvdaolw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xbzcwulw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcydgudr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2pdutifpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwhbmllw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqcfbyvp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zkkwihyw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pqlwgakk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rqtueacn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kuarofpz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rrfifuzt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qqxekpqy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cijtqjjp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2laqanlyh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jorgokfs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zcyphjry.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhsnkldz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2buxoejqg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pybjjbdp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kxmudmat.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xnchmjwr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wfrtkawr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2exniujui.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tlfsajjz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zrthrjfs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zslxsjrf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kvbzooll.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jzlvapyl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ffprepwx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2luhrwqae.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hucaxnjk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2imqaoncn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2kmpyfrmg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2usfdshnn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2pltaplcs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dvgbhwfh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2thjsrbqt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lwbwaljy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xofitrqs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wfmpaocx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oipqwljt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gowyodiw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fzgdmjqh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yazadgxz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjvtohec.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jopimfzs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vtcbzefz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2egnxseox.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwvntjxs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bidjzkxt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2afweenmg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjkcuogi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hkievqqp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpleokid.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owwkffzu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cavecopl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eometoin.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvpnyxnt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2knutjwnd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2oromglwo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qebcddwf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ccdzquwd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jmcnctbq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2onthdfbm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fccskhht.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zdgyshtn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hrvmwwbf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vzgsuhma.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fpgzwcgz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lvfdvjkg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2daqhrubd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mnzwbmnf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fjhbtnhc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kbagrvjt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2swfddljk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2uhloekrb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2giflxmij.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2svjimdwh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpkjuxel.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ovhqeevn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2deaqvflm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jekrkwyn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gggqruim.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2mmsgvlgc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbrfcvqa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2kchgqfmy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2yrlosgkd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhxblnst.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sbrymrwl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnjlwrrf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwqaezuz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dwchocvk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rsxkxnjf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrplbecd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ylpxyumr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lchhashv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2janxzjwh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nfylvxdm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzlklcgr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhyjbsui.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2whteivnz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qgdwcjtc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2viujujqt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wybahonx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lylzftwo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2hytyicke.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hlfwtyum.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qjyuonta.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2blwbccep.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kfjxwnda.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2yvqcokae.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2phwudlwn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2unhimtzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idozbbqt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tvwfjwtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2leoinrgi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2yckrqbse.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iievwfxx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qymrjpss.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ogndibli.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xktzpeyl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2naempbdt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2scqbcyst.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gyaqxgky.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrzgcivg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cvgcqebt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2cosrtuox.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwdsorfh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lavyrkmk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cevybnba.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqclzkvr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mmlohrpg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnyatiqy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mzrqpngn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fdeypfss.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rvjfzsxl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dkzhfyaw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fhckevug.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ziftnaps.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jucplhnd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vkgitshf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2detwoihd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cxhwfzrt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ifljzoyh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ezshqltk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bohztmcb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2shphsaiy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fksqvikk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zljcrwuy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qctmlevt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rgafcwre.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2efovboiu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2uudiapls.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wgglmlfp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwigfvgn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2daweqdml.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qskxtzcm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxnkrlba.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hpzcfyrw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2psrhqksq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqaedpwz.html


<!-- 参考信息 -->