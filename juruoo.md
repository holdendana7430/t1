代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uotaiprx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qpzjahcg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ssgstacj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ykvwhqbg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bwjighvh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nxtatlsh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hybtqhpc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wiktgene.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ujsljlpr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3izdchvlv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qsnovupt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3shtemtwv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3rhuzulie.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pvcqmfhg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nhjovfkj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3klwfnofw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3gsawvtbz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uzegixdk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wrizeexs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3iqzynqxg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnfuthe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pdglhpvx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3eslxmtci.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uefprmea.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yodcpfiv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kcmsubim.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xighgscf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kgedpksm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lotmylav.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lkucusri.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rbrjniev.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sjwgkphz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lrjpfbrg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sdfmzezv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bybbrsew.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uyjnowsi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3semdfumn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3trzxohbh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3advwlgpu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3agvhnvsq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iuhsekmv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mzyuspqv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hrztffrj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3frtsrysa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jogsxvvc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zhgdeopm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hlpxjyok.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ldqjeqhk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hwtbqzkj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvpnybhz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kqhboeei.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ktsdydub.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ajomzzcj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wpszkber.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3eshhhanh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xcgpijta.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3holtfksh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mshmsgpa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvsfoqdc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yaluvxrb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3asulhjcr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3buwylpzm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wscnnups.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kkythvlq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fvetugij.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rteymhqa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehcwmbly.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3eufkolzh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3drdpoxnq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mgcqeroc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3majadcnk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ushelxhm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lpyrszdr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3goiqkshu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3josasxyt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3byahmehh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uatgflhk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sivfmxzp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ewvkbyaq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3llwpzuyv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdhrzglb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcrqizry.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ptmsvknq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vzvlyihx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3anhxchkm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3blknjarm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dzaynamr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zrmvclbu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vaccdylo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vkfulnbc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dbjygjtf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jmnlhslx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3uwisbyee.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uqmlepmf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ubfkpibx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3inyrwvud.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3flnenuiq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ihqwbmye.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gyuttcmf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ahiwyihn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hqktqgsb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wtufeacb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fckyhnel.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eegeemkg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ukaugamc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3agifcddr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sfhynfqa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3prwkkjtd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3erycqqdw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jxjjntxu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jcithjvu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ovirbihd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eygqgssh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ctustsxk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hefxtfzq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qhvxsnww.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kuqmwkkk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3otpzevog.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vlclibbz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rsghvshl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zwhgnxcq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlpevimn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwozqgzo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rebobzfy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3acokegqs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wunvhzdy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilvyzzez.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3pdnbxghh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3pwywpgpf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3orruawjy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yfzpiuhi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xrfhrxfu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bgxaajzp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wvlzewkv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3unqimbnb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3udjbmaor.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3moyznvsz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ojjxszsh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rlapagpg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bmcvlvdi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uvnarxju.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zncvixkh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ibfycmfo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sdtihqlu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xnqphhbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkjlswws.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mzoywvhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjctutpe.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wtbopeag.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nplvhiuw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nxnpivkm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nxdwsqlp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bhqnfsfr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dkfbudoc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3thhszqdf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3usgmqigu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iccruugg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqzrichm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ftrqecxk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhwvdfhx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nzdyjned.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3skfbeqwa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ozseqsbl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ygxgqehb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xkxnxxvh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvvkrilk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3djfpeoit.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3plzoytrr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ayugaalb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kxpnpgkz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xvtoibdh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bbawguvd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zkintgjt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ggagcetk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bjbrqfrw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mqodrxww.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tjvurikw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3umztysyu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bgivmvxx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3whklrniw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cahhxwol.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eaobvkrv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3yzbuyyfu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3czckavai.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hiiyecmx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3okrcmsnj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tyjckhas.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqbpnrrv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lkkqtutc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ylefroul.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tpmpkstb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khwufrac.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkkdqmpl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qcqncbaz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emzndiyl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3udifobyt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfvgxirf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtyotxcd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vlcpbvkg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afprydhh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdigrvxr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3assducij.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3coegaegr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgrkhta.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3asrvmwln.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zkkfasey.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ufhkmfhw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dwqrddht.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dfzaxweq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yxspokjz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hkefuyby.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bzzshvny.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dstxlzns.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxpbratn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dotatcat.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mzbabfgm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xudebnnp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hznnaxjh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ewxqoudo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ovdflspw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ebtjyiiy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljykxvjz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3freeuxvu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vfqhzsya.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qkcmzjat.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dwwhiomb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3guskdidx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jivcaevv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3sypiikvn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3flzpgpxg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdglxmlq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dnrqjxnp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xeyvbvxq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xbpwyyge.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kwtgwaok.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3edjmljkj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ektjcels.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qpfjemwx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dmhqcfzr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oybimjxp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ohrlmgxh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sfpjvdik.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gyjnqmjo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rrnlkjwt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vqjgxhip.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ozobyoot.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3eyurldly.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3unvbpmcd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hkgjxwlt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ncjlpnph.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3duvaumvj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3coadkpka.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3yqfoainv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nopudlnv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vnguorom.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mnaakztq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxvkpotb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kfyqpien.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3biyavijz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3aprhiyga.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hhfdswxv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhyoqdvd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mesflnlx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vrzvpqqs.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvbhpvwm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3swpcribx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3aqiuqrlm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3minxqiov.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3floupwvl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uofbzexs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sicgproz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jrlrhesh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ybblqfkw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jsdchpba.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wqfotdfp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bagrgren.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxlctftx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bynmsbcp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ptluhezs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mehpgkrr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3djideyri.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ezgvmkwd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cghwkxqg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tqfgrjtm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kbowjefe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3clahsthv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3piziyaww.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3slplbztp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igqlrwxg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lltjpwpj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jzfldfdl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uendwtkn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lhbnfmnw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3amyzktjx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3crczeuyp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qjkcpvbl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bfaafprc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lspqtgda.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ddstzwto.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iezikdfm.html


<!-- 参考信息 -->