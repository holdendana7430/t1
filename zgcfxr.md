代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tlkdspnm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qcxlvgww.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mqzzanci.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yqxzwgvm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3kalstnwb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3onccvsqr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mmyluxnl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gntzsmve.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uhyvuflf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zvrznctn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mczvafkw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tkymddxz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3poclinyv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3auikrrxy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3igrhmbhl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zuuobbho.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ebrnsnfz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wrcqabwf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ybzkpnqo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhiygmnv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uhlfeily.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tfqurzwp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3kyqmapzg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nlnqltbp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3iekfxgtp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lyjzppum.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bvihagqs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vnsqqwej.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3plbzsvtf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qsemwhhu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3skwjxiqb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ebirjmdn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kjnwqesb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovseshlq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kpxvhdim.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xowueaxb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vvrgkhdw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ptqiqvui.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pysbabrr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xnkvbumo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3uwgfrgqi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hevawaul.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ajapcevp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ukpuqoyp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kwsjbjaa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmbcnbt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fkybuvwn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lbbqhuzr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mpcwnnbr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fgrxnfdf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gcutegis.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yyjohbsd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ohmxtcxk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wxvfffqz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kfhomhsu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mpxszvqm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ayavxiqi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ufuyoueg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dketezfd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nqqajctz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3tijrgela.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ngkyspet.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xedyvllm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3nirlnets.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3iselkdsz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xrgckeen.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3irecsslo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hiadqbrb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qttayucc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahpqbewi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fsrqzdxc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qvrzahhy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3imjfbcpa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3bsqwhkuo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pbwawmnq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgjolybl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3nrkinxix.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kyisszaq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ahlodlul.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3mmnkllnw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3xlugnjzm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ndzpuody.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3nawumfzh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uyoaoqtv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hzwvados.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qufnfhud.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mlhvswrd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3lzxotkdc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3doeeyvfj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zibsayug.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3aktnmida.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rozjobjk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fakbflcv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3seyayatj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dvkkulce.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzxjkafn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pipbhebf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3scwkkdso.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nvrrcqzp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tfcqkmfb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3fmqnkvhg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dvopuvyu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ohskxocy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3btjjdvxf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vesqjyfh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3aiwhxskk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uaktysau.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rfrjqxzw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3textyklc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xakcjsmg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3npakbpel.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qerhlipi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ylpmfcyv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jxmscvka.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pxclascx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eawrltgx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rtcbdnvi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3shjehdzz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cgcsqtjp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uujhtmjl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ddnyjkom.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vnqaxdcc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3guntlrcc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3abxoddrk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ykoktmsq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3smyhrmlq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bdsebrdu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xfivlirb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3upakwdqj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pfenoqez.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gejsvyzx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fbulvkrk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mbgcqhiu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ikpmpxwy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lecciypp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rdtkcnzc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3poosskwj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3pwbdittk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3fvnffojy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vrmenqsr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dabppmew.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rlvcbvpm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ikcfqzap.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fmypsbmm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qvwcvlpn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3aqrbydzq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sysgqjxp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ahmcafue.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ihtdglzq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrvkjlqs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cbiyjber.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kziysyqk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3anyrbsqe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mpbyapvk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ryadpvld.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lpwwlrst.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qfbriedt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rynbzokd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hnopakoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtjoavza.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3oyowupyi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3icsdmvhu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kzsjvdcu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bpujfcdh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3epsxizih.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mncmmlya.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bjugrvnp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnxyswox.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jhipgbmh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kilzcxaw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wapncryf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3eqsynjsu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzbxsnoa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnlsrzmt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pjfsxwxc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3paxuojgd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vyppxhqc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gthbuzsz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kpvncxta.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wragryck.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dvrbycby.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3asoubcvh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lmlglrml.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wfyrchih.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nrbbprmo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pigjdjju.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3baherqru.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xnaabnkw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dvlczvjz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zjyslhzv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ckefdmwg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nrxvgast.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrsbepe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dgmzepno.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ylrvwfhe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rqvhsvni.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3tpfjufrt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ivisbygy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zrnlkdxt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3csbyfvng.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ywaxwusa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yauthqpj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lhraqnpd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhbngasc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fuwwsfsd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3abcizxgs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xclmnayq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3suhqyquo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjhjsjgz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twuigqqj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ujjahlhy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3klodsxsh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3casobaxq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sjaaxoqy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gskolliu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hiwwsruy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3rilzcsws.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3drsmixli.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bgwhtaic.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gveaazwd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3shauuunl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wkkleprf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3npaeacua.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3suhpblrk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3aunvgals.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ettscukl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qjoycmra.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mxqxprsp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gbmwvdyi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sgzuelkb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jbbzilgp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qmwthqkz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rnkeqgot.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3knxqzrjp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bcfjbbjp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wvcsrumq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iehhwxpy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gtcrwsik.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bhjadjzq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrrhqghb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pvexcoqb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gibpukfw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmulyaxl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3catojfbt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxserjfi.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igarhaky.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fysrxrrb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fppizvbx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxziywbq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebnwndnm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wnivwaxu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsiggaqc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3rxztaosw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqrndery.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncnianyj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wqkwpziy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tbdxvqpl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3butynexu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dkxgppsq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3iiddqzin.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fdqnxswg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ksuoorah.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xfvbxvoi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hrcwnfft.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sjpsyrld.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3yxsiezia.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3drsjftiq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3iagxqmvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyjpecgg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3kzdxwzsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awkxktmn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lpkwtgwn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3cdkwuayr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jjtsycfa.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrowdxwo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yaumwdcy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3gawjyaqr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vmhxvwxg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hgqmanip.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jdiwqeeu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yusforzm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3egreexsz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qeyucgsr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wqerexot.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uscqmgrn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybnbipel.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wwchhqew.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xfbytxby.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3blxkdrig.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3glhuljup.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uloovhzd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ikxavnfn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zxqdzphp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uukllafn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wqolqfxe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wividhea.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3odhoschl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3viojtldv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ekdlrlsc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zgamguoi.html


<!-- 参考信息 -->