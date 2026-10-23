代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tosduiov.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ahcxyedn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pukyogrq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlftxcqq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3epdanqjv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xbzswnfo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3lqpcqghk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cpnmbvih.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kiwbrjge.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3khecntjq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nqzumkhv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ibnqechz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ndieaigq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3teowlrwo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3phdmckjv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3aujaggxj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tcbivddc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jlocujik.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3stgejamo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aivxzfmc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zliyrpzc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ppssttyh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3llvzcwxh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mzqwaenb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3smbejrpr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kyfqqptq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3nfsdtnza.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eqpfmqhh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ntlicxyo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qtqqjhjg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tumdhpoo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dnegfheu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jsbsdeqy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fyindfbm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zyraqqku.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jpzuhhfi.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cznfevro.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fyhylweu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uownvoph.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cjicdigq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jtbwheqr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bixcqovb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gjcylwip.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ndwbtetv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kinczrek.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yfbihirc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xujctcls.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3igbluyzk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3pbxjycbi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mjdvklvy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ihfzmhzg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3momkzpcv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3aiaeaidx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mumxcgmg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hirbtcpe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3phizhymo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rbodcjvn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3llalqyxa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3teqazxdp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlttyupp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vwcxnzzd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gcaegdvw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tntyfxiv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3neneyxsa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtrfrub.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gfwoozwi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jeyjkojo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vucoktei.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ubtotfrr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3htdtoehg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mcrudqec.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3migpexti.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ypvgwthq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nlnbtsxp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vjuvvruc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntpbetwl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3asncnodu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zkwojdcw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kgsvumto.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xgpnkohu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ttnrwwcy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qmghckzd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bbkbleir.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lznvbuql.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dsneecqs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jnwidyqh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3xtjxphds.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3nfywqtsh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pxvdlqaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sluxrwvg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3barsigdu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lwtaksvu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3frfvssyo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wrwtsgqr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bsliojlb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3veermeyd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gutohapb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hzkanqfw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xqgeujcf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mcljsiij.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eevhkfjl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qbohxode.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eurtrbta.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3onvxgyec.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ujixdvvg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cqkyqrpq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3neksatzq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3omibjdpd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vevgiamv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rblowtug.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iyaqbvba.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3emvaqayg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vowsggdi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3imdiafyc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3sywdwxgd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jzshdsmm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cqpuatlv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3koquopem.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fojqeoat.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ebcwaoiv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcmqxdbz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3suqutqzw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mjsobsjs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vvfqjmvb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sbqzdagh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cxitujod.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gqtczjiv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qffauhoh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3alfmngyi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pyewjbzc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zwpzvylm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gtnkgaty.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fguukbzi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jzchwrgy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dejrrweu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zxqttgyp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yqgtyssr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wbbilonf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3avezuvyd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yczakzpa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qxwecwid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ligzvtal.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ndffykxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ranlxvlb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3icpbsulp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wtstdgqb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vkowqlfo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3npgedmjp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wamqkgjg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wfexcxmq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vyylsypz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqdvdhbr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zzqvnodi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xspkoioo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pbmcugoj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvvobxur.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rwbfsvhl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pzrmuudl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yoonxdgb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hpbmnflr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xregqpmx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3stjgageu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wrmpowru.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bgrzcdfy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dknahshg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3axwnwltj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3crqrpwfn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3scwncgrg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jcabizxj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ratexjwz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nkbkczse.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvehbpuo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nxgnganl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3jrlucyjt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pxoijvhe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xwgptmwk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3miohxmte.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zjonqaie.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3pukilnps.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zxkhgxwp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dmslwdyd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ofyimgdc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rxzjinvv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnonvokh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opiesxvl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zdcceabm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3gudugrbi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tlyvbsyf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlnhifmm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3eeddmefa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sncalufd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3przszcll.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udbvmszs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axjomrmd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ggvevojc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oeqrmqqp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnusnglb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vqtviwnq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nbflwwfg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fabmayjq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gkvdfizo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lxwdtktv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lvptiigc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qlgmegdu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vgvmboge.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xdvzswnb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ttampisl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ghbqitfz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3pbmuacyc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3igydzzod.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mgxzmkln.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sliiglto.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nbqgxywd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pmigbhio.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lmqjejsd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gvzjbwqz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ctuhegla.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzkldprk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zevpwnai.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tblculvx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gwynvvis.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3smvskhox.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bfxqbzqu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exptarht.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xctmdmmz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vkeqdeic.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svxrjlgs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vuungcfa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgcucdxq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocqfvxbu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fcnfthur.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3moigcgwg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocdemtax.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjymclbj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3rpbjaaea.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzhfaxtb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xirgmfop.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3symglcaj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggfkyahz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kzlkmpgi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wjoxisaa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmhclbtn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ficllycu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jqjpambr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3suobcjwq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3aeqwqxoi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tvqkemoz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pdnsquyi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tbkfznmb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hcafuekl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ptjlbuej.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jvabkocx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prmadrxz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tjmodyyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnccpvdf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vnfjaocm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3lzfentir.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iljechgt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hprvnsya.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sdyhvdpy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3slivptfa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3siutwcbu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xcycqfnw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbynfpax.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bwxrynen.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qmrvkxvq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3pxsamado.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edjrlbkk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ugqaoyfj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmlmmtco.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ufebkmxj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvxnsmsv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wqxfxaee.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rdvqrbxa.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ddihmopb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gezrpkaf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nrucmibs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iqkuucvz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3medjpvhr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wbvzrrkl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vivxkkvm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ukgdnkll.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3neiemsti.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nivbmbur.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdgnysh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqwqciro.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3arzpfzym.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vchqzife.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vigfegiy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkriihth.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tmekjkkg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ixgknges.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tlnovnwi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qisxqnzb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ungmtztb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3opbnnkmf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3birzlnoz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fmwhtjjm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3axqeomca.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3shthojbj.html


<!-- 参考信息 -->