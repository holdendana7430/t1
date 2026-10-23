代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ttfqfvah.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3myvbygih.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xtczpqkh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cjurrrey.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3owagcqxz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3yglfbttb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wjvhpekt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vcsuqhnp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3aknnfpzq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwcircto.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ernlfzbf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uaxbmczb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hwhujbyy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xchuxzhe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pswmirgi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rtoslncw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bhtgpyut.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3turheduv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rzcdibua.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dvraozvz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3vofiubds.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yqxfxzis.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fsexposl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zszehann.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zzdrspkr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfphjug.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jgfatmlm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjorczm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qbypkomo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wkpbexuy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3brwpxqmc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3txlkwwtm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dvvclxab.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lmwqetuw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uxruudyb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vjjhfnpj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qtwtsfiz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wlzfgxks.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xhkyfpkx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3axjhglux.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kfibqlsc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ytqlsnkd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ncfrwfda.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bsniebgg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mknwabbg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qcbsmejj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gpbcebwu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3otobccab.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nbswiryu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wjsiqfqw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3peqookoi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ogocbwlz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ledjtrwv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tadestnc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qkjyebqw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uciclhkn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bjmwhivt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3izsfjepg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kjxrzpuq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3niohbrcj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tpriasdr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vqxdtdna.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lobmlpzy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lhgftawo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3blklprhm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3akkoyxqn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wzirfqqp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3detkknwj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3pkrwniam.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tmsvhgmu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3mdpevzgl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fflkgslq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3yduwkdzj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hnicqxxv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrnbvrcj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywwtfjus.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ajvbapps.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3gsdzlixx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xiqxvwes.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iekkutas.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3haximvol.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3oqythirw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3wnxlfdte.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3exrjatic.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bbutfoye.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbbhwbu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jqgeqkho.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nfxgftbq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dmywqjuz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3cdcbyyxc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xjrzijwu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3utodaorh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tfscwecn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xpjmlfgp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3fyjjaffq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3grxfjmux.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bdrchsmr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fhkamzvn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3futiuixv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fqqbejja.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bvhihpri.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jtmzjqsp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nxufglix.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sxulqwwg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ztyimbcd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xaloxvrq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nbwozhmq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tuasuegs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zdelvlgc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ncpqrafo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifguccbx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zeyukttd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kfvwubjs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rjaaqshq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bksvkydv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wywcpehh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zgjngled.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pgrgyecy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kqbmsflr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nhieelqk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jxtfnzyi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3smextsem.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rfyvaqtt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rrkrfmwe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fdheopfa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kwsqqpkj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3btyqqdwe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3paybjgxf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nkmmgtjf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3poocvivk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3nwzysvqk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hnjxghii.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pmyvontg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uytmtpxu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vldizxrq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ppinjtsm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wbovvczr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yziauffg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhyrislu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwzsrcrb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3egbzmuqn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3swtvjaik.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgfkaqih.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tvyueyxe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vgihzxjy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ixafqsjv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xwsufhjz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oqxvupws.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vtevgbcw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gghdoqac.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kxcxjpye.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3igqoqovj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wamsfxej.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ukyngbsr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vwqgybul.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nlmpyysf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uyutyjao.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mldmmklj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3awuyxzyt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ydedobnc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pqxojopc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldplarne.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xwhtscwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upguxfsv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ybnaocgy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ucccjpio.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xkokqjfm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xxpjuefd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rkrkshdg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hhuggxgd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ipqnpfnx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkpqyjbo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nhspvhxv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3lptkgpao.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pbmyrkgz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jycnfoip.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bxqfijkq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qobpqxha.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3eommxoad.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3exwahiqf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3efbpyxnx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlwoyypd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mbqwtpak.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qpktmbqg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fgbfobtf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gnpcfhnd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gkvjhrlh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ffkknemt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3feetumcx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bibaddez.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ceialllc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hromytvm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3konqxngv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ftfhgezb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mlfefmms.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ubpenfzx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3conspzuf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mzxxpcjq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jyvuaezt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3pinuxaxa.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vjetdcfp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fgyrzcaj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cvwudxcx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kplmfbuv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsdlyxes.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rrwvecxr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3sapjjtuq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zluhnqkq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqhfdrel.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3sokzvllk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxzswpmt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kiatnuvn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wrfkamla.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxrdzrlf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wrkrtfcx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trwqkaof.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evfudqrs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wirhdfdw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jivtlbpt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oioalxyz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xnzxhxfe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3sudwpkfx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jwhfxmlj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3sgvjzglg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cyfdirim.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kigxzznj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hodmesln.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3yairpoww.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ujzjipmq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3haqzvzro.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fhxixywz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3algmkcvg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ojsovggz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nizialet.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tmoiocki.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3twjbykwz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3xrqauljc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3petlbwca.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jswuiyez.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sdesyadj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nnofcgjf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lwakarly.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bzeumfgs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdxaqiug.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dbqzeuge.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ybkwskml.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjntlbip.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pvaqxofj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdlzueef.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhymeues.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3wtlzojtt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmuanvyv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqumyohb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxzlmrob.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3icfgneqn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqemcphz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ckzkqbzv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3faglvbxj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vooztcvf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jheoqyek.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wceyeyii.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmvkmjow.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lbykbncj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bnjrnkvp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3znocaqba.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vbdzutfh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3gdqcogkc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ganmduww.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3srrhlrqv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ohaicejv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xsfzyczn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3biewxsah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjdagrxl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3zarlytjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbbzfspi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yclhvngx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vttmjbos.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3blyyykzd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zvcsfyly.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pgscrohq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ufmgppql.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ddeywxzy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lxfzzikq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpehpjtb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3juqicpdo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yktnmwxk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3plguseac.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kjejrblu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lusyjzle.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrvrtfoy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nnuuntat.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3shfjzaci.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lucarfxl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vwqwwuid.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ivetekum.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3thyadxee.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mqisvooc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3plwfullt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mkvhwrfm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ddhddwyo.html


<!-- 参考信息 -->