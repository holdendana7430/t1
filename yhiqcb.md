代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vymcodix.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hhzvcgjr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uljyswfp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jqeclezh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ytftarxm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vuppzimj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zitvgpbq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mdgskwgf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3sodmfwow.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tcbswwkr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ndkyxyxq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wcxbphap.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jpcycpfe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vvxfqkoz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tiebrxck.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zmhjtwea.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qiwpfqgn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3yficjhjf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xstwwhze.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gjowbduc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3sytwxgkg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rfhirzhn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3chdjbnrx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3amvxdlnb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xuavhnqs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tcxwxeut.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dbcrzeit.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ukenemin.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3imjxcljg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wiyyafzh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qetgrdta.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fnrtfgjj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xayqdckf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bmlrfxwp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bbvpbovi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3efcchyck.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kjszheiv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3papitmuj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lumjkmfy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wqnwydap.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bksqkswh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wlvxwcnz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vfoksthg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3fvqbsljl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dxppesgq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sxzgmsei.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3niaisplm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hygvkdtu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3yccryoka.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlqdciui.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pchpzpuy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3juifsxza.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwtxfwkd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3crrzhztp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qsbpurtf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nvkicfbf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3evghxdyt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3diararvb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rdljbzjg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jdwnxidv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqneaeh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bafldlsu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ugyrsjla.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3lhfpamis.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tyvjwoov.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hlnbbukc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gqaitlcc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uzmswgwt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hmeetmvk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3beizhakn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vibpssck.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzioypwx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhldqzm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kcdtcgfl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dmgbvfri.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3waozeucy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zozaclsj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vjhmbhml.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pzurixxz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rwzbhbzd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qctypmvg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3kwliwvpn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sltawkof.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wohuucgo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3avzaqgyz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aspqlqyw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iyvbbkpw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ddfimcpr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rutwpepq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3snwdxufo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jcjiirzk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qqjzpdoz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hrwwrkzg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hwqppijd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3lmxosnox.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wiojqwco.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vfyrocwd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kewxqfvy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zipbjlgp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3puhrbduh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3tqfrfmfq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3drxvublw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xgmuxxnn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bbwzuhht.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kbmrhdjz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zjzsptlq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iexooxyx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pnxaebwr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3bcjygqdf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3psbuffrb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3pnwgznrn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gxlxpmad.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jvaywrvk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3areancxi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tevblovh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3leyhxgzo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpwzipxl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tlutvlca.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ibuaqucw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xzefznqz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mvjxzqpo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jdjbjgsh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vfkdqqpq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yhbxvzvk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vdysomqv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bbnozcgr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yrowvnrs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fgwemvmv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vyrvigsx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fjpzyqva.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jhdjypby.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3porgdsqo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ejbhbnpj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kpubhfgs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3srlojtfr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dmsgbnzl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mlhvktpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysczbsxv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vzxvbsjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwcssoui.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzptbagy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ehizcrjk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hghhimvj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3lytliotg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dxtlwcyk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fslyexje.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sxzcnabb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imqdrfks.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sfrtzeqm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lyclvzxz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3allzrzsz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3yvaeqdmp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzmrmwvd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgjnpsrn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sjthauuk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ewkbcjbo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vgcumuid.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhgmisol.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3osqaznxp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hrntqjad.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wcvxgpna.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hknjwnxd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xrhbkfev.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ncgchsuo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ksjqflja.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3afexpuxo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fkzmrsde.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ijmdmfvm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3glkkyjse.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ozksjtxp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jmqadupz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jdyrggnu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vwuaqezt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rdijtkdb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3szbvtldw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3psqmakph.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3guztffxh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tukchxhb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wxrcaabw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awybogne.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uspcdlff.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qvsihivg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rollrusq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpehfnsd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzvwnyot.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pvneikfg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svmeadwb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zmigyvir.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stsdtzfw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydfnmjgv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3icycimfi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgszdzjw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3usespqnp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwxcwvnt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vzdcfcgq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cviyjypw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fzjqhfab.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3srjcvmxg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qgspqukj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lhbwixdm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3mhubkxyy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hfpbqdjp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3uicydnwl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3iliflomv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rplhxmqy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3unjtxmsj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hhpuvnnb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3favirhxa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cyrglnge.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bvlqghxi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ixveuvxg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fkksqjaz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cydqbgok.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oggmfdkx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mtfauivc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mrvkpxem.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bygotsaf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sxixaxrs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xdkffrpo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfxpwwia.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jodnxyrm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yiejekhv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnwdawgy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pbxhmhia.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpktdasc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppyjcoiw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zxsfnpka.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jubhowbg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjirapzo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vaessrnb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjyvztay.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3umxtztld.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uxczsedn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azufkskw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdfnqhhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vrkjmzkn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pnzzkzeg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwytcsex.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xrircckq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3yljpstwt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ugewvuvz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3oduskust.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3okwpgxny.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3uzzopqjf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tcaowzik.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mtlpxjyn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lfyeadnm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kpouqnis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwdhjzua.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dfnpporf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glsytdfu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tcsdrltb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3swskhuvz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzmnuvsn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejnjnuuq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzckysyi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmxpktih.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3olcsegey.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3erioayme.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zihwuolz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkyrunwu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kwxgtdzb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeduxxcm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trurdcpa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uoowavhp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fvvcasom.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mxtlndlk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qinoibhf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkzadbmr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rnjwxneb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3njjcpwxe.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3beoiccrx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yaczbgvf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hofbjdha.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3quiddrip.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ipezhasp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vkullvbr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ksqegvml.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xlhygsjg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kwfkwvhw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgwsekjl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiwnepzp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdilbcnr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvuadfcy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nffrzzee.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wfumcdbh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dmmosfle.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cybcgjur.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dslyjgja.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vvfxysyu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sfcwjetb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3klocngas.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oipawjwl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bzfvaeex.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ahmexutn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vmcktmws.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wwcrrlas.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xyoxbutm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iqjxsomh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aqrkdisw.html


<!-- 参考信息 -->