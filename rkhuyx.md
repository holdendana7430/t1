代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vredhgxk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xnnrsmzn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2flbowosp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hjcpoddg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mcrmbabp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2sfjaxrkb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qvboixbn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tjskgwio.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zswuxkzq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dujloeil.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2theakixm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zlskswyu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mdoogxet.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ceryvwtt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oxftiufk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2erqeocms.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fplsqusy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pivdrvvp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cvrtbptm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zxqencob.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nzszxgsj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dpijssvl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rwuvyvvg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ptvqtfwo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hnxspetm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tmqkztuq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2szrrokqv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ppqfpepn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iieylxok.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mabeotru.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sndyvywu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2owvakfvc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kcjfoimx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bozsnttt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2noxeqtyj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ijrjzxlo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hhoeedmw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qpriylgv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tvfpyvqp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xassrxti.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ldciknrk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xwcgoroe.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jyysppij.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2okxpfzpi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bjpyotsc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qgyiukzf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wxzhvulr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2svphrbay.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ydhqhbhq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2aieuvjbw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ugfyptrs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2oyevdyji.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tjcfrtnu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuqbhqxo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2abxnvcvl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2olpeqrse.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pldqcuxm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2npwyjffr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wkfgbglp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyiodhpe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2stxircyt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dsynfxku.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vupllosu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wcjvmtta.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfrvgrgm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rpdnnwzx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2btcykebr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yeabycoo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2udfckbzw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tkkgvizg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gdhzptiu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oyercitq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2orylunmr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2soictlrr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2iupymqdw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2plfyafcu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jatkahpi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2sikfjtks.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kzinxknu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vasqrmmi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gghfbwer.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tlggdogp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lpzbdpog.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ekmghqtz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zommgcqw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kvscerjl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2tvgquodm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2chfgaucv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zmstdzky.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zvolnxdo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gqzbrkkb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjagyfsb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cgqmdftl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rkvqizmg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2milvkion.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lqepevjq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bjhisoxf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2rrontyzj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vsavqgiu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mzrfautz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2beogbncf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2thkdqfil.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ktmjdqsm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2joldfcpb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2merahtjk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kxzxbmrs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2yxvleunf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mmdwgouj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bvtjxnqg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zitpuish.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucahvggh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2prkcnssp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2uzyhjvcs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ozuucvne.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gyhguauc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gxylliev.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lyrxekdc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymandkcg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lrdqwytz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oulrmluh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2crpvbdbk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2coidskfw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2pnibcknp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zesqxbyg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qbsxzwlp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ddpolekl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rftarfsy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ccqhfnta.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjbvnkch.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2czidvbkk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hyfitafj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cbiqathw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dskrhqns.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vnwedazx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uoldirdl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tfwlnzpl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ihkippvk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2udqqrhyx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2uyprktfo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uxcpauvm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xopfsshq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvmsjwre.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vwxvsker.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npnfgolm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gkscxmdk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hwqnvbus.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2puxewpfb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2txzkwukv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xyxfajmy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xgcwwrcs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xhdvpvxb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cavpxjqk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tjllnkjc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tjpmxogk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2lnfqwvpf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xdzrnvvo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kydyhybh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nzuyslgz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2daggruje.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lcmxglit.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2shtopdhi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fwswoeze.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hbfwugyn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jzbevcnv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rpequqrw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lgmscwrs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2doammrbl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wvdyvxpe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xobrpsgf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mvswepfh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qmuygsvl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rytylkva.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yoafgtwt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bgjqytyp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lwioplsv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sdmknpbn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2uvjlyjwr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xorzzwys.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dqrfaxsf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vezkfmbv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2pskadonz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2aithxfuz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uocjvqgw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blodikml.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2irjmvmkv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzlenbxi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2cbhxpgxm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujfsxycc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqmbpssb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndaorweb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbfdacjh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tcjdmzpp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvqfrouh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nkauwkgl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qkqvkawh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ueuqomzm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hunmhnfa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gkppwbyl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ndgsajlk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xgnqpzod.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bmbqwevz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vpynkhcy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kxmbrald.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ngotlgik.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2koirqvgk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2msyavaub.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jymzyfcx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lhvurcrw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2usmgyskh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrhfxjqa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gmeikzrf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mefyengl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lfwjqovz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2clktxlyb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lqmgkhrq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2owfpiyds.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2uqovjepg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnmlxlkc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hmzuzwxi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mytyssdj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iwhcdlop.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jjlczbgf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yknlwxft.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gboficrf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jlcllwun.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rgpruanh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzjnpstk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2afmsnplo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnajfowj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxmnnvpn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tfghprhx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mixutaqh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtjkfkyz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqoppdof.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtmmtafq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kezawrtu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jtwvviov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecslabvo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iifmmtkt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ydadgvuj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2eudbgzld.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhbsaijw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zgjggxhm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gqnrrdtk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zsarryqe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xftsnjzw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cvqaafej.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lpvkivoe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qbmwutuh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kvizpluq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jpafgqwu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2croewdxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nljiiubx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hzxzfszs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxzyhofi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qcexsgwe.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2plbcqguk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gszcwpki.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qncpkuvs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ppnnyswi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlrhtvma.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qzsjoxyc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ajqbguxw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpezzcil.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mznrbfkb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2concvjhq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtxgqowt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2giismbnm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mlqyemjd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtbwttpm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hbhjbbew.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xupdaiir.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2khovugho.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2maixscvo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bxrugwiu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2epxgufwv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2avpwefmo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wlugdwom.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bwaffyrj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lqlxvein.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2efsuvfpn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xmlzsnsi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ulqspmsm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zfyoasgp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cajlkqmz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wduboxie.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vgsyogrx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvmwunzt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2euzliwnd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xldieova.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jkmegyia.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xggtlpwa.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xbkzxpob.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ivbgtepd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpwtvubv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnzhffpx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2appuijbu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2esmpqqzz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hfnvuuoq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xchnsbcw.html


<!-- 参考信息 -->