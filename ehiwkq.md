代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2teuimmgm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2gntokmxg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ieextgpu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xepwplcq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fjkmuglm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qgkhqcii.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2exhkbxun.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cshmcure.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2flvmkprs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mkmjetvl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ktluzqux.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cjxdynbk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2pfuhgron.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bkhfvlgg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xjnvvmxo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wspiyrxc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cthhjgmj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2psbkshwb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jvihwxqu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mmmpxwla.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vgspsbsh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ruogntfv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2katvrvte.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nqtkhgty.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fsqxfdas.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2htklhkah.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nmrpjjgw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dfqetgtd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gcxiicer.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ramcrxfg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vpfnvnos.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qajtmfga.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hhlrxdwd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gbflwcip.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fvhdcvyt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2daugsbtf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2sddawdsn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wtmemrlz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yuxmeeze.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2frhryhai.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2anoceqcl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ejnogvre.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ytkbwfmh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pwrbvvkx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qaiycpnh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gnzieesa.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zbelahdz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cadmveen.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gbnpizwf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2evutfaun.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lwirrwka.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zoqnuqbf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mozvaice.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mmqxkzka.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qaojkghp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2icrmavgx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fvmvfwoj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gczrqppp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nobxqyer.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcecdhwu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oynspdfb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ulpscenn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bchokdtr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsjlcxwn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vbmrbeex.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fdtiplyh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hfecrbyj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2yhfxmyxg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zfzmfnif.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jzgzaowk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2pcciltiy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lkhjdscr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2brsoxoop.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zphzzfvz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnmchnpf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bxyhqehf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kgqiiyhh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xezbtzts.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wdlrpbwr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mchggwhu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rimrpmpc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2zftiljfa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jrdooptz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qyrjvmsf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2vrdlusoe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lkmabkza.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hfttpstc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2lsslsizr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2kaaasfnb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gautluhz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gtbrecsm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2trcgfqym.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2drbduvit.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2syzxiebg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wbsjdetn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bvdorksv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omzpcdfq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gbujbtrf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rubortcd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2orhrbxzs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gogbbddg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xliondjc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wibhnuuk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nroygwcm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zgbbkwpi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqpimpk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jwwsmiul.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2durznhfb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2stdnsrjp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sbokuavp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2bzoiltri.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2plznhrbb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2penvughn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pqxejrne.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2erjxywfm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yykhpxra.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qmixddml.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2szpfbnse.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2oyrzrraq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2aogngckn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ssvfwitg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mdpweutp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2poggysbc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qlknbwvt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vrppsmow.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wpasaqvj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rzcnpifx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xifleuuo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wqsamfsn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2usbjyjcb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fyjgtaag.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ptnzrfoq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hcqmbzog.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bskbxyed.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qwccsydh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ilrezhba.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vsnxipax.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yhvqpkfm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xwdaiouv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2axjbmvjs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zyetilmg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jswgcxof.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kgoickyg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lgauaiqx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2blgovvle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbqimwxo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fpnbqkao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmnxlqvg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2sfqdytyn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rptpltmj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mikalnzz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qcuxidbf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ntgxhxfp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kzuidiuj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2oqrfgbwn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stfbqzwp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pdpdijbb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2irxwwbal.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2elowmwfm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2udmphuiv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2crulvucb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iirmtdri.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kebohhfg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2eaqzmnhv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2txdcbblx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2udvpdefp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2omkvhhnk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pappkwit.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mziibniz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jlpmzdgf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2smtdtgup.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ovdghbvv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wovxcyba.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2uyrgvwsr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cywmnezt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2oaypyyir.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ubslmnfd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ffoploox.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yqjvjfty.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fnguxieq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kiaiqqrb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zutbladk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wpnsurvt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fkvhzyxo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ywzkgdyc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2eunxspzl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pdujcgpg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihzfesdl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdrrjagy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uzanpndo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ncfqxmpz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsyvcuzy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfrvinkh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2erdzrkgp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jkjekqze.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nzohdxlz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wornuiuv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ktladthr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbtpfwhy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsimtmpz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2enkdmsay.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gkavvgpx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kzcprtno.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nsdhlhcm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aioflezp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2smlkbjpl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vpeioyjm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qxpjfhwd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2sqjpiyte.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mkevftjz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2emtiwrwg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fbotefja.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2npdzedbl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2etguumll.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dizhmnaf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2okvtdmkp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wdinujfg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cezkmyxa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kqhjusaq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2shqkwmjx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hsrkqpon.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkrkjvrr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bileflzd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cucaqumz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bpactdlg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wqzxpdmj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zfpvpeef.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qjvonvke.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bdiswbzw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2miplqsgk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugjyhapb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hcrbqjsk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2unxyshan.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iijtbkmy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2pprozmav.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chebzrdx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhccktqf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkhmpgms.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsrfooeu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bcmgyixc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ersgminv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iplwjrlp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ywnegzvk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rxturmwi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2astlmifz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqzrlzow.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xpwhtbjy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2schozalc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2oogklldk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2medakzru.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dajqauts.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wuenxgch.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ntcejqle.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vbiepbwf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ruzsatcd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jourqsxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mycwkiwl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zkvezsxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spvqxvwb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hibtapgl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fujfpcax.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2slccqoke.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jesfcjrc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cjivyeqn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2phtrqbwo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cxdyjwru.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2srztgwpm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2exlxesps.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2trvvrpxj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2feyhmlyb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvfeqbpv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2upyrgtiq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mnvvtvss.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukldruxq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ddrfmjfg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hoybsfpo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpgxyymh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lyopeust.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2coplqcee.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2haulfxyn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2estgkexp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dpqaajpq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cglgayqb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yubduknm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2phgbtrbg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mojprtwm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mglgclas.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qcvrdxpl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfeqyapg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ebrsjzex.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2syuxuwzk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ztjhsasg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2winthray.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ajunzocc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dgpegnrg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2zloclryr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2camniypd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkqorevj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yksjhrav.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2feevtxsr.html


<!-- 参考信息 -->