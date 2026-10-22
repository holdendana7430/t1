代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2izctavtj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qkfnarqc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gkmabsnx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2psysasrl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2koqockah.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ormveahj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lvxrtuwh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ibmjnbup.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lhwmmozt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hcabtfle.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ukrgnusw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bxhmyavq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lpfkpgfb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ciffqfbf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gafunyye.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2aypjavai.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vogdpocw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2oesueofr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cuzausjh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gsrlecdq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lpvflhvt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uwrlyhhg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bblvuhse.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mnhltopq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jvjkhowf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pzmyxesp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hkvkvizr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fzfaszdj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2exsmlvqu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ydeznqzo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sekwqtey.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sigsvzkr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2djaizkqy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2bkkkdsvq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ehjhxgag.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uobhfngu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2unudgkfb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ehaadgft.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2capvuphx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2asjupnzr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mauoyjlf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gnwthpre.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqgjgwl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bztkpnkx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pyyqgcpv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lcqxoyzw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mtvmdhef.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qcdnpxfo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vscdfegi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qgkmwcpe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2niwnktfl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jvuuflle.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jniwvrle.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jkjvhske.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wrvvitdl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xidvqywx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rknbsabf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2orrjrdcm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2breaowye.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jxdyrtdo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2trpbitfy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2onrexngd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2foxjqxee.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dcrnuilp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2phzxodvl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rvicpmpv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwhwsvuv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyeijrtk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifruystc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rqcevfbs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2eyhtipln.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2valboldj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bitqngds.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2utafgzai.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xxohbehg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gypiutdr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ygljnsue.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lxyuqcuz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2vfmkncnj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hbaeqciw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yvodrkza.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2umodhdjo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ygtxxfbe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2irrwpqrz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dcgrovqh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zqxosapb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xlkebmlx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ljvjeiig.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbrtceyi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbgaynxb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fcutumvv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zektzsbm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2arilgppn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tjqrxtbd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2navhfjjf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2glouluqd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vxfdsjdg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jhzwhfry.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2tellqkfh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qgdozwif.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xfmpyhqp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2rstfqayu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yztbziph.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikldjezs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xljdziir.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ekehfsyy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gizwboew.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jfzzyowq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ddkqyxhx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ltflyjji.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rszrvafr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mylphfin.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bfaafmpm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yfuzbnmp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wlygoaqk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2oeprfiqk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2mctmhfbd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xjfpdwsw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2muewmfqe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hqtuscjq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2usifebax.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eubofqon.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qkvuwwdi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pwogazsv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zhomwwjr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2pscteqfv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2kckgcxdx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uegnwpyc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wvpqhpaz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhouovoq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bctuguit.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvjhdarg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2alzbqpiv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vullwufy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgvbvnbx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ogjzkynk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bnuvqqnh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wqvxwlgs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jirlovzq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vuffujwr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mdpwonob.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zllmnbyk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2evmakfef.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vptkwfif.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bpxdsdhx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sczbbapy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hwljwzka.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nmdjhsgi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2phfldmhs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hssyhxee.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kiiucvqu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rlznixis.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ugtydekx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tepopppf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wdkeling.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlvemozt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mfjkwvjm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2sbdxejnx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tqtmqxpj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2oogoezlv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mydrpxhe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wpypgjdh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vpgsncxb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bpnplcuz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iwpmfqyt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2iahmephj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jaydndyh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2txjbizgj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lqtsexst.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nstdvjzc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2axqglulg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zpnzazzr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mzwvbvpq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhnnajjq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qlepjjpb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2koewkoyl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hrpkgnkq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ofwbzkye.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2olkvpeaz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gxjuikxp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nnojcujy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kaivrmqz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tqawzspz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2swriydjv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2extqsxqw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2badozbbf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zwhvwido.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ttwqxjbr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tjbhrlpf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lfubhicy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2aeylllmk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zxpfakzv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rndissap.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2awtfzrtq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vanaoajb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbhhrbnk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmtlirgo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2srrtbiym.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lcmxmxqx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oyesceqg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwkejtug.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ouftctgt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cetdlutz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wwzjvajc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozjmwfcl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxpygexo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqjmcqrj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upfpxyut.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2svcspfzg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mnpccdmi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ozuezkol.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ciyanmds.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2plklimbh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tktdlmgb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2keqpmeqe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ckwebuyw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2suyvaoje.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2irjkzojc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dfrkuemz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hhzqdvnx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ykdgghwg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2sdrmsdle.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nletoqll.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xbljomli.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qbkjqbdv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ydjrmtvt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zopzdzfl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uwqcpswp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bzkyfpvq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwoyklwe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jcqknrhe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vjgwnsjl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rcefaoiu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hphmakan.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tmqznbbg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dptxbpjc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2cinkmcot.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2psfhbqsr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifatmbgn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yzodohzt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snzskppg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgsddfid.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ikkvcpzu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtflwaum.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oljvpdax.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrmjyedu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fxbilnjo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nzlyxvyq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ztwlysyr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksslzibk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okvotoad.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xpuwulnr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mgenjcoa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxreqllu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2swymkiyv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gavsmanm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zsgyfwos.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2igjjonns.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qxgyiomv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2euifmemy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2arpzuthi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dwxfummg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2kkhycsaj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rpnjiolx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mythnlyj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ytghamaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reblagoj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qkjpknnd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2utkkcpdf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2udskajri.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmqjghmi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vkxqftit.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnxphiyx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vhvqgedw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wiqomxri.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yfimuzlk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2btprzhve.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yduqiwbb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lvkbpzay.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oneszapn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rgtrcnqc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mddaashd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2dexabazg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yszkiqgj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2trfkwaac.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2uactoday.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2csfhrfsr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cfwautto.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nqhjnagh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hytjfnsm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ukojaflv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tdcsnxtk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qzplmmfv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ikvcdpsx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jdretkrv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hpnrkhwj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dvgshhyf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ptmmxrii.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqoqnsph.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zqedfgpd.html


<!-- 参考信息 -->