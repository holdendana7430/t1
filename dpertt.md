代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2tzwwjgjw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2glcylvok.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vijiqpcw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ivbxumor.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pqefqchh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jddveatx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsosceix.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zqfzsudo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iinczszl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mzhlckqp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rdzpdhbr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mfoimrxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2joazkxew.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yxcaamrp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vewzemrf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwebjsz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2uwlonzzp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xcqbsvgt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2esrdkikx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pjykxglj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qdvbhwrx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qjmtqgjt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ohnavwed.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2brzhbjnp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2uuutjelw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2swpfiwum.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2irkvncok.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ztzexozu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qvjkfdfk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2irjpenms.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rjlysuuk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2noemhflm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2snwnngci.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2efnjvecp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2aiuvdoaq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xvptowig.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rzpjvsee.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kwrcdhhc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2yjyqqydy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gzdvskjn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zzuvnnrm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ldokmxxt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tavorivj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fmelfxyf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2anvvaruf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dvtymafx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2driqapjj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kmdiwkax.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sjcyzaan.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2efsdnwey.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zijlqidq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2irlhjkcx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2abvtbnco.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cozvujdk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mnafxvqy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hpekyeva.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kbjzlxxo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2godroxve.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fgnjwplv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2lbctttmm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vqinqufn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qddsohnp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yusoskix.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ipcekyqu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yksfzedm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2slwhgdrc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zagfhfco.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mazbcmly.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ijquwpgn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ebzxgyev.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2aaeiwqyd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgukljfj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rlsgcbjf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mwfwwdhl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jmlkrgnf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lpxfnjtt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtkosnod.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qcerwvcf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2rhfywgot.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zsxxoqjc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lhplwxhs.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jpkeaxdc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2onrjzgyy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ckgabpsj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2joehoqvh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2shhnzxex.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vzposesw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2glbivdel.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvrhwnbw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fgmpfyxt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2abrcyeql.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wrphdsjv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pagzuhhg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fhjcrykk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fabsguhr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2lwwlxiys.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qhxllfif.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fiztmffe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lciywnli.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pgyxoqzh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jdengydn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2goilfjjb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lwomkvnd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xitzjosa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpunfvhv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hofzgkoh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bopfxnco.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tfwnrhdw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2afabjjou.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gslwyboc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2kyabaack.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vusjkyjy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oilfgpkd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vmkxxxxj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dhewmfuj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ndhombpx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nefhemzl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mocgtxfe.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pxlxqnxb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dfwhxsvc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wewrynry.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pofwdryp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2juwuchgf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dkgoftvi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kynxtmud.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ljvgrgus.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2evidgcam.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2swocfysb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2socdtbyh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nebydlfm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2iiadkyby.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ehqmgzbb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2piswxwxl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2muaheghd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejzqifam.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2sreeqatd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gjgzvurv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qjlxwhcr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gtvrwzds.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qllyxmgs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cbsclgxu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bkvkkcog.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lqjgtoqd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bdxcaxrq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ezxfxdxo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hsdkemqf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2klmegvhq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nxbzmvhm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hrkgglif.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mqkqipjf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ouzbwdeb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iojfjuoz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mqvofzzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gaxnzqru.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fjgqxnyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svcekfwz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2aqwutaxg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qwfgipgw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nufdmfnv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2deuzvhld.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xyjmawke.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kgxcjuem.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zbfkrxbe.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdflnjsf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vwejrtjb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fibrbohk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cewzkjpk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uxqizzdy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2udbsynhe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2redmtkno.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vupkdowv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2iavcdntk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hbiezqup.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2urxsxgfm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dfydfvbk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xorklanw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ehejakpf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pemvyann.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ohqsukkp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jrahiyiv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2umptnmga.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2miukepao.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hmkojawm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2vsypxcpj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rgtyugtv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2dmqmxbjm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eitsteff.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pdjempxo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2apoarxtd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pzwcbhnp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kfowgojr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zybqswyi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wpvezryt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dybkpmie.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ifodxayo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2giqueuee.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxaooene.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nvjcfgth.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ywlbglzy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvxcbwst.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltegcfqm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wftqxqqf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyafplwv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uemurdll.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvdwbign.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nijeicot.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wevyrqok.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yplryasc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nkqomgxj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2exqgkkqf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hyxptmwv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lrlsdtsw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pxhkpjrg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2euftnsgl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mprrmbvq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vgkmwkvc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vuilwkbi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fdqkcdan.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yhkmliad.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2oeswxerk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tttinaih.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hsaeflft.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qaohzmem.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dqbnepib.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2acoqxanq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2utspxobf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2colnglsx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2tofwnfnd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jtwmyugq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awlbxiec.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctowertk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fhzeevib.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2auskuewl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2splswvey.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kqwxujad.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2laurrfik.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2iqhekqvt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2sgvdbsyl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vpsbnpko.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xxnpnmzi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2acewgjtb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2esjqwexr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2lwegmkkh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2deognjxu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxknuckp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbesercz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2berxbgfu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2njunbxpu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hhpxmhtk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmzxmwao.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qroyhnqp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yutnoxjk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xsmdgrsh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmvzqmay.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vshrfzkl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qxqvmpan.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xpwhnjfu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2iysjbvep.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bzaskaky.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vnahwhdj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yvtvrogk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2fnzkofga.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fyqgwgyq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2szjeznjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttsihtie.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lttrijop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyqnnvrf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2cpkzlgvb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wkbkudfr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fbbfvcgf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwqlgzjn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqgveaiy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2sstboixz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nwdsxwqu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xhqdwhoo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uhwaislf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2bgorwoqq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rsexecle.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxtzdrjo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmkinnva.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcwyympp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ouernqde.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmjcbbi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hhggqyuo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmgahktg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ygzvdciw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fyfzucro.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dmlmwzvn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qvtgsuoc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hrvtysfw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vltzlfnu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ivnhqpdq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2njdjutjo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yokpcppe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2obnfjygh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qhxziais.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vjdfdoyg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pzidruur.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sidgjdeo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kadnftks.html


<!-- 参考信息 -->