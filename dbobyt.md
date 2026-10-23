代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rvfzjcys.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3iwiektjg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xgdlpsos.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbcnrjzo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wfublnpr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3osmdtfzd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hvmfgzmh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tnpzvxcy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lvwzgeyo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3eqmxhexs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3kekcalxm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qjeaurfo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3aqhapvzd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vuzsrytb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yqthcswd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrutqev.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3olbfyyet.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhybott.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qyczgimx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rthpjynm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3sgklkghi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xtncgdls.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zfllgquw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ptjmkgae.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gydfcrwy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uzucyieu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mwtlvgwj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xylkefpe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hqocimht.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tldnvwlw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jgnauokf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3miaolgcc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rafwwdao.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tubbbwcs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3syxgvhpx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ngtuomru.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nckrvtjh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fxqexerp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3spbgiczl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rmtnpuqj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nhpcmywy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3krkejvzl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3odkrhwzi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3benkeshz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ceydrvlv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3oyupdgep.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qteubxtt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ejfhwhgh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vgfhjgqg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yuhgmzxt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sedfecdh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pvkymqre.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qjpuranl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fvaxmbpo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3gmxdipqa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3etemjshv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rhdiopji.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3gwhddobe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aujlodfu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dqwuybps.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mxucvqru.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ntwbuzcy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3iaghsteg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3stcdtpvn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jixohpnf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3aydjnfok.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qyrfjlle.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwrszes.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qeuwehkv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3korifksv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xewmkyks.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hubkgguw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3suwdnaxm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ftkmgmdd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xubescwx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3khbxkpuc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcnclfev.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uzvjntds.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ugiqpghq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3koplximf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bzqfkkhc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzomzzaw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vtctuste.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bfulbjsa.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3namurvzw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vwotozsb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bdhvcyin.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qmruztne.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3lhlfqsvw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dujkuzpn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zmynxjhi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3yfasiubd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fxalsgbj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3khaemsqi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdtlyntq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjsaxzxv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zjmwvngd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3pjuxwloq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wdoqbojz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yivjdgzo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3aayiaiys.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vfgjogzy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vtxcmuni.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ohprgktg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mjiixkur.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kjdebgpg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ksrcqtgz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qyysdala.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lgyighko.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yftxdgej.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hjpdiylb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ffzsufps.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3efhehptr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wnwjiuou.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jrxtkjnw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3yeknbdlh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3oaiqzisq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wzqgterd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mavslean.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qjxseaoz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rbxgdhkh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bqbtzzhk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqstjtyu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3skatgwck.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ldlfldkb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3uqlvuglo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvchvnco.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3anfmgxoz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ymxikjuf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rbqhnacr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bbrkystz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pelqgttd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gnriugjq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3junexlit.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zkiufmdf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uzxzvlya.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ijqzjyqi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojefzdac.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xdouqtyi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3agzedjjq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3njqdtweq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wqnrjkmu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3iucqcfwz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wkndzipq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aummsiuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krrohhig.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lrqkcjjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgrkzvyi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3scfdbqst.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3yfkkxhkn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jtylmykp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3uqhhxhvb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3djnjbzkj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cxcbvong.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jfsjbgik.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blgoibnf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ilyinmlf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ymvncqsz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ahicskmf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjfmpzad.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gtgmruml.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcaachmx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pgxgoecu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qamcxzuc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3mjsonssb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wihzpijg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lgtsuaiv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wkbvccxj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jcxfswst.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3racjbbio.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nymssvnv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vzdhrkje.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zdixkgtn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hmihujmv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gilmlhuv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fkgsabww.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uczkusjm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uymctgmw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nddvaspp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hfokoalu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3brujbstd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hnzgawdp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3supbxmfg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ampwnbez.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xbdkyyoh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fjgqstsi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cnkywvur.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxdalqas.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wlfhoyqr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vxkdzssx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vptuhtug.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgorvmej.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzmodsaa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3quorppzr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnljznqx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kpshthhi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttajnxkm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oikmszfl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mvhgzsea.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsyitwyn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bnbjarra.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wohospjd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3belrqkdy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3asxbrmkx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jfedlzyb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lafduywv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rmtoitrd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qoypbrdq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xmoncqjm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jcykscjx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3eluoktca.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lhojkjmd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vbsubrhe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3boishgnw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gqjxcpxt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bhtnecbk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gpaodaup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jbzrszec.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zbyfmzdq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mfzpsrxf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dsdkdlaw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3takjpfku.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jjgccnbe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xrazbbkp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nftbtvvu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wreunxfc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3lsppdbut.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsdsaimw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jfmotpln.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ecervnkf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iciboeew.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pyzbecbj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vexlivvf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzkrgchc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oymdtidx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlfxdgrz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mynbqsus.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzrktkah.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxtfqxba.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vosoeajt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kcmhpwnu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ozybxwhx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcrygriu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nkwnlolz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hzldjrek.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvgtvjra.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xiwhgbjd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zkbpesug.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3buinpqum.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3cspedgsi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ebgkrdtl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nejexawn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tkkidniw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ptztwkph.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lqtmnfbv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wzizaord.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enexgjcp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zinyqewq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3boctekjd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3chiboygc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wnmtejwv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbngbzcs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkaiwvof.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlrojodq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ohosmxnv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sxaunpjg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vpnsuozx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmbuucnv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nmsvjxwx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ukgjohpr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gnlpmwpm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqesciza.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svrzfnwg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dveocyhr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kduzjjyb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3mrducmvl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jorzvyzz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mlhgauhe.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vhjiqons.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3feicdnjl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wtzwemwp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mrlpbihe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qwduncbo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pwxfkgnv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hlkzblkf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cmnejjyw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lxttmhhe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rohtslgz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rtbtjdmh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ylqnundb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3npsupgid.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilzeosfo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3osnfpfsd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gwhuixnw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3axauqqor.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nsrvfrmu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bxqdolwy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3khagstlw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qckocxds.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qghdiklr.html


<!-- 参考信息 -->