代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vdprsdwj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ypcskhmx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ipyiifnz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2csjxwfrj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2noarbiek.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mfqruiph.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uoxvfjzw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2spoyhuca.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sfygheqx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2sqtljalf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2onnlmvpj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dzldivaw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ackmcvaq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ecihzjux.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vynadpje.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nlvmowzm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eeisyhpz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tdgvtnea.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wadnxrfq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2avuhcxzu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2gjxoiyzu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qtqyxxmy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jbcwnchi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2utgiumie.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cgvezcim.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uajcxqdp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fltekges.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yaoocdtr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mcmcijke.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gvvcxrrn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xunfahvt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oxofmlgo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mqpjskra.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eyrxivjs.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mzzixten.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zoqdxdla.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2quojozpo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zuzjuwgj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2phbogryg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ygegipsm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ulpumshw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzfbetsj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fjjzmadw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2whhiiqwz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xkkhnkfk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ucxloekn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2utqiuilo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cchkrwmz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2iaijvesq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qemznltp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgberpua.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pwkiugqh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzedbtg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kpjmrpve.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2syfwoxas.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qhyrhour.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lzzbnzvr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2lbswhmwy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2uphedjyg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kennzejq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ciwujnng.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2aerxmluo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ebwkybjw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tegmtzmk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2odekavlt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dqjkihab.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nsgvghzb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bgehcxdh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nihopytx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cwrphafq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sqdsgkhx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xpqjqzxd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ottcjmrv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qgjuwpri.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fjxmrqzw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jhpxaeyo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rgcheqtb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2muqiqpwn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2poyhvfjq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2frsaepho.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmwefzpp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fftfevub.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jawgyopk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wovfgkkm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wvyasgil.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wycprumu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ujqsywls.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ihctckne.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tommlcxp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ktxkwwug.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2njngnjcy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2iemgylfr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2snsgvxae.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ryegshfi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ckvecajq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwkbumnl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rxliwofm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dsaipxkx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qgojibyj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rmymfmyv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2eqjoqgtn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qkhfhaqr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2tforgdru.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jqplewrj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2raeeikli.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jausikrd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bscylfsn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zdkugshl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wthikgfd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uphxannz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ihshnmjy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2nvvvnasj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zxthhyen.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ymwquixu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dbwtiafy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2trlcdvnz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gaaunrmk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ugfjkmah.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cvvmoifn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kmiokctv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ubfzcniy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ktvfyquk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tfiwnpvu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jcekwaxj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bgbuwcfb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2celcbabu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ucsrhqag.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hhcemdah.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gddiecqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2repasoqh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jflhhvfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttcpuhzk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2imkxfram.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hftcmirp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eeqberaz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qslaruwm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zqzczqzh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zopfmxqj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tmblojmz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwowwkam.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2llunecwg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2eopucelt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qvuldtlt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2diwnlfyz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gndfjjaa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2httlxeuf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jdktxvda.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ffpqxecy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ebgdotfr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zzffyfcq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2whgsqico.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nwrtolok.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sqdidfmr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rgauwzyn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jqbcxvke.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ucvxtggu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wwexzzog.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bogzqprl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xqolmsyg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2frizgjdz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2myoxkeit.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2eciwggbc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rzvtbtjf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lsjtdxpg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bfzptmpu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ijcigvjt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uiumrpeu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xbmpxxsc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gbhtitgs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tasqmqax.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ofleqiac.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2insbpvhr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iuisajez.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzaveznc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fviaxzpk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kekpgpcf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vlvsjzby.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xnfsmnpf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2acdgjxkh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2irsqxucy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnbvqlse.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcabangy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wiibzibv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2soruncuk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvesquwg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qyspacli.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lmxntziw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ymlwaadu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jzexpdyh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xlmtnons.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iopnjxec.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qesevjja.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tggxxmqz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2amjltesp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dqbmbrsa.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wkhkxauj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vmqfuofb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2olikcigj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2acevqemq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ahytycxw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2czeqvhci.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bjnvdfgc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jxusuljd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xzdybxgb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vtelfizd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lwtelpti.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2biglmbfk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2btabdenw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vfbkviad.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xcwsbpnw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xiawtgxw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upclrmql.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rysjpcco.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ztbyhnqq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvxwyoah.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2prykmlsq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zyqzfzek.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkqiuocd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ocwhneox.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhgqwqmt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vynjnqlf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gjzwajcx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhkvrjey.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wllhrgxe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gasygslp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmengdik.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhmypiyv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yvohwjql.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xcugngcr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zrdkeyux.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2diwimxlb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rjgczxsv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2szcyoiho.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2vglzymdd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ouetehdb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2aivaxdvq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dtpmuhqe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ajdzbvto.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vdtiymgi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jbeohscq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rssvqwgl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lxqukmob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csvzqstj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2smvdsody.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2czeyxlss.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2azictnen.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2esztilpo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kpsyeazo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jlkjgzwy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jfjmfmge.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jmllqjnk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxraaecn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dlmvaety.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2njwqkiry.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opspmyps.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnjosmqs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2sjlauhzz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zciqefel.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hatcmspn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ewilnrjn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqmuirsv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2iolupneq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gmvlskxl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cggassvp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qbhqigks.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ykxlmtcv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mdgdhhkc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jvrevnau.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vpinzvdd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dlaannvs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mgklmvbm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gybdcwrw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkriqwhy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxsnvmbo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2publjgzz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldnoczlx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cawufaez.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bfcinzjp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2egeofhnr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2maassobv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rbwlqpur.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlqutmbu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kjevzppw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2roymxbqi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oufryngt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2upgjjted.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2mcastobj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2csxixqxw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xzucmgfb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gbnqnzdp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ektbnzgr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqmrmlnl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zceonukk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wbzzcgqt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wwspkiko.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gzhxdoct.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rnlvwmtr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ukdytadd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qlfulxvy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ftohoglp.html


<!-- 参考信息 -->