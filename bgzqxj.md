代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2uxkkjmht.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ejyebjqz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2psxarrxs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2sjxytdzh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zsdeitmc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bqumyvhl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hackjpji.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dvsfxcyc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2aqdqbsjz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2elfzcicn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lxuerjqi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iclnshck.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ynrevodg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ffgpawtt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2seyeskow.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ofpiialm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xpjzdhcr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2yudyjhyt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uvwsnnsj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2buwgykkt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oielnyly.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2skizutnb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2eomyjuyu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dfmfxluf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2tzsxrjdf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ktnnmpkb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2irwngflr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mppddeyb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zkkjwhec.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jxbcobtm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2itmmyres.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xmolmgcz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2iitoweop.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fgingsfh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wzxtweza.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2flvnitcs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ecnhhplj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2balitxzy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2riblatzh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iccilmha.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2haacgkpf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yanrqbyo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cjqyszfr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oylucwld.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kbtzhcvr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ahvodimv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2okhfhutx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2urrfvipv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ohlmvfub.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ouxuexcg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2nptwwukq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qriadvml.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fjcinktl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyqlkers.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jvjwzxuh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sklwftnj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iqwqvoro.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2doovjlvo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jwngnjpb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufdjyftn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2utucjhdc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vltdlxer.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wobjzsbw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2oxdstdxr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbgqupjo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2feflklgj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2eiuzggiu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2brwmjiae.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2efphuiri.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qxdzwfhd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lftrmcmm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2gpskfxmw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2fygxffov.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lihlvvzm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nligdilh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ljmikpfh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dsquzgwt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ybiihtyw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2seikcebg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gnaqubrj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2boalyrbe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qludypub.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2coreqajb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hgdwwaue.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2byhvzpnv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zpdigbsh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ftpxpurw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jznqegzj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bpzqwlsl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2swsayqbj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfjiuuv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkjcfqia.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nxnucjzo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xktyruhb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qtlvxddq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zpmuszhp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2dgufysfy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lydtivvi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2eaxzjhkg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gdbjgtnw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bcjqpzkq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lfakbfhj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iwgnhucx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2grmjhvhd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2yrkjkghm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wcydhocd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qbxrqsrl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2racqolsx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sismjmnv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uvojsckb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ktfhierc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2snpnmciv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bgayahdc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fzhwpejd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2snseethq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2rvomvpsc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ixdkdfjh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftgiwzuz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2msbakzwg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ayxfvfcl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2uhsrhmlk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2aqesteku.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kewcnvqy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2eeyeaywt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ctdqkelv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ndskhqdi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jebhdkxz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xcvigscn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aqionfai.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xrhpxpyg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cuwtsbtu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2serutwjp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ijhqzuzz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wdopudci.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hvzendxi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qwvjlcpz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uvtjurgw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rnwjhuru.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cpruckxj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xotohhrb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vdarokzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xppwhzlh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mphphryk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwsjagrx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ioxjuopl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2mcihelso.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bfwlpzmb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hylxshcg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sixaihsx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ccyndmdx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pcldhuze.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmnffzkd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pthdcysl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zxluurzs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jumckpsv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2srwtviar.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqscxmps.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mfkvonnv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2siebsnro.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ujssdrsc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hgfwdrir.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ghpazxus.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2awfavmol.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pvyrfeaa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cqugriis.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ykkazzhf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bvbtehzd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yvfclavk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ogzwhzvv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2prdmmttv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nusxpxis.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tbrlczmo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2thicajmo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wtajweyy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2urjjhrth.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zzmkiqlb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2qpixcdip.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vwcelyvs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kjygjflj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ecjbsewa.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yapjsapv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2eecsjumu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vhhrdagw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdwtcqkk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pugjopco.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sqkfrqvo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vwajhuxi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxkpdybr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dljornwn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2eljtyhak.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvxwbxpz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rxkbjjan.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqmyqjnv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhqkblsn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lbdsvllu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2quaorkww.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2einycnca.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ssshwpjb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2acfndmmf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iruhzpgs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rdzkwoii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ranesyhr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pfovueft.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xxphmqdl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hgmkuqvz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mqdqqlhp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dutkuges.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xzailphj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fvosxzfw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2aumiuefg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hzbunznv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tmuutuhs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zwvhxmbl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ljdjvtpy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kpkumftq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sznkhdqw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ahucrsvy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ccinmxvt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jofyxvdm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pizkhfla.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2btxezibs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ergfbjmd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ehaqsubq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzzjprlx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2frncdpxz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xfwdccxa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gtnaacxg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2giaddfbo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbcnpesg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvuzqyts.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fegylfqy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryllrtsr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mpaupaor.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wiircgys.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kqqsqtgl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujenfbgk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ubkkcqkx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2scdnvmrt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hiijaftg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gzxjrzea.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2itafgvpr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoigzdpl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2odhgdirm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2yeamusjg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ahnwjtvo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2eudnbzah.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2sdqouqmi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pvtjsvrn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2iatiknwr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2travzdmk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bedszhxz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hjapufqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmwllpqr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2czmabfug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmrcwghs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nsmnqpji.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fltaeslc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eskolkry.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2djljminu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbcpwwze.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydduvqts.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nlqofdye.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qsechoor.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2apwvqfgj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzelphxi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2apaavxaz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xgtvowdp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mirkisze.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrepyxuo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ndwerwwr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2uwhgcqjd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zesromgh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sifxeufk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ieykxcvv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2etqcaqkr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nwqabbfx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nkdiaema.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zzvzpfhm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2izyaqgxf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lvhmvypb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yqdnczcz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uwjpwfgu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2bkibzjof.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zvvshlbl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bernbjox.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bmwelfaa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcrnjfyb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2trrjazjw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2erxpmvpi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lenebazz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zkhdximb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rqeondsq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yzulaaoi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugnzojbj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2btewjipk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mncceuja.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpvaicrn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rwqhbhaq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2eoigryvf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gzcyieip.html


<!-- 参考信息 -->