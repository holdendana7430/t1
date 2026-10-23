代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jmnykpdr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oabkebrq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3srdpzcvb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nzjqjyqr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tkmufjba.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hkymazws.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rofcevqw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3utyevpqs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mkjlacra.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3akxvhovk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tptmwflp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3akhfqbqx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jgvhxhex.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nyncalps.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iexmyltx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zqmqxxho.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cfiscyof.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gvretdtg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uimxhtqr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3etwkfinx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ioysbaxk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dqjulxlb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fwqqbfyz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgnbfwxt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xmsmtwcj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kvqmmydz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qehkicas.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3prxscrhf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3caelizbe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wgzicqhd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rifczrqw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cfivgmir.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dwmawtyd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qiuwziie.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3urrdygcd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gwhfuqwp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xykpqppm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jqjrmoex.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mrkkkjgv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mjzlrxzl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ujhxjaae.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qfnyqeke.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3alatrnxd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qgciruje.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3egeiffsn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3oluizaim.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fqjkeoau.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ceegdvgl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zwralpoi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gvlwuxcw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3fsekuofp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rnkdvira.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iwzqmmob.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3amiaauxb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fzoolppz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hsdlogvn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ampxtmxa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ocjmctde.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xsmmnwjj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zugtwvnb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wunwftum.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wwzhxdpo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zzmcvmcs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3giqfusgp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3botquckj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dyrurzqz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qfxnooaa.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3szxwqjpd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3prjiwmbx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wzmezjuy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3khsjcofg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3uqxyxzlb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3qnzpinih.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3osxcjjzu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3xfkteslq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3oaqpluap.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mbwrnide.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3apayhmfy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtgjbory.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3urtpclrq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dwioootc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dtzbdjlm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3edjqjmtg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oyrarecm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3rieznopc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qcviwhjk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xndtsutz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3orglvtmj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ujuwojxu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lsydigdd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3yodyqikf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rceojayo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lfczuuou.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ppoxpdul.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zypeeprq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zanyujkx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3odiwcjeu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kbqcaaok.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3oavwieki.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcyoeasv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbnujruc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mjoyeedy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xbpmenkh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wteknbqs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3sgzztkpg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wuwvifcn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3oljqgajo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kakqrtom.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pqfqqidp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nmjjvelv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kcudkans.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gptfffye.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sddojebr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rsqhaiei.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ecuwkujj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qdmnnuzg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nenogart.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dxdgrfni.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dfpnctxl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xwhemwqu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fxtmnntx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gksuiokf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ulnhiyig.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ftnqdcgv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjalphf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3arczmrri.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3htpymsry.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lindrtcx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3grhashkl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xfauwxep.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vcnzapdt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sbsexici.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3iyvxayrl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rpzfvlqe.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qoodtyff.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zyzypmuh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jerdrokv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jdsnjnze.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jazpazlu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ckpjubof.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3atptlrcx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kiapjhwx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mhyldzuk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bazqwhcd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctpubhgn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kiryfxzt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydzeqgbt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3clfnnskj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ewlwwyxn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cwlgnsrt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ruikivwk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zfndtlom.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fqcjcinm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vmxjmxhv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ijqkbabr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dsjexzdy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3cavvhsne.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jkniwczt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3btjorjrw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qkrhgoid.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vxthkctc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3apzevcln.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3nweyenxw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zywhqwcn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wquqlxpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjvdigdg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zkrhafgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzvbhvks.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uaxeeiad.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3thoyxgol.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3erzxxjlo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wjdvhuuc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ozawnuog.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mnencbly.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kzddfrsk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifkssjit.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ifcmarqf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3decvggpw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ggwzvowu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3cwlquxfo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3neftrqce.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yjdycajm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hotdllck.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fbrtibeq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nrfxglds.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cwjcsivl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nmeitdfu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yfqukexg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lxypinvb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dvumdcun.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yzzxjwwh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3zdjzfqwk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zduyrqyg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cpuxgzzz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qzodhupe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3aexeizwt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gsnwgxmg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ltiwazfo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pyzzgtpm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gtgwsexw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kqajhmto.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hlducest.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yetogtue.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3sozaqpkl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3sovbjjix.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zkwcdulj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eiurqofj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptmykzti.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3musmwhcp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3npvaoyqf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rywfnizi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmmeaqzr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvujwyco.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3koxotmrz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzxschuw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3igsizseu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cswwonxk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eyuxnwcs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yikgmubv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdcxvqph.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sihdcfpi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hklprgpc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qfnlmony.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gwrvvqgo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hjntrmjj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xscuyxhy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xcrvwvmp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmsaimlb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vfxgrkvk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vqgbxnru.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hpbotagl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3idlhvtkx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rimkqgsb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3czdxprnt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hgvlzekq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3baegenei.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xvkdkbby.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ejtlfqkd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ywrothbq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bxznpzyb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wuuvekyo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhcivlrg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gqythfek.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hmhqzgkz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nkyecmon.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3femjbleq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rngcgffy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkvqkmro.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qgxxkwue.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dnsvewng.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsnqmayo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ommolxtt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbqqdncx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckgawtqi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3wxxgasoc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmaqrryx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqueiwwm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sadtnjjz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mnpbhtbd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xpqzygki.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qtqviskd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulcplppp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkxkccxm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3akvtwmvf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rcxfuzav.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybnwpiiu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yzcuibtg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3nkxobpdc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3epwmrwxz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3fzzekylv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kqtwecfg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mliywlqv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bejfcmlw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xapxqgfh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ykhboowm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3hjuetghh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqvabdze.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wddwtfld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdnmuitt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ddppbnom.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bcegnmdm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vohllxpx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmnmlszf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dvzmpilq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qgdlkvyw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hkorccur.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbfpmtky.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vtpeisbt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qzpndaeu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3pxvfneuy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eqebsixs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sfyemiko.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3emqthlqr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shizzubr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3uuazyrrm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3uuohyruf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3knbqpywc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mbvxjvgc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jhhzgsau.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3opbawrwb.html


<!-- 参考信息 -->