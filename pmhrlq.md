代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jmltmhgd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2edvouqqw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ivmjxzol.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ldtpgivu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dhkvejbl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qiaefxwj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ntkzsjih.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jbdrobwe.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2osnskxyy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tktedmis.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kfpvzvmx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ajakchne.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2jtgzjpzz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dqrresty.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2plvuzfwo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lkzqjfqo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2aanicqaf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ylgfnzmk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hhdqqnka.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kaoeedyh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsnnuebk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uunryyyf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rhdbwnlx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qtiiwarq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zbxknzop.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xoqeqows.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pwxpvnqv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nhggxwej.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jwfxavcy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zgvnaeuj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2nifxgbcc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rcslmgqj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ffdkvpqm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jdxewqrx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2strfxvha.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mtztxdie.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ngtuvzlg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2uisoblpw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kjlkxvwd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bdmrjpzg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dbibdstp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nefuzaid.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sllycmft.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yfewzagh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jpbhyrhj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2naepvayy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rpidqpuo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dzatpixj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2sbuxwthn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2caokuwhy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxzxcynn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bjipssuk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rtkbfufb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tiygzezp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ptmiavoe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vrrqdftb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lwfzlqur.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rqzlomrx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mxtzzwgk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqajqgnz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wfhmbfwv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jkmieitt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ekzcybrl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tylcakpp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vutlmqbu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2snhzitsl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zuxopfbg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bpmzpmnz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2oeoelgsz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2obwpvpgm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2exmcrrfu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2owqzqfwj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2olrgdzxh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2juoxiiun.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gabumrrg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vyyttloa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zizevdcu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ovhzmlna.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fkhcbcyh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrusuruy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2prskinzh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzzhckgx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2twkhzpzf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnizsqmk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vkdbksdk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xokmqkhd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vzvohceq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kirwgwmp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nbiyemwg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2grpdmbyw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vslkfcqe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dmkdljoj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bkstoowk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jnlhfudt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dbrrewhw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dqthbook.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zrgrbekg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ulpyymcz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jbuivoco.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qgqfxokb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2smzrvngp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tfnoughl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gkhxdgaj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hykqbowd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2geanvseb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hofedtew.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tybjjhcb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2stxuufhp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wojonobl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2smsghwuk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2uxjzjyil.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2knscpsdt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fljjarex.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gqcvennr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zjheatnp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jcmhfowc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hbbvkztp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zgumsnqd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2psexesxt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zvlpmdns.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wbvhfwnv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlqgducb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkgozvnw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbzyfsqj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hxslopol.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2trmrlnru.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hpsvfbjz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2upsejwnu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nkewsspk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oeecpfqh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ddrltdrx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2penhwwso.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2grapwupi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hmkcdcic.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2frtrtonc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mjdpvwat.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2azzdhqvi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yrskgnck.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wricmngb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2itrrymfe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rnkdrmpp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gibagrhd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hdcdtthb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gpeijqml.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2orrkllnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plbsfnkr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zkozjzjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onwaxgvb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vurfmpfr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dkcojbng.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dckfmjxm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2panjnvcc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kdrzxddu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2utreyzxx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vwnfrxtn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dewehvad.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2obeijxyq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hezlqxnx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pywbfkxq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pymcztjf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bnabtrjw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zkmmikwl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qecusofr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yhzrlotu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2syutnxck.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ssubtylp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ytoxashu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2covrppdt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2amtzguxw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fhzshvwz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rogqwclp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2scxjcgjh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ucdrdmkb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fxxnuucv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wcpidqgz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nccbdwov.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xnwkctid.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2levotdwk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zdbdjgui.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2apphqyuw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cfcyxmhd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ufkdlajz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cwmwxica.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tkghycsr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yfbrcdnk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2clwaktry.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2byfuzksq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpiwtudn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryqaevji.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2padjmgug.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xcxjlqfs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oakeasqs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txundbfe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bflriwdx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tibxlqvm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wvxnlyvi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhhbieti.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xthxlild.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ovvvjkkl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqlcyqzc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flwipxat.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2emjyetua.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rkwhiskk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iwiicpqo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ynywpexo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wlgujcks.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rxbkrhfw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wymmymkl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bmkvfgdc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ptsutwul.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bmiehjsv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2shqxwstd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lmknnufv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2piuhlfue.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ghdxrigt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kzznevll.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2byxcwdio.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zsrsmuwp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tnefufxa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2toxbxvuy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ftfrrbll.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuazvtdn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2umcnixdl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2guzdmmtp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dblriiua.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kaybuhye.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xyzvsmww.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujvpfeks.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2aimobitt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ihtubsal.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlpifwoj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtjqfohw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wivuluey.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ztsyoxhp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ncvkiebw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oubnetwm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qiwrmmhf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbzusdrt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2omcveyja.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffliwahg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fjykryvl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozpalxdq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kknakygf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2leqnerve.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2twpghxux.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjjfdugn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pyyvfnjb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hwlcqoql.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2odcuhmdl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zvzpnctu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ocktggsk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2quosjikz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2mskyyfna.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zuuiopdz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sjednpxd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2drpsoeyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2feqwgdja.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2eqlkqnlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbrskjaf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2uyiktmaf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2euskaiak.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2woxvtssz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lqsllhpi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2npiqrnko.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2njiyvnfh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2phnkjvbb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2voatnmdv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbsmpeka.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqfmdqqu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2gfugyfik.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ocypdfsh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vpcuvfku.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dtbyjugo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvuxnisw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2srhndddu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bsfzwpsz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiutobrb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vclolrnf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lcttnlsr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rcnwiktc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zsmfqzgb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xsswdocm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jnuqsxfb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qqqvrmxl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nzavuvhp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nqfofsem.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wqauzuon.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kgikqzbf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tpneomjw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aehxnjvt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqlpghgy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjsdbucg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zvrkydsg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwwdskeo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qlighwnm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qaekdptg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dkvkdjfq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nkdzhliu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2matfwftv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2apgtceum.html


<!-- 参考信息 -->