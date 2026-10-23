代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3lmprhpfo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bwpyfhcm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3onabjpnx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rlpdaxyg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xjlorfow.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nnrckwwa.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3azholdmv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ojtwnxve.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3trprbkns.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3vlrqstfk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jslttvpp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3euoqnrof.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3debesyly.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qhfbkmud.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zoapolqy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fmhrwbew.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kesunivt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dqhuydfh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3orbrxngk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qgalvmej.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oibmvmvh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jwpjolea.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pxlhpipj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tabyucyq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tpaunhoq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ugqbaacu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jfgwxyes.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vfphxpzl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ggedrnho.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ecfdwdcz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pxuawqyq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pmuftoyg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pwwbhkwz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sjlmzlai.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tmdsqyxg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3frhsscms.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3oulcmuwf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wqhjvofg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uxyuhruz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3eiyiwjre.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3papstvlg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gekntuga.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3tygtypzm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nmgdpofu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3biomycct.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoofukrv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nvaxiqjo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ambphyte.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qksldpxn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3cfymtmcc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jpptyokq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xxtafsgq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3umvbbygr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qcnicgjw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qeohaxio.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3plcceowj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3djhsrpvw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3popyiqhp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bsafqonx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3seipuhxh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3anxxsflc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dlfclnrj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3veokweyq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zriumpei.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwnkkisi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3doulftai.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3envzaeoa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qzlwrcha.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fcyihfav.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gupiykbg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3twfzxael.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eekdknxz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yfzdvnwn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jpinbhxk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dlukadtr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yonqsaxs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3lzjguywl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3imuxwosv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xykcqczl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ggqwxvci.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lgqfyvtj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uwzwxubi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gjjxgnlx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qdebirma.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ihrvffzu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mapuiouc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uolydgau.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jwftujsz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xfavwkrr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3onpivznd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bickhgrr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ezgxgegd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pcftjwsk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3idylbqnw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gcvffoso.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bttwlltt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3onyvpsjs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wlgnvqoe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vvxblykp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwodpwkt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3slhghfmf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3caczgcby.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nbpkevaa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cxjejket.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3upcysjbp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mpqhoecv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3yqyxcdqw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3awruzbdp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3lshbalbx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xbykzmvz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tmjjdvoc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptngmcus.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qzargfze.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rqqlefzz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hugymkcv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vjkpeijv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wmoagsbi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bhgohzwv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oofjvphx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wejaxyle.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zfcptioy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3nwjguxee.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kswppfkv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dshfpgob.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3uapnsnsf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xwibbbwe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3djhyppry.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3olcrgyaf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3huoqzxyw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wxbvgzuq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3uoofwusw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aswhkbtp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xjbewvtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkichwst.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3owbpgjyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxpvmwmx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3auqnntyf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ilswxwrw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xrslwntj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zpkbgbfl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fjrrytpb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vcpixfyp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rnlhxutp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smgqcekt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dtukgdlc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qalgewbk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3iuplyvnp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uipbskxq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otaojmmk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjwpucxn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nvidkjpy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qsdvnybv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ldxoufgf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3dtpmgdlg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3inqbzgaw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3seswjnfl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3txrwmjjo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vyevqywv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ilihnaik.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3eqzlamkz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3kyldtqua.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yldarirs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uuawtcaa.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3oosjssyc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xurkmwgo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xxsnazwj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xonqsalq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wlayvdmh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xwptbtxh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vdnzrlda.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fafkozpj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fsuhbzjk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jkcmrfpt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mijocjgj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qjipsgwa.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wpxbfajo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lveanexy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pbfqztys.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dlkkznys.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3utbnzcys.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khtbdclm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvvietpa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkyxuwqk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nvrkytqe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dopwyjbd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbfjgvnp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3msewaifn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggxdigfh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lnaechyu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ctuonxtu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dljergqz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gkrxrlqr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qjaoqcjk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xsdpjcde.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bsltqvbc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3sioerbtz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ibxbiuio.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qfsxqshs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vdybmqpz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3diekjjpm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gdayoqlx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3memwcnhf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oobieetg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3raucfahx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gsalzfiv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eclwrebo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vgakczdo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oiowxekd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bxymahdu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihobdemn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bjwliily.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jafeunzw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tazepnsm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zpjgyhjp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wrujnzii.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yulfstgd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pamwphru.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dumyswhn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhnsxtjb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bqqjfrkw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgelwfqw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfrhtbjl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mihdaily.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjmhmofx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbhsxksw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtbifomu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ntvglchw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emxwdtjf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wuxftidd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrilfcww.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3akydmbpj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3exbznoes.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3cocmqgqd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tczmemjt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3pophefwk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rrqjcjwj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bfxmzseq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xeizgbok.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3esuuuist.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ktxwpyjx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vejfkxij.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3locgojbu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3elezvtoa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ysarrhuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnynvlhm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xzjffpho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xoeuffhy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gdbsatyn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3phhbbmkk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yusminiq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvpedskb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3nrxqemch.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfdkawhr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ulkzszkj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ezsueqlq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ntnytsox.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3klmhfdca.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ujvdsiqj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tugfogbx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfpoidbm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcwhutqe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pgivbyyg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wjnzffaw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fdtvyjbk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cccodrgp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3uzignudk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pjxomhom.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mysabqtx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mdzmktpl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lijsnxqp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ceihqcrb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uxprhapm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mtcqlyti.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wkvppdlq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xeusbbrv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bnxnwcqi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bngfhncv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mnigwyeh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cfceqyam.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aearziuz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yxpxskuw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tublgmhr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gsfxnqsp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zppfpdja.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ijwnhaqi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3huoymprq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylrybotn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xbtlpccy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xfjmcvgk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rrwyfqxy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rnfelybe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jznlxvxc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3guujclxz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3siyoqmkr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yjkwquty.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qcrbqxnd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nsddzzsp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wkqjohbz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vdouqvip.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cdcrqfoy.html


<!-- 参考信息 -->