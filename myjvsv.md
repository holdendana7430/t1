代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vwyusgtl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nwouvwuf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3idscgqrr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fcyqmkzt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3shplheul.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kskrgcon.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3smcaevzm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3artutkle.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mtcfrfpe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yqscbzyc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jffnxahg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kdbfxghh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ytrfdxca.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bxgxwlls.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bjfzdzlv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dqhkhxgs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ugvuqoor.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emxatkcj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uknyorfy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3muanegag.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yrsbjsoa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3itqoihgt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3dyzcsqlr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3suehfdzy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xalxyfox.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kxmstcxv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3effswwqf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3emjbylfp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mscfkhkv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3auoypimp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3axapgpqr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gpyzeyqj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cowowsfj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dyjfhxpx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3dzusvebe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3boewzgan.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3otoclcvt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hbmynouf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rcwdbdqi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zojfbnpn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbxxjgcd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pbxujokz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3psggatob.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsaugbnc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zpejfbpk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3obhuzcnm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hwlkbqiu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kcgugcno.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkygkysd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hzflqtjt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zsqeuipm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uxtgengq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xlguojno.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zbvhcsah.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3aeczyejr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wuxceslb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pvzyxfzn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xhjordei.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gnwhonid.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lalweqqv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3sqvjyria.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3auktwktt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vcezzgyc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xkuqafvx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ojxdqlll.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3eslsitxl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xldkpvmm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3icckrquw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kobkkjar.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3quqifsxr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ntnwlgzo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ychlbimm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wwdtrjds.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3dbcxxzme.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qybnpqkv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tpztdcbz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jlzaqass.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hvrcjbjr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lovfnqfu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3alxitayg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wrrhkcde.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tekfbfuh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lfgjzycq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ynzpuzyc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kmvzcijt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yyhokind.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bruxwltf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3znvtqsjn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkgzzmna.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qhcjgksw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ecefrynt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xgprvaox.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hvgrdwzy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dycudcos.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ltamyafk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hzmvychj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ldiqoajz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wtphkdgs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yipxrtoe.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kfuimajx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3frgcrxmc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gtzwtdzf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3haumdqur.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fewgkwbp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmizcuro.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ohvxjrwn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gecjrjwd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rvaxmmqc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kzyggvuo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kqnmmkyf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vzqfqruq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ksngberc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sxpkxiju.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fnzzfuih.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eozmzpwa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gjewwnpj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3xwiulkxu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3narjgjqj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wmxhotkp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3agbyhwom.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bpnjsqby.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ogfudxhu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3uonklzji.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3raxdcwkx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mhdxpalv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwtgzpht.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dsggoljr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yekzbdfd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxkanthf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vpxuoahr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3izrjfkft.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3oreqwhtu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ifypubrs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xgaxizcu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3arodelik.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yijoeryw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ajfzgxjo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jaoetedq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gtyzupfy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoxcmjer.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhgqfkbk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apiiifko.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kpsacegr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pqamzrbp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wnbmczgd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qyflbjvg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ehltkdlx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dgzxwsxv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jetgkger.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vjdliqzz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zdnsxsit.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wjfcnvqj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dwldmfho.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uaoobyle.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jqjggfaa.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3owgzdemj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yloykqlt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3dnkwxqjy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rrlhykav.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3okdhwiwx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fupkdnyf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ihkohbtd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nfcqhyqy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3vnpdxkue.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zhmkqljb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3veyihpjq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tscjxoqa.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxiyftst.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uomknewl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ivfobbzt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qcscqcyu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkucahir.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txqnnebh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3osswqydi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhrvtbgr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xyxzgdcl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scsrwxcd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3neficrxs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zjaabjiy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3arudzcnm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3clsfarxv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okfcunxc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3relfhytd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xxtpmtug.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bjobajct.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pexxozzo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3memricwl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3afzvchkc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wixluhhb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3awazefnv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3apoaepsv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xyiioqpe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3slzmniip.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dsgkyotf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ovjmnqaz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hzbsfzii.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lfdwtote.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xtagcppd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oqracvnb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hjgkicbg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rzntlkpf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3riyufbzz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mpryzmyi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bqsajbww.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fmgovlbl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3casmdhav.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xdgohqhv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfqurtjh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qnvtlgzi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3slwgcklq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zflxotga.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uyvgdpqz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zmwajzha.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3leraokrf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3atyluegq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdjhvsmm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sbnbokkk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhbqleea.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3phcwngxo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ciqvdxma.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ehfkfoto.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3raukgzsu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tmvwxjlb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zdjefkkd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qpyosins.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3esnhefoy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rxvptpmc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3yrlkxokb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wtgvkquw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ztzhbgjt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3slgaqafs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bvpxexdw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3lnrqqkhl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3qubxkkya.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ltpsaxcl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pwfhudpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nntvmegz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tccfnhsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zanbefhr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dlhviqeq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ekyqddds.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3veppfdbv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fqtwtidf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3elihjvak.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3takxrwty.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oetwxwij.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qchckidd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vntizxdi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3cirrszqh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wbloyzhq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntqsqtwu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yctckfdq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wyekmvya.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lohfkhbp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3txgtvlbq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hxdnhcjt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzsnqcos.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dsaywrts.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gxbrvita.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mfvrirno.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tmofttef.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dqugihjg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zzdzwywe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xxtkymet.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rimgbjtm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kkpaorkw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3czrapvga.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gzysooli.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqxzlppl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qzgkxkks.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fpjlsmhp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lbancssa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fauxuxed.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gafcmlbb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jdbwqtsi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fhvrsznz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dyobugtr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtqvsktk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcrbtwev.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcuzdplb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zxdetilk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pgbikhqc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zovfhzzz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3znngbwjr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xbwbfpqt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ornihqux.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3upwfwoov.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdwslwzh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioozvceo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpwzzlbh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xvhwdnjt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qkooupkl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3melmskuj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kqjrzyrs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zggdndri.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3crbkmqxw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3guwxqekn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jidtnfsi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pwybpaoe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xmmigdeg.html


<!-- 参考信息 -->