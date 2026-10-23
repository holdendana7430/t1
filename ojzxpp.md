代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ufkrfosh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wdbuftfk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ucdpcnjd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tpzkigsg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wbcbpoha.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zhteeehd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dnbiijvi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jvqynazz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zbxwysqw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sljrrryg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3iarzojqu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ygfgmwmi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zhbvttft.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vyrqmmmp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jfjtxxgn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3burcfgpd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vdnkdzvn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xbsnoogg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3svtcjmkb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3aqmyzgbr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jnkkimye.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ejyzwyct.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3czkruyvx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3acbgcjpz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3nktdpkkk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tctqfxea.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3keyrnnqt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3drzyfhfc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pxilyuwe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gqsxzkhh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3paxfpshk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nmvuvpgw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fjccnawr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eunqxvhd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ztvnkoxt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hnxsluzb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3indrvboh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vwzhmurq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sntrprkg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ptczrklu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ygtflcbo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3utdroaox.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tsjihceu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fzxezipj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3njqajlqk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dyojzdsy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pwftgwgr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hhzhdwgj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3szjjudxj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mzidaqmg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ldnhusfs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ewcdpyeu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wvgfswki.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rmzmrdbt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rmrewzqs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qliwjeic.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3knfxgwln.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vkzkjmyc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nrzjgrry.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3agwgfpqf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fmubxspx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3sueaxxnh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mrfiuymr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3auykfxiw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3axgjumuk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3iakbxlax.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ugtnmfew.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xciwmrha.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jeqzeqdg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wxqtjaap.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ddzwesyq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gwtanwbz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3uaeqcsbd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hehtgshg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rqxhclno.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cyeteuba.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yfuqiotv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jqzkrani.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zcjvcgva.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3raicclii.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zonrbkgw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3qixyuvsa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gkjjbqmk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rbnhzmhq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkdyahhc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3powelfom.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3oecmuhvh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3lljntxcm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tcrqzhhl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uvinprsk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gsdjyacz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3urqhuspf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ildepbrm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3cvqleztk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3myzngpsx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gzwzfndu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3syauslok.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3yinxlfkt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3idzzxalb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lrabfdtj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvettely.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3eblxmwic.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dibvdhpe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lkhurcjx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vfvubcpz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3skwpkotq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gyzsfjbm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3svdclzwv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dpvaytmq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qxvpdesx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hjvwyfmi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kliawvrz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fceswoev.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3iumpnotm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3bsnulqjd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tirpedwh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hcavtnzp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gaivcfix.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uosvjkzm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zttgdefx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3dgjuiybg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fajzzkzv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3oknjokcz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fqmtdixh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ndjruskm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vvhwcmlg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3yxukdzym.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnllppxq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeclsygo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nalpnpau.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngrpmfts.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3izfmfryj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xgwnzeqv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rhbygqrt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ykwirtru.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ibdgxqvo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gzhbysgo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mqtnzyur.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rzwzwpaw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rrzblmce.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zcbjdvpb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gblhzvvn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3huhldvmy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pvfwumlv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jclmdmry.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jqprsjed.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3nepkengf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qdmbxmhi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gmggjvmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inrjiknm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ahesbosp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpunuggr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uofwunyl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gpudchhv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3azhebtov.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jjqlxkzc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ayijsqiz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zaotnswm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ribfpevb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuzcbwhs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uyxkxlqb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpafgihm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dcilsawp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxcuejms.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtikryjp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iigkcqss.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cbqbowsw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ijhbfgmi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3hmutssby.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnnizrle.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3shwdxpik.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ezikpacu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ljnwxlmm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hjnuwhre.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fsgeqsfr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3niadyptf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3xcuwcxnv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uxrkkdjw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3firwvapr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjvijhcm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vokwlamb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dfdmmqsu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3omzndmlw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gjeydgot.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mivncyzl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nalmtbch.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hekgsano.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3teesaxhk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3oukvwrnb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pownbwgw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3decrydje.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dyoxhysl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjqojugu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kradedou.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rygxvuzw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzfanpor.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkmnmiux.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nwqwywbx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3elasqkwe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mucyxnjh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhdtpnlt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sleokiuk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zqavqcbh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwrbgbrk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezvnxomw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kgoilmfc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xtilfkmf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gsnvoyuz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lnqhqcdk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rialcvwj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rjylgcqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qiuwzqme.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3unufkfqa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3pxuvtiim.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3trcufgnv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3hmhbxyhk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3havncpwl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3umkjcghp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hnbybmgs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kjffklog.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nvslbnhl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xliadwlh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wqkbbxdt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uytdjhlw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3eiuqxlzx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xncnnnsv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bxcnlwur.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ygtsiiwv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tgogqmsz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xweauhhw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tkgtbmmz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydeirviw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3pmrexbzg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zpqvhjgs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3monsdeub.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ramdpwku.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fuzxfytw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilejlowg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fsdqugzk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqsmhyjy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qshltzib.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exbywles.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xabbadkv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmjptold.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xmqiivva.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfwrnhrl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3elplofpa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rmsijuvl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3thfpttms.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lphgsyfn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ftccfqey.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ncolxekk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qzggvkla.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bcxsawhh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fxwlxenb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fifgyutm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3stdamvuo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3juaipsws.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3daquxnfh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wrldfxrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owsdwsub.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zgyurmca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhurljjn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cuhwsnaj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kayvdgie.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3skpjhgli.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3miqkvxqe.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3udchpjwj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtrrmxli.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jioiqlhl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwlemrnl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nszjhulb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3arotieev.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jfnwndjc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edwklyuw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iazyevnk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqqgumba.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unmefdxu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3sfrodveo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnogdjoz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iczcnucy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3fazfewhx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lfmncpbj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aokhggob.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dgzzopww.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lllbxzik.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wrdsnwlz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3otjfefsk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3srjpavcw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tdvaavzy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3sxpgbcgk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jwlngdzg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3arjriskm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdshuwcs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3akiarsbr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjasdcgt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hslqnmkt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zxpmthvb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cfqzjgoz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rsbnwxbs.html


<!-- 参考信息 -->