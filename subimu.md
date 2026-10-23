代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3peudilja.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mzqtfwxg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3druhjdoe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tvrpfkbp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bxtqclqa.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3rrnkypvj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3semhdxxr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yvqsvzuq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3vkqgofgg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zcpgziit.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ftzxxxmf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jurhinpu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3zcjimdkt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3sarastpy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ijdlgwhc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3pghwlstk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3fctsdkch.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cbmuouxq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mtneibyp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjskbgz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vywoicxv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3anjkeyud.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tdjufvze.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ediwsqsl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntyzlsde.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hbbxpeck.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qaykrhfe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dxgbvnnc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yypxegbk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3oyfrjmay.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ywzjlkqi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jzogngvh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zqmvcouy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3muptmwwn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3eabylaqe.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3prhcxdkn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ibufiukr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wxxrjzeg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nenasyof.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dkbhcysc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dntxagjn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wkqlgsab.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hiitpwhn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nbcncczo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sipijfwk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cvwsrxqi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3aqhxnsqc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gyfmktaj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ffhuilba.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qdskbpzr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3sjfluaez.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gdsnjarn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zuhhnxbt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iraelvxe.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gxqjesde.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ztcqdcdx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bjyklais.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ejnahtgz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hejaqinr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nqdekzee.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rmluiina.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xyreweld.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lxkhznca.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxdtorib.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3huqnuxmw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jsyeqpnh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wxahgmxm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3usjtddkd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qhlcxhgu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jsusubws.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mofbrhij.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3usgkwngw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mahfpfup.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kricydxc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3fzalslls.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bcownifw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cgxyukjt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3akolpwrk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjdanfcr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dehlvvyn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3izumnbhu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3voxjgiis.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3wayfhzhb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqicvywb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3qscunjdp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xqzwvuzc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ovupaebm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckczjqvq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xfbpuocr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iirrwbpx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lycbfeem.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uhdbzbii.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3seycxmzu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cqfuvlzk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zjebpgcj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jyzantnf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lxlbnlyc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ofkkzfro.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dkrivpnz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lsgxsfpk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjrjeps.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vurgglzk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rflrvpjn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hhfcclfp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hbqucpfa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3sxjxhdyi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3shsjydzj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kbxlcysu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iykdymav.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3alevxfkd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fbdqzqsp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cuqukaeb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vymjqqjc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3skwfkapw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zvwpkbxh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kakllkwb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yczreyyw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3myhxazqq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ynoegdig.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dslxzvud.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mosdnhpm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cytvcxhn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3yixofkfw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vifbugmw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ynqmpemv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzswnowk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3drtdsufc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ewuvmqmu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvsuyidl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xjsakfxb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fffddgjv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lrxblova.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yrqhqpsk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qqhezidw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xbrscmwx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kasxpsil.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ntcfzvmk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3edihojlf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mttrkfet.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nejxpais.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3svsnaiou.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvcokkwb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nwygbsqb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bafoaocx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nwjorjwq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yqsipkzf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lchmsysz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dyhgwtym.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wzkhbxxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amzsnceg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ixwnmwzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3purxjkhb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lslcmllj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uncvojfe.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3emmxorgb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bputgcwb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jddgzggf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eiushmmj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fowjumii.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxbgwrgn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjuntftk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jaxmjayz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mcahnebi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpqbubae.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtgdhtoh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jizeuygc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yksldfty.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yjzzyycl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3okaalaxb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lrodvwna.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fllwyuio.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3srdbziku.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vwuwbpfn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3stjtojyx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wpfdglva.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3leghboer.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3eztlxhph.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mejhplpb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mknlhzxj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3spyswxol.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jmxmhscb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fjookeew.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vreibatg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hjebcbek.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wmasinmt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qqbolhjb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yjzuwqhd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3epccjvqu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3focnkyou.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lmmrszur.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ftopntrp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oabwyvzr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obreglyl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wahvqxjd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3iceyoead.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfihilnm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgwpduho.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3odowenay.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwcouoqj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jrtiyoxx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgcqohai.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iboezady.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ndmdplve.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxlpenmr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqdavyoo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ovbeaput.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hycensfy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gsoxzebc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3cmrxwmdg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dxkvpcse.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qhkbwuok.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bljwbbjm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3psagcifp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ljhflrbx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hdyzmtde.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lkntrhqp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3gwdtzudc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmrhymin.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dkowkesd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kobjkrvx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3glythwnu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zlyoerwc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ezstqwmr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rkusuydf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ijplkxsn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezrzqcct.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btwwezxd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kiywmgqx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uerrxeiu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uebfdqcq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gjjhzkpa.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3efjxlhhs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uvnpgctd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bgtzpstf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcdddjqs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3renklkzm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdnlnwmz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mimznhlo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pqegglsr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzdhawwe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nuixirpz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmtlcrtn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3bfrjpqhw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrkjjvey.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xzcvwqde.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3apsmeyfu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihfibcem.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xptpifhs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cewxhpbt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzkxrqrn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sgkfgagr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dpsgjsgd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3dzgapgaw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ggicgecq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cngwcjbe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uhvljtof.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wtuxxpra.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ohxggjub.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hkahpavw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ovjfjlru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjdgriok.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ntszgiyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfbcfloz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zdjlzvco.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fcddeeqv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ildmugwn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bztucwvc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vqjcsknt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxruhyin.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zqlvwiel.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3otdoqibp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnschqkd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uopxclun.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3idfkxjvo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lpcejxei.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djtnwutf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mygjmlqk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rwbovmon.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dxtxiawl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3liejvgcd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmlpymid.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ljbvxjcd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lngwfjww.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ymzybdnf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vlfadujy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oyuwtono.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fffxnunh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3iapxiuih.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3acnjoshg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cwzibxxg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3djqsybto.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qzkqzbtl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shsrbiqz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fuwnkjsa.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3drbzvxir.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugapmdnj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fbnoqkfb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvfplxgf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iciykypq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3efflnorc.html


<!-- 参考信息 -->