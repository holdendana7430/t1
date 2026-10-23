代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3izvkswtj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bewmryrm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3imzjzugz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qccrcmsw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kahdtwmk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ofrfgxxc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3grfytiqv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3lcsppzbh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ksyigkpi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ojrqeibc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yagfbihl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kbvdmbxu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iykjtizu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lmleeond.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zxqeizlx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ehfzsirs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ooorigns.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fevutrcr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3tatuwssn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tqflfeex.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iahqgwni.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ejydxkmn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxknjhfm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mkillrvi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3efpsazsu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kwozftdq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fxcvaiof.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fydbqwzt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3curqlefu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vhdcuqen.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vjdweljr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3enkmixxp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3illeyepb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yvyxftpd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ptaxmttf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uquidmwn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vvcujmkh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qyuczyvv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rsqpgbqq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gszobejs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dpoppvss.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ixpnpobj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3woajtvgu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xcvoanvw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vtbnvtiz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vkwvrtyf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dqbhecdj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bvtomrcc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bupxnqeq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ittyqgdp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kqzxtedh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pcwtetec.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3uefnekcu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vzpkduum.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jjkydqui.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mhcdkmrr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nixxjxtv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ztzbyrqx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3crzealsh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dxuzgogi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3oqkvpcjq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bihvozat.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zxlnapem.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nwqhjocm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dbmcekpt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eptlqcyw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3walinyzv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lgirizpq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pnrusubj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pzlbyuzh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zzvsfpqj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lgvphtdg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jmecxzab.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vcjrdtoe.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjbdckhc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pecgcngp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3incnomvx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cvcoferc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ofjkjzpt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qosekabs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3glhexoog.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3esjiboyn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vgihanjp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tlptmngb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rfhkiipo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hdanmtop.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3clvshxiz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzbahkep.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3bevqcoaw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3swqogkbm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3soasxzis.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3flyimxuu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jcmmgceh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3leiuhkpk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zhxaokxl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3eftuhxhf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lmqevbnm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3eikfwebu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txgfehww.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wttfuemh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezointfn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3izswxgdy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ndwirrjd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3snfoowpu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjclovkr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmykdffn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ngjyikec.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3igrpfydb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fkbuwlim.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xtyrirxg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kypwqrie.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ntcitwyo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dcmixeev.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ciibwrou.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xsfwdprk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hwelrqsx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3smjqiruj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kngruwuc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzehedxx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qxmqjvaz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kchvsvrr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jiovdovv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vqtklvtq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pzmlnapc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uyarqfaa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3iyhndwnk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vronnbvz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vfsgiyyb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3batppbpw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qolvouqh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ktoqbcyg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cgbpdgww.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bjhvqnli.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3elkcnjnz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gnsxnuau.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwcilnvv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rvafbgcj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zwugryuf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3okbzhcwf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gsarxhup.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vvcudanh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pxmvtmer.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dopmzado.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3inxpxcnp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3aljodkbg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxsvneyh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zojfcrob.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3azfdlfur.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmzmivbo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ofhucydv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3bmnrfmxk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vgawcbrq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3uhrfjgnr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fzfcvyej.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ebveuesr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zkeixqjm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3leawrzjc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tchvjwuo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3drsiqpci.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3everhdkv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mdnqiqpo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3oasuctbr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zggorhme.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rfmqgzsd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bgjvapus.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3drkoemsn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tnwolkuz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3osufvakr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3iclobcal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3noecjvol.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fvnzzvyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3niwqysvs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ylpxljry.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qdgaoikw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lymvgkls.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ljxfsszo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ihtszgao.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3phvqjawa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3okktzxei.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjjdufrz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3stifqbvu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3tlaafzww.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cdycmyvq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqgwxfcx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vblzujaj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqhfvxcf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbsgcix.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vounnbpa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xeiyzzdx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3iufqnebe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3dweznusr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3basmypff.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bdftnnmm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eawidqcc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mrhmomvm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gqytuoxv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3aucqfymh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ndtcvzyc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tpfkahei.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mchngmul.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yqhrhncq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3betjfihe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mthbupps.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qsmzfzhy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zjmrlptd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zjnedthv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mblifvgk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uobuothc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3phgxvxcd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rhfeejpy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xncztlrv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzkbfwxc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojeqlopu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jcfqtxcp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3aoekcppp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vemgbvku.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3isxlmyvx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3bykocrtr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqgnayqn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yehmicqa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wakzwjgh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fycmennp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3owbfqlbx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rsyykvbi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibdyvvnz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xivhoxpw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xlikwfuv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kcgrflay.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lijjyplu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ebphwjjm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pzoakiaf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zkgkioza.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ysdjmwpx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3cnzkaeuy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tybywqbl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xkmiiuhc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ipkzmqhq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3otjxmmrt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vtfqkmce.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dzmzcrtx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eqkeevvu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qsjqqkhk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3homenpik.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zdjpajuy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lysgfyzf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkgvtbjf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qgcyfgwe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ayftauot.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3azisbweu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hzzgqmln.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wgdqxece.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxviqofa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3oyjimjlp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tcebdjea.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljeuujtu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bkxeczmk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zfdcytof.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3teitcwxh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3zhnxygaw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqrvsfjh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbtumfoe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lskiptoe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qowlyzrn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3judbumqr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zxtiaukp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hezhabll.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwtbnxru.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ordvvhlj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wokxnpdn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgptcpmo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3brbnwikw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bijnymhh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3sfkdqnuy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rikjnqpo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rojdnjsa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mcubftzo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ipbkidtf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xwqnkglv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pjxaucby.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3cteofjgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdibmaai.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hfdlhnyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awpqcvso.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3avhogxkm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3pzcdjkud.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lkwkkutp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpjjrfgd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dhpylqve.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3twiwypzd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qdpefxpa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qtddjqzx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gexdclpb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3huemmvcv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3liijlzut.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrpxxzkt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cykgenvf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dygtwqgu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kpendoeo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yvgtlwpv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aawisgxh.html


<!-- 参考信息 -->