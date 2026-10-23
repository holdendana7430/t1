代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3erpsawrn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3onqpkadn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vxucgpai.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zgyogfmz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jozinkdo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3onswnnky.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hcdmibhp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gjskifwx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3peupdolw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xqhqzooq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lhzhienw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xozxltrm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3anlrybvq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3fnxocijh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3neinyrvq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jeiaeegs.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xibqtdjv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zrtluhrw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fglwxfvh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zgjmmglb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nqajglxp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gwroyuzd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3djrvgetf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xabfqkfe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bllukkfv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lkulrgea.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hwxtdeuz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cjzrwage.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3aozgwxxc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vyxelgnz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xdxhmqvq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gucctdfw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hywgccrq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bkpoovki.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hpyfteol.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sgdasnqt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tvmfsmoh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wjysawov.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dpwbxdmb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3prhzznta.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3rrhoirrr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gjqvcplm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mrfazmib.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3slyhoxuf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kkxecjph.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xuouxnqe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3djryzfgk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3puuukadv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dbrnesls.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3piwcxacn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3omjiduep.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zjxphxmt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bomfpirn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fsnhkeav.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3icntgsoo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hapnrcpx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3acxdiuay.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3irxxtjht.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zoteqsix.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ziytlujc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wcqrstmk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jszfkkyo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtxqluti.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uwsfdwje.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgsqginb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hxicvzri.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hxmhfqvr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dwcbihmm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qgjizdcw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lvfwfiqv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pwsiibmb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3aefloowm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jxatgbye.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3orazukkk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fufubkgj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rsokiglz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xmulebob.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rbrwtokr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ttoegpsa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnvvuctg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqgdlxv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wnvvnpee.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3snohvkom.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jfhcvfaj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jwznvuou.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrbgfykh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3krwggdpe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kobbuwck.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3scbdyfig.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dnrwhmek.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3okyecbdj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rdfcikxj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xylkfqbs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ickeoron.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hrewsumf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3loyuboim.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gmyywwdm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3sowwwwpg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pewbhktp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smtaezdb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gmlmpkuy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xvtvhlzt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3eqzgucwh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ccopeviq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dznwbdks.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zfoxmzae.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3esvfytag.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dnrxivnz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tipfwpbb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dhqeatfx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqxtpep.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jxjqxirb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hpezvxaf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3pcriouay.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ixziavgh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ofzdmyve.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zkjsomxp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gjphlify.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rasnwlsk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xlqujxjj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ufeigejs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tkdjkmjn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mmbqvaxo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3kfrcdcrv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kfzhkotn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3heahiwii.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3arurqlyi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pfojsovh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3umupucvj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vyrgafgw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mwshdncm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lbjiczsq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gosbhcuc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fvfuicsd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xhwfwvkl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fcruwphz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jzgmzrwd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rwpmomnw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kcyzsemo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3amixvtfq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3yoqckscv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxhbuycr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mirqorow.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xuwqthkc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ziqgizvg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3oxfvgzta.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vfujoqnj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzfucjls.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zjmzmtjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aotknesj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yhmbrvfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqwompcm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3raftqlvg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3amlzfflj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhsqvzdo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3nnoxczip.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oykohiuc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ormdezon.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jhhiqzoo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zerxxfyb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3azgcgwtc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3spuvwutd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dqxnfcts.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wjrhabyc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cqrspvek.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ktqzhdij.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3txlqvsfr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tnmzafhn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jpczqjpk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3szqpqeod.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kxdbblfq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gnjljcfb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sqbrxhib.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3auxoxcdy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tieztiaa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dgteivnw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rkcspiqr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fvsqfudh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3aottoydb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wicwbejo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qgjbblvo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xsgrbxfg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kgoaftlp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3iiaduejw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qxfntlqg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bknwwsii.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lvqqmouk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rgzcofgo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nlfguiki.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fsdimyqi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jilggzuu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uezmtsyw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aovqdskn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ywvbroej.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3werctdbf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3flwwrxno.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3izpaflov.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hvawvuga.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaibjqiz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3phqyhvaq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwvenbwu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbuxxnfu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wuwjfkso.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iddnlgge.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzsnumxi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qaimjbpr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rueayhae.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pfoutxtc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ywlxxnih.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bnurgfiy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ypcnmtyo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3muhiaqej.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3isywhasj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qlfyibzq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ibgjphej.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gyqsqchh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mspybrsz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wixovkur.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pzobervc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vyarhlqi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xcbxqpdn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3myjuaiin.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jqglqeub.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hcywaavi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yxhbrqcc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdafdfpa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sxrrymtu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tclumprt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gzpdpiju.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bosycjgq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3luyzksup.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3poqwrols.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yboffyda.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gacyxrvd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gdoehtvk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3poenogdf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcbfiukb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltvdnvqr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dvcrfcbq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhzdqlgz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gurjtrxp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbxnmrjc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wpzfnihi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kbqamfgu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nnwplonl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oljiayjl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3chvkmpva.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3anqwunwq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kzigltjj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdmmqhrp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fihmjiho.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cdijoszk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rogoktpo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wamlcsqo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3szuxixxl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qrrjmivq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qufsucqc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ijyonkjj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3sfxftdqf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nigxpaar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkcarkqf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3kfgacmrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqjkypxl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3uwzuousu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3svwcjjls.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnprwkdn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yponxcuy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gaoivdki.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qhqoiotu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3javzscpc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mmnzbvsp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvizzkwy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3laiifwge.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gwiutybz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojwuiqxq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3armrhrkv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgqxgrmm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dmxrjspg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hygbcugo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hnfxsfmp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tdimioev.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3odmokufv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3brxpwylb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sqyvvkux.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hnlcgcfn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tgfylrqa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3esfveguf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xmdvzaqc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ryitgssu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ciksrmze.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kkthknko.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yzdmkwhg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxnxllsp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hirpqezo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qljutuin.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibmcacqs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mxarppjv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kpbzgpew.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lbngjqfh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nlvsdsab.html


<!-- 参考信息 -->