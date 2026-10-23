代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xiiydzgi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ikgersjn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oxoctfmk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mukgkckr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ffvasytd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cbitbcrd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxhgepto.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3koathwxv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xevnjxjy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ifmjbxjc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qyvjvpum.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ilfgjdvm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bbayfyhf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sivrqwbh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yeppnezm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmuvlkcx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yxiqolil.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fnarrvod.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xmkpkrtb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hgtybmnh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nowccnmy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fcidlttr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bvajqdiz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tvnbokdq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pvjneycw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jzaqwxkc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yoyhpmsr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wzjggecd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zapcueix.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3umnkhkqj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cutppdgd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3drnoukfv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ofchbuad.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qfrdonov.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pyxlshiq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mhucycbx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hfkrdfjp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mvvrsabk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3sodymhyv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3blkonana.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wqxdsvwd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3swfccckx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qahjnnho.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bxagpflu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ujsoylyc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ynaaywza.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zrunutuk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tznvtamo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hgqbzekv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zuykqnjm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mskfbfeb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xrsnsxho.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lkzsznrj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zbmamrtr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kkppvaxx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pzfkvbam.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lfmpofun.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nvnbvvmg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qdalonty.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wsbuopbg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3elqjwyii.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3urtuptqu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jrzjiind.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lbakikny.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qfnzxzef.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3aniuyvam.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vucnforx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugrsfrrk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxpsjhoq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qjxhepjo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rmtpdihl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqnftxev.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3tigefhmt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ojarwrbb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ykafjbfl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tiaqejfm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3irxlzyrj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jspacihp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3enujlswm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lykxrwvy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xclwurpo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3naxokrhd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nafyivau.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bztyzvyw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3auxafhkj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ygeszhzu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rfctxulh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvmtsbzz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tphrqufh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vnisqnrp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hpersymy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3iuwztefs.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fhcskmzk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wwukjvyc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3owacmwei.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kinnbqoi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qkthnico.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3iysdvevn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zcydisur.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3yiepgkvc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3sdzsdyck.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zumvzogo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3atcxlrku.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vratxlnk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mwlcbhcs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rhvjwyki.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3otgnuvxp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3gdxsbhyi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3linrywso.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3owurnjmi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ssvmefcg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3abzarcur.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lbmdtvkq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jxhdeikj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lwximmmk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3huaoqqov.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nalfnswm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3webnteyr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3afmjdgia.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dhxpuofl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3abesygnn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3licmxzne.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ixvkanpa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tljcwfqm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3rbmnujam.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3lzaeszoz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3bxiosnsd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3yuzqbwyb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3csqmykkd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ogcqfqqo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wqbvoxki.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iganpsbq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3osxmwzxs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wumdcumv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3knqyhzma.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ubvjujby.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3eoxseesm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lbdhvyyb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rkrftcdl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mfixvana.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wvbgaltq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wcatasmq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lhdwddec.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hxkixeyg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rsgyzncf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ocnvkfjx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3soihqxlp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qogrdkqo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zglciomi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ttcuczey.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3smxhcair.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3krocdlxz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pbvfmnua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wklyvqxu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dkubafcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipggnmrl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmlngzuj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3adwdikgq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vmglncrz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3izufgyrz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bcdaqpji.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jgukttcq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mpissvnh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntniaebe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kosxtpki.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mndpwkvw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3idwglmpi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yztttrrc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jtkncblm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijfvmxpf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3msfrncsa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3eskdeloa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3khvtinsc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3larwdxtc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3pijqfjrs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3osnhkpwj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sfywmolq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nuawpxgp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mpuhuhxh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gkyutqyb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qrnzykho.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hlpjhudm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vvlxhedb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3raqqknmz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zgcnstxi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3preiqjwg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xhksdehr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fgbzrycw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3irgdxlpq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bdxnpics.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uezhosjn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3totviyrg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xofeaumw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pnufvjil.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3klbizjem.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhqpirfn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivvqcuyu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rmwjsvom.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3bazjmtpt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zuizmhsr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpitxdqa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3shaflrwn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hselbovw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fsdkdbef.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vemnecgr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptgvnibh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3flnwexws.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqwuuskh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebzwlwti.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vjnfszut.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gymdfktf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kdzrfcxj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ynkwgozj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mufodcup.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3brtsoxcb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bgdbypsf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3udzyezev.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zbnpjgon.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3pifgverw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ornmwraj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vtvquyaw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3grdpkalw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dysohfjk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gjwroxoo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bghifmsj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3lqbfcilj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fflzuodk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fezjynnn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xumrxonw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sycoiltv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eyvyacge.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3heeqsyho.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wmpxrjyc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kjhvetuz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yoohmhxs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubvmyese.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qlkkddhj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3aadvhnmq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irbkqvch.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zczuswad.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqgauubr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqvxxmjh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3glxgqgwn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtbbxgbz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ccxzptcw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xsitqnkb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ekkjoera.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3piajzgga.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nhtlrbia.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gftwybtz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbvmbmmq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3csgdqbsc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3uidbfzyx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tyjydxmv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3quhxexlj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vrdrgleg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rafgpqfq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3eaaktnin.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ikhiexkz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rwodmxcq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xfwzwbpj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3awzzxemw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lobkcglk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3adrjztmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfvvaeci.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3nqqsmtry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjsboafy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3pqgbehjq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3pbgytshm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdekkxkx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pjxyyovx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gayisjgp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qbpmbzal.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wxupwtqq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gtvbhegx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yfziepvz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkpqvrkn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kzztfuhs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kigrtutj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ugovzmnq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3umnbyzju.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwdxandk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vnobusvj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3rwpyxrae.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfyogtfq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qysdkjxj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nnidkwxw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3btfgfsir.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bzfdpyke.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xnyvgxmz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3iszxzxmu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nkoxoqjj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kwtrexow.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3iiqxfjhz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3imrltmvf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uwsgtoxp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqelonsk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdznuyhx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cowdelnx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojtjviie.html


<!-- 参考信息 -->