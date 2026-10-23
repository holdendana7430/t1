代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ysvxpzjq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ivbhlmvg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ndosnsns.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uaojqpoo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fcrrzdyk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ewsqbaby.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jafrkbyq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ujldciso.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kjtddouv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ivnytsju.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xukcgvkd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nlljwrmg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qnahpysx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jsvmovgj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dotnjano.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ubdxdzje.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3donhvdnj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ixmwjkmc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sdgoaqtl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bijzhvbn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfjekuba.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lcyhupry.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uzoqdojc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vedjbnzb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3equdbrjo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3uivzvrcr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ywxvxjby.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pjyubicv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lqaddivd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3npuvzykm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mcwhufdh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yywfejyy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3punjcltu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xwzwvezs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3alwoercu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3knrzgdum.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3aepyazjr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3muuvepzj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3friccqkr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cxzkletq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xbvbjcjc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3huvuwfvn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kabnbmnx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cenzrfkr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3peqyahta.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hghfrite.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3oxbpchhi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lfvlomhn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ktwnctcc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kugzhfzr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fsstraob.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ddunlscu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hcoufuuo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qmtsmzod.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3aqbisyyd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jalireqo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3stiqicvs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckkjjmbj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3onfkraam.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciazcwnw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qnkqtizk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cycwfdbu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3aagqwmmu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iekhiptc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3bfjsowxc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ulyboons.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hnvzcrct.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jhojywab.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udieyzkr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3endnjrxf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3esvdxeib.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uksmusjc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mjhqvvjl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3uggnajqv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyjlehto.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3iufqpbjn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uohzaoqy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fmnmrxlq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vynhzwxr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vjmkqauy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3tslynntq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vajwkqfo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3urwmzvkq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3wgleidsm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vzxzedjb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3aqwudqog.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zccgrgdr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pdwfirra.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cfkajzee.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ivnmdjep.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ajeaqhfz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dwcpepwf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zzryamgr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xyplrfgw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbpxyhso.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbzdker.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbriuytf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qtxtenvn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ygjbsuzl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mwttmzop.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kbzrrzxt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3wzixlnns.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3sfqvujbi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wgbvenwz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nmthjgpy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uhtwcqzt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dzjarxza.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3szysuxem.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3eaiidgqi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xziwntlk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3cyweyppv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3smlcduea.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pykaeclz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nlztzlba.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qhzslyvg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vputgqqa.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qsmeeycu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3eussrduz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cwpmdxue.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lvolmfum.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3uuvajkcs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3entysiko.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vmpnigdd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rhvgbcew.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3umlwwgcv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zjvfgoak.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vtgucuyf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xmjtnsqf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vcmuuqcy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nfbqydoc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3foqrnfvr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kjklxbbs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zobvnnxo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3yhxexaov.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3efaufscg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yziesete.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xbfmydmd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3exyabguv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ffkfmcci.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zhvgwfgq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lpqtskqo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rhejjsfv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gzdoevfj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lxqctivt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hwmocknf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcvwxlrr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wtbltija.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmgvlyjf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3psgmfslj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vlxxyajh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tqyesoow.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3esfdejfw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yricmqcn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3stkypxrl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dbnfgvun.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ioeqshxx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bwfuctur.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rvecvqnp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3kuiyklde.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rkotxnkq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qalnzrsf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpiruhdi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ncbmnfuo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zylvpltw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3crziovxe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3typvpfzj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3quwnjvys.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ycodfegc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3svwpkftp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nolsjyvw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wbyahsds.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dflnexsg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3tnpbbvwc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xzjlbkaa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qslfvhpl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yegfrlgv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ggzvxcbo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3jwefrgir.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3blxgeajq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vbtlxwgl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kxxorqme.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hpmqehkp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ftiwqsom.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nzdtymjm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qgzlkype.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3voghxvxr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zqbsuepq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkyknvgt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tezilyqq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rqcnqive.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3foejextl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iawhogmg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omdtfnua.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3iygvrftf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njypbvwy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zdxjrawd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3badlfmdd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwmtanyn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nuhdvomq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwkjuftg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqcvvvlj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jzpxnqxe.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3szecwqme.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vvszgaoj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tpqukuqu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qmrhiazk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kbjmknxf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qlovyosm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ezgknfye.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zfdnaavg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gxowpzkg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3emrmnfgx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hffrzesa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3umurvbge.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3inmolkvl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qaplvodc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ndinnrjx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nayklavt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ahpjcqpz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jelxpica.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hcbwxyxi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzcdhiqe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gfekjamo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bednncly.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yxoyblea.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eelwpctj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lfjkilpd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajcvwnkb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xnacqlop.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nawzurme.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqmeenwc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gaqtnkqu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttykfiyb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzvidfec.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ussxvafz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iscizueh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tugywgdg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqvzggqp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqgxuknk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbkrmwqp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zxelostd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qxhpihjq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kiwbmovp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fnxxamza.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fcdalqwl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kpndfgax.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ixqkstvk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dlzoopaw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pnjkecbx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zgggmpzz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3kjbbilug.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ukevhfiy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wtzlpgbs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ddzbgrpb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3sdxmvdrl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zkfzqilz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnklvmqz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tozeiuva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmkoauxb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tpqxqnmp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uepilupy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3twwlcaqm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cocfkzwi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uoyioaij.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3gvbvocbp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3halagxxe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qrfdqgrj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3anqnuqpz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sjpfwizr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3govvwcfv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sepnvxev.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mqcnxulc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbqxdumo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nopmgkbm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ndupggay.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3nfphswzx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3usyjhctc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3oxyfjpqt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lwxqxosr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bsjxbhll.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3blkpxciz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fuokfglj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zlsxhzhk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hgoephpk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kkgbflvu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3agbwhacb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3auuugktr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vvmozter.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzxxgoin.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmwcgcgr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpopxmuo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gslirfde.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aypkstha.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pbvjnnqw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gvvpnkvm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3lirhcucb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qcurpabb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mkocxnum.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdrefpkm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfgwuusa.html


<!-- 参考信息 -->