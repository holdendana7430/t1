代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ldwrtptu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nqxsjhoe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pweykyxc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwtxkmzu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2elcnsepp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2anwkwohz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ghgquwhx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vapoqvke.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2oiusmyvg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2pwywbwik.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pzgteihz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ccbyepgg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xolmgklh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hvcypany.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wqqtmhjh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dznrefns.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mmnedgcy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ksusvxbj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdomyuh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ibcaibim.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hbtqaqki.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nzdximpm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vcpcsdot.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2csizvxyt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vlztxlmc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ywteqxwu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2iutwtilm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jhzxqcdo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gdpcgshu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2soetsidu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hcwrnibr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zpnhoblc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hnnqxxpj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cfceuxjj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sigzujzj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvdxyai.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kbetnhal.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qugbyxxj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2phooexpf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wsficlyh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wwixzxdp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gsejuedc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2esovjxsp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eeroseoh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2clbydheg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lprtzqvx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2yirxatyu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qjcelznc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ykexdhil.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hnnuwvbj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ewufwkgb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ikkppmvd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nqqjgkbo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2payjidmd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vivhenls.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bkvogsmk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2whplliqw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gugzcdgg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fpmhafbd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vijdxejn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpezfimb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iakahrxn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ehcmoeki.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2biygoqcj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bjafchhh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2eipotwbq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nzwvkmrd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zvfmkzog.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ndhgexgp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bpqitsjk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2czhwnlcz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ycvtwovr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jzchloem.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nfqvefok.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzusuysi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dvmibkox.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zsxtarsq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ojmwzojm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pffjbpfc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2btoyjpgw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fysmymeg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xfwnoxwa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nvgoeqcv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nklrqbyp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2mlcmviyv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rdjenvke.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tuqvwceu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2huthmnsy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xplwekbc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tjmipggj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ldtrazyn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rlbyosud.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qqcwdbvd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mguxkwac.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zijtbina.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wlqraiwn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnodzslg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2iiztkbeq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ssuxgfbu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2axwuesmu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dcqezosm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iybmwlam.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vfdjlduh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2irdduqva.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2msmlevur.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ftxiljbh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aftatybt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tabzdlgb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fjlscvnl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cufixtbz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kwdoycqx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vflpczgh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cnugdbub.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2atvffjhu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hxihlvhf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ikidpczv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2udlfddtq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2shoyfxte.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bcwqcikq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jnxttzir.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2irbfufiv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcnkmugx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qtmwjoei.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntbzcquq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruvxmpfw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dhxvnbqd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahwckzen.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gawbtwfx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2htrrnbas.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nujejcmg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yzlaqsaf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bmvavnyk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vxhrmfex.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ygmlrcza.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xebsuggs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2egiziyjs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dklhyqte.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ufwvlyhh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zkfaikfr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xyczpxde.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oruhvapj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lohfunfn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2evwqcmig.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yeofxzva.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hmjfsvxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqpweuwc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nnagabsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yosonkkx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ynzgjywi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rmetuzry.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejasgdwk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jytldfwf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cpunnrqu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gmundszc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tpnbbvyk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmbvkyhp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2irdfdeey.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrivpyiz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2krrhxyyh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2irhxdrnq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bnxrjssg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqnhggsp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bufeoeyn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uzxyuntp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2anznafjz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kleaqgdf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qavbpein.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ebxqpsae.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2grbevjab.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tdsxghkh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hkcypjft.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2wbvstivp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2epgglqgs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2cbpvurps.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ovbirykz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsmbrdif.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kvlsntpm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ostermhf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2niwelnrs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2srcinpso.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nmjsakey.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gfnawouj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2boxeqscj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2szdyzmmx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fyoesogn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gktywlbc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ravsfxik.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sehhlhmc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kxjxwnfr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cxkbromv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rsbvdmvi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prmotkce.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifjxlovf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2vvhkfdrv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2egkfzkzc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fsxbixsn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qrivfjko.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gtxjlrqp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hcwlmhqh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2chdfouxf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwjrntsr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sqzydcmz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zamhwarj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eokpxlvb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lluewfvz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bimzcwgi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2idubqdbx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2susarxdb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dxyohnpf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vxulkoao.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2onhyyqve.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fyieqcpr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjulndg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2exfutzav.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xxwnorgq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gjoqbcnp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wqtqtims.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cigroumh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2phxgawpx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2embluyhy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pkzecgba.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gcdevhfs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctwgdbli.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cbprvuvo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lcjbkbft.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cfsszoez.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2srhujfwm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wevhyhoz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gzzmbxsn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gxthiqty.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jlmbbhic.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zdagrkpo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bxqverqb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftmtspev.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mblfotxf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uyhtitzs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvovxhwx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kydqncfv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2curbtdps.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnavtzya.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bbyhmwig.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqudtlnz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwpkiohf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bzswpgcv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2icflopjj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ofzpiwsw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ipijeyuh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mcvplnwb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tgzzatdf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pglxdpuc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2dcekdogc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2byqofnnc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dmujynoy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2lyfhqvme.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2oacpjdhb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tvzvxwne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yheytfro.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dxicqvgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2psnyopqy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fxekxqng.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2swzmbdcc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jffvuqwa.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2khoezgkq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsgixtkn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xxbvsyqe.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ynvvdfou.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jdklitms.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyvegzvr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gsxpwfxk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zqhwuwgt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epphzbjm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zrwtsnos.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ffieylib.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vdzdscxq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vxcinllf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kpswjubn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scscrcji.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yzejwyca.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2esroukda.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fvsqypkm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ellxvjic.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hqyxeyvw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hpasdxpa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lplukkha.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nyorkxqj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wwigjzio.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2udbaedqh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lxtyijjy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ztzagtsm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfsqhked.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2owlnssew.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxnrprqn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tocudskv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2agumtgpa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mcecrqtl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mgzrobaf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qviqrvnh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjwufklk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2trboujqy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2flagobjb.html


<!-- 参考信息 -->