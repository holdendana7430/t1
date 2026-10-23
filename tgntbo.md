代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mspurzqb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3opsgfnos.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hzvqetga.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vntwzlqo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bmgtjxls.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3aitweebu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kdvfoxrj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ltwqtjcu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ewhnvjgt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlqntmyv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3srojduiq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ngjprqtl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ozmugkrv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3osfkoylh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cmvaqoin.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lflouncj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dkteludq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3iwwocmeb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zymjtcis.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mgdfhsvz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ctuwnhaa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wakkdshi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3thrfrrcq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3spabyyyz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jxuvgfjf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pxemwkxf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yksgogqe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vyqypdwb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3eiqpcvtp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lfulufls.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3innkunbu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pfsqvamx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mvtuvjyu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eohyhkgn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3notfdigo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3aywsgfhb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfywxsd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3phdcixay.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3swbzgxva.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uydmgmiz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jywzxtka.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kiunakkv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zscdujyt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3migpoaej.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3slodxkyr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wnykeoxp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ybgwnkkl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vhihkkvy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kuijpvbe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmowged.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lhtuhofm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3osjuhmaf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3elndvpqr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tvdgcqiv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xvrxduva.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ueqofprf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nkosvubs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iestwubn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tyxcwsuy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vsaparox.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dlvycfsh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vxdcurvi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pjupythl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sxjifgnf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lnxsvhfk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3luvxxqvp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3azjujlcj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3szemthoe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3twzvxlrt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kaxxrvfn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fmbayxjs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cqqpsjxq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ajopytrd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ecnqbhlh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wxrexxzy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdufqzus.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zekjzlve.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qrpmskhz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3nektbxbv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjedlpsg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lplcebst.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3nanxtzns.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3elqlwvnw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wdrvizdh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qtcqqaqp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqafygz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kxkgifrh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ovlftger.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sbyjpjxd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3grkhfrmg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tneuiias.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vffoectx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ppunkvrz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tnekhlhw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cwboofim.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcswkfaj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3stvcbzgf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3buemchka.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lmusrwiz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uwkqnspw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tculjfxx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3itywuqcz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hphoxczf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3siflvndl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jqrpbkhe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3sjsvgypx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ntqxsaoy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fclfqcpd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wicvvmhj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ntldddsq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pzgelxpg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hbwnlxuf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqupuccd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lvycbgip.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3arulcbps.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lnmcatlz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ezpojbuu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3aqtqahkk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3sebrdkgj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qysnxhfv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xlxidabe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wtwheuuj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nrkamqvj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dnhggphy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ytdgvbxc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3miyufzue.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nbawbzen.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wqsuvulv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wbcpfnvi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3aupgibbh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3yoniojdr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3yjhsijhh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xxmwiuwe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3aclvbokr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zinaombu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gvdorynq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gjznajam.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xkyuclcc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xixpfwmu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3afttseas.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3eqaoxkwe.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vnlbleig.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jdxpkfvb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3oufaqctt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ejcteyuv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mxxoyqvk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oytcnnxa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xbltphwu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zigsfzde.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zpzoljua.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ugtyvnxj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tmddmqye.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xwdewjcb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3uklezrjg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bwvmeyzp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mrxwcjyk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mnxauvyq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gbcjnhym.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zolanwss.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qxraexyc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kisgnlnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruefyozb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nvuwfeow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhjihqss.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbxipgwb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uamnjpuk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uehorniu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xwsmowmv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3htojojyq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vvnxvyia.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ghrjxysa.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbsvlmui.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sxjnqqqe.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnmfpdht.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3futnvjzs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kcmiwimw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnkzjvbx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xoqcjxow.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wmjxnoeq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ktvtxngk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vhfgpufj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3skeisqeu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ofntprdu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3liifrkqk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dyposgim.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xdhdwemd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tzxsxdwc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3yqxpzvvt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3eocsgljk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3odhdcoyn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kymtfszt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wriegclq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bduqdobz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ixpjunxd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jkebeufh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3muucsvzk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fpvtpfcb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fikcuuqb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3tmjkmpfm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mavbjzda.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3awiwirph.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qxknuqlx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3juophqgz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xzolgepe.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbbdyboh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mturifoa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3taydzome.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iybwszwx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owttirsy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hxvtuvli.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uruuaatk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bseluagv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzspuqhh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubtkiyjr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xzitljwv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abwexwhz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awbfqicq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gteuyauf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fmhmywgp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vgekhnkc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hjwcybvu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vvmgqkei.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fkvqmjoz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zwmjecdy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzvwwhc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mrjigyut.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3yhwjdfok.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3eczjbzmj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3agfmkjmm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qlqffgsg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jvhygwpv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3izmtqips.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kiztyilr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3kmznnhcz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tsqoabwk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nafaochw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hptenkkz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbzxqoer.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jfqdgdjw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cqqachro.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qjxrrpoi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3awzvgfvh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fvmkhakx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kihdqhwa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zndhrqlr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lznjjgnj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kntfpzpc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wybrfngt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gtchcsdn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmuwcsfl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xbazjaim.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rcwbqwzs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sxhnuyxb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxvreolx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3evovvzqp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3anftmcyb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3yjvtilpb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmwzccoy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmaeebnu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3znhvstsu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vkasizfo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgnvqjxh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dhsajjuq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fpzrqfbq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ixdpqvsu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rtojrirl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lkadfgev.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3eghrvdjp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qotawfvm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lhaffkqo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zwnwvdyv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ylinhffy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flkgbrvs.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gvotwcvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aggpqhmq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vxfbusom.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tbtrfahe.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3awiicxvf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekcyhcll.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3obwkrbvc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkmhavgb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vjrqukpf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dbtzlinz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3quwschbz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lqbmsgjw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ekwaffhy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lygsxpdu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcnttbbr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3yfzxxkwj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaiadrqy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fuqhcrwj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tvcyzfzv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mdrusoqo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3myuypjty.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pvjyfihx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xasuqyrk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lrufvlbi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3glzcmfuo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3biptybub.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pmxjbfuk.html


<!-- 参考信息 -->