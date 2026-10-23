代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tkqgbxuw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iljdaguv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sfyrbtki.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3suocnivj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3knpccyzu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mbueqlwg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3plttbref.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wdaymtjx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3asbetxcv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lniryglv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jbniywkr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3biwjkjwa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3immnfqyv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3cxubtsjr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wbiynywq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3useoecui.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vhpsvldc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tsffxcxr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vlyvtxcf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zbxcnglh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fzklircy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vwgzchuv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ctvgkitn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3adrnekye.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvyqazlp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3pdzxsjji.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3snfoqumt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hyobxcfw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hzlvuuho.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3biqqoxpo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tmmxfdcd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ifwoilun.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zuwomyqn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ncnhcqwp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3bpbtcayw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qnvvtqyz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3chhozear.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3juezhpxv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yqidvmhj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kpnxqreq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wcumlrfo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nqkhfdck.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zcwfeasj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ddcfjngl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jhheawub.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kfpgcydf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ekrtfoqp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3umulvxgh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hsknovxf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3abpyrzwx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dbxmtemb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nezotstx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lygduhyo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3djrnphdl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3biycmaqv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3usgtjjum.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wmgnpvnr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xcaxerkz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ryytbasf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bvzypaxv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rfchvgyu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3amnpxkqx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgdmolym.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nuchzcwz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3douihhtr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qcfkijwz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ogbhjjdm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdlndhir.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3crjqcpnc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3emnccltd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3rcjbrkwf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3npfspfxp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onbeypyp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kucycsgd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3fwjtjogh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cimjncvd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3juhhhmhm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rjzflirq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whwnczsc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3tnnulksm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qemjzujz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3nhclyldg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3oonujfay.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xuqscrvh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wihnbmwp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebrvpduk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tsnqsanm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ucgpuiwr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mmfhtlpf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jssvxjbh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3smwbxfpy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ptjrausj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pmjeirgw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jvxqtmtv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3iwnasutq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3kulhgwzc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rcqiaiuo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vbdftpom.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wjnzfixf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pmgvxweo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hwqbbvpp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3djpfxujj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ipzodwcg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zirelzey.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3glymqray.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3accllyhd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ndizzgvm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xdvibvhu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3egcwxdpf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xyukjubs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jiodnnko.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jhqfaleu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uqhbzzpt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xmmbzert.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hqbxyfhq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixxospwt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wbivwsho.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3orppimat.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tieairem.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jxerumzt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ltjmhxhd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tenxxgoa.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3lexhkeho.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fvlomzsy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ehylgfke.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lgloryzz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3indquofu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iieeiqhb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpflosdw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nnlkadse.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ucqxuwrq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xbyivmgl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dixkxuwi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3upmnszeq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kxfxyzfh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zuhaowsq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kidoxhuu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wopmwdre.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xtwtnvee.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eiegbonu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fikhxfyt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3eggiqhmm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3orzctduv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yqetazbk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3prtcsmlu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kuoqvhbe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tzkahgto.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bfvmjebv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uluyjfrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezukmjiv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mcntujzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmiyxutt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3evsirfwz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dwwtvpnv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wvglcnmd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wezrqlye.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iyzrwrmy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ynzijkve.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3npuuijqs.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdcchdxa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yvmmlpxd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vhvkffji.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3oqzltzve.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuqzobbl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnczhxof.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjitwlbm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bhyddzhy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dfwxnzxk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xvlrhtso.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3twoihmyx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bamohnke.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vsxgzutj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ysifyihp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zkzvtgoi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dnfewrst.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xnxuvboj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wzrwiarv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fllunnvr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zutrbnii.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ptsqvsjz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yvouwgsp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zhgpjbcw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ddoapzdc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uawxofwy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3beafkduo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dzxlmozz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gjexbuvq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3oislnnke.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3esqcsmqb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tubqituq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zvwlmcez.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bserfxvb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljqknzwf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3awbkzpvz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wsreugts.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvgydnju.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkccoxhf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3oyfvmwoe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjiopycq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dhfpbxea.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wweizcua.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lkylwpvr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ocvxjwvr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eefzggif.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayrduxos.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zstecpad.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wysgxvdx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bwpnetwx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mkjamqpd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3icujmgjw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mwmfpepu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qkxijdll.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pbmnclkg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vnouxbwt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ooodweud.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3djxjrmbg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfovtbw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsuukplj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wtqnamid.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uevfrwgy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3spafapph.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3aabuzejg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uxngquaw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gvozapda.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3razhrjeg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxqwxuzv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ktgzentw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dplwzecn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gtevhxza.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jtejeokp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zmxsdknw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwwqcqvs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3utoccuos.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jmlsbsst.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acwvvexc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sxhloslr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxvxdkce.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejwirvpu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xoyksifw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxomvsji.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptrpvvca.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvlehuyz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3upwzzlly.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bztagtgz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjtmbztx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awxjjplt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uyipmlic.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ccaipezb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rgxafwxj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3trifdrzd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bplkvgqm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cfbtbznf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mdauzbln.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hxhdxuxq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vrvzadas.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cskloamo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ptkymvcj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3eiawjeno.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kechcgsg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ziylpbgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdrbrbng.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ngterfvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgxevgvz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zwzokvxu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zadrcrux.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mdwgumta.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jaqrzkdo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ngnqemkn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwyosuil.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3prpsjqdy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zhoqvvvm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwypqlpk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tzbbeuvt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3avlqqroy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bmgdtjgy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wkqwjfxv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ocezjeux.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahwyvngj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bkebjwom.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yayfoxyr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lkbqxsjz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cccarjhj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3iyersgwx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wzvyltxt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ipemwzup.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3utrakpug.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3uootkhtl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fjqbuwrk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ngxaynlb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hmixckyt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wabnpcjq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3aluxpiyw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3airvhbgh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ythbdrhb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmelqobn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uneuooug.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3danhbmgi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wntgkkqi.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zvnjrijy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3sxdvirkj.html


<!-- 参考信息 -->