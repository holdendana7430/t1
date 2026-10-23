代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3teqzuafd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qclubkcx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iccdrpao.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lzytcnly.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gdarzzgs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mxvjmuql.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mjmqxdtn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3etkbnucg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ypqxkksv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zqbajorl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3pesadnhc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aegupkph.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ypdzxudu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3lgdmglce.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xbebgxth.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3klspnvrw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fdrmmdbz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vujhauxl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bumnxsrj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wagdicql.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rkcinryf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vcjlsfyo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zxunlqdr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bufazosm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uiunzznc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cvyagzfx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jfdzblcn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3crwpmklr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3iffekgaz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xlsfdrbt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ipdcvvoi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hguakzoe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nnuceoul.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bwbdosso.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bdrpvhwj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wncfxfwr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zubzvorb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvtsaxc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3otiumeww.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ugulsmyr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3glkumkje.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zlopjpqv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lzkexkdj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oqpvcqoj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iyctobip.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ejozofij.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mxtprdwd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lyvuirsh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jxdsnfbb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lheqebzx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cysqfvkb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wooxadrp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lnwqmdfw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hcmfkehb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bpcpinrs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ridwmsru.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3yxisbbsv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3anxmsezg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fkbeetdr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ybmouzzp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3kusluxxh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzvjbfvq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oopgiaab.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vffzlygs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lyhkcbjl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3twtyoseu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pywamkoz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oipdjjbz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wlwhhdve.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mmctjebf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fbiqsvff.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qjkrpsdp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yculwrya.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jwkxnmkj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xgjdacob.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3isablqhh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qtexmntm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cjmvxdmj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3trnhitjg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3oadrrnxs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtmiyuok.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3dulxaqzm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vyfdyora.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3nyikmyqa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3idswukcj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3armdzpmb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3owvmxaml.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xmejjdey.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3qoamfnoa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yldkyopu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rirnwfjh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3urjeabry.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xgovykot.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3frsyksws.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3cykgzuon.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ddmxsgxj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uyhjhehi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhtiulqg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hqvcnldo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3phgyrgjj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zoirtyvm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3auvdqycl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ovhwquth.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vaxexcyk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dazhqbcb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zfzehbpg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pxxsmdkc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3czahibgo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qijschoh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bbwfylvk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3krpmpjax.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xakpgjbv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3aovrydnd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3voahmcuv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3srlfopux.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cigqxnvf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dwttcozw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ohkiocwk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3raktfcko.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vzhxddkx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xegprzsl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3fjnatssk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3lirqcxza.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ftgqrjbl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3kcozjrzf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gntfxthz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3oizbjzzl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snldtozd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3oekcphme.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zrftxxuo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlmhagto.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xreicsvc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xnjggrbz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uoqntjhm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hdlqdhwx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tysaumpj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lzppricb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3atzzqcbi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kaumbrgr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ozgsgqkd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3knribrdh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nicauzvl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bymgqvju.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3luzvdixj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3raonvjua.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3obwxayhg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bgefgzpu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zhncvtwm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vmzkjibu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbvyxtrc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3idzkktfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxiaigtw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iurdanhh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qoetffsp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hwpohfdz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tbzyowiv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3usiykeis.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kfahgxrs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3mfxaonvb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3byfmqpkp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dnmgdfpj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdydkldf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bryujfdi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3laswibgj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ompnkcva.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcsmsjgp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zccfqjuq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vlterwxb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ustvfjjg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vdkxatev.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xbhizrbr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3weetyobo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rltdoxgw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gkoxqafu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qkuiwxhz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nkghgpmn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3arlpkglq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wpokenbw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3owhayifc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3dwzvcahl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lciupnmo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yxworrli.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bpuunesv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lplzlmmy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kgfcvhwj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3udivifye.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hteqfomw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ycelropa.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cqaaqowx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qpseyghx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yxtkxjhd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3izipaozu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwwnvhse.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eyjrlplh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mvjuxtjw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdnrndfp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3syqengjt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3babpvxrh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txeahqtm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ihycuhht.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nedvmraf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qiqrabyl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xxdalnwx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfnuqwrk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3enqpxtxr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wodwphnz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fjmkwnqz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tncvbqcj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xorisstt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vcgaqblp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nliqklzy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mkhqfunb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3eehdghed.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3soaopclq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tumpmpcn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3daahebau.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3hsasiyho.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmgljans.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3komaedzh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xtasoqre.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mpoprgcj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kznomzwa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ocgevkyr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zvcvlyqj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ycatsjiy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gsddzqim.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3juzqrheq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bmxftpem.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3znxkdaur.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wtduldlz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3bqlullnb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eybsrnge.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qoxnrtdx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3thuqjmng.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hziexyrg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ybmyddwc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eyqktgnt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3majetkkh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kdhndiaz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkrxbiun.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpexnwxg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbtpvoth.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vegtffni.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnccnobg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oawrfpag.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udbpnvss.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgkqttgx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bfhcgglg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mkewscjq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dpbbvrdv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kqajbikd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ftiaphqo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pmerqacj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xqyeaiqc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3uewtchhy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sxigivce.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ncvnxxwb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3frsustvs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lxvuwtma.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wbywmfir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovpgngdn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jrlrvqww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aorehcjp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3evshmcmy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3zeqkylgw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbshxahe.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sufpzeci.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3aumiygfi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjkomzzr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wcgnhjpe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tgxfxcua.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgxbyfvz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qyzmdedd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lfamhptt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovuyaubq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hwbrslhv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rabjhcqo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3butydcwv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mwweagrl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pxvpmuyw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qblkblti.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3izzwakjj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ngwmcvmb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hlucgcmw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pqaldfzr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lftvdadg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hfpaltji.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cekvvrry.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gaeqvpgh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ytdajmtc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hrubtlfr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sfdgzlve.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zettqkqe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmyqbdrr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lvkhjdpv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xvnniieh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mhlwecpn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yugjhwpo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3danpdqfl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kgtkpmmw.html


<!-- 参考信息 -->