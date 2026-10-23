代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dgmhetpt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3szxgosbg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ddnlmwgc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qhnguzwo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bopqxqkz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3pumbojhg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cxodwjyp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vmrqfsiy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3afqeuryp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3texrdpvs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3znnmndqn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mmhhiztn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ojnxesmq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkarunty.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3uwarizap.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3moviomkd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yalhbqdn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3frvbbrcz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahktacih.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jpwbwtlb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hfvjnuju.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3wuyfcvvt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ptkopivu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jpmqkdmt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3vpfzgdwm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3owaaucuv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mttrmyzt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbqsygmo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lqbhgulp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3sgrobtfu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kbmfyjeh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jxvbipoj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bbypzlij.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cdvuqsxw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ajcjqbmj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bygkkrrn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zinzxvzi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nrnygnzx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3arjupljw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3feiaabqb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ciynysaq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wksuqijf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fpacksfa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dptywhkj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ekhqkcdq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bkdjejfm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kmvxqxss.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hygvmkqb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3joawgyuh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kfdgurhz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tioelqop.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uplztzxy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3whkpkowz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3joybcilb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aakcmfws.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zqknjedd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ypxnnqho.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrsqmhmq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tdiysdlx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ofszxxmz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tfrqiyuh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xiyuerdu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rdrlnoez.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3akpknace.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3exzobvcs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hxupqbwn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qexnlpsi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ogxtikqn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3skvyqqqc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlhxdpjc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uhjxxdpy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ugowbdob.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wymsrrjh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xylihtxe.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3chjrllrp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3asdmvdxh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ydmafvyp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3usszpoxo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tjcycugh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nyjbscdx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqpolzcn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kpwpgzdy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ebioijye.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eelgjzxn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lhxckqrj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3varvpahg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3clryzyow.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xyuiifig.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3dttfmpms.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqhuvfb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3irvqbjqd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xaxfxmun.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zeypqota.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gupltjhe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rttsjdqv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jgiaffwt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbfvbobf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fjxmyuyj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3hgyfoxcj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zamgxefi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnvatde.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tqfhedhh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3unqajwwm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zvtlhexk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vqjtltyo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cgvlrevp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ushtrjcc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iyilqngz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ordhngtq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jchiavcs.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3cnehvyrh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ljibagvq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mvsegrcc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rycqitob.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lgkpinki.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaawrzlg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbehdchu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ndoswjld.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nihabrkc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ctwmnvfm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3isvjnokc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tmgkblqp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fkbtfehp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jkwdxbzc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xgbpapjm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dutmdhec.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uzslyowe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wduduult.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hxwffldv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yqlalxze.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vjzzfntq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ipzhjogw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vlxfbnvi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kqujurym.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3oforcdyh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dvtmdmjv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3afdhcxud.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3rzuuvjvy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gtbnrqhe.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3yktmzdab.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nzhdfzol.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phoclhvl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mygjzjbk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jypwxqvf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhisebrm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rysgsnrx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yymzefcj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3kpfesycz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jhthpcsb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hvsknbkj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sijwseph.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lypfsvmk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dkosyhkz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ozcwzkhg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3anvnhpjo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3phjnpzwr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3djrqcdrc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3clmveanb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eyvsakvj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xlayytab.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zftnjawo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pcvtmxoe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3aagelrhp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3swvpuard.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ngfzmkxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3myxofgux.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wticawys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vozlohnq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3irjkzrzp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3czgltshr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3egwstmap.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3oryiejkr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zxuquyds.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pmgilxfh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gjlqyuru.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xowpdazb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kadvafif.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtyaaumf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zlyeiddz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3bmndusat.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ereswlgv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsdhydrd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3idrgzucx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fuiytgqo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gvryqotq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lttatpds.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3lhvrtcoh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jdxlsrqd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oxqvjwgx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eglwxlxy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3txonidjl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ofovgbep.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vwgocwys.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3uohcqlss.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wfwzqlqz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cvdowxpn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ohdlvzsk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tudtinqi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ajsvlicb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qzagbmvw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3rygyqlqu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lqfjzmof.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ounchpcm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nchbzqrk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nwpeupzh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fhdenkop.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3otmpojwr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjrnicqi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nadhfzfw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3quqlzqlh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yyegtisd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwtwxrif.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hguialgw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqbdvuzg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qiafxynz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3imnvdbxe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qehjtisg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtggfleo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fcxodshg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zjhtzvsc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubvfjzzj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3txrzfzsn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3locgypek.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjhzrxi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bmushwwb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gzhdniaz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qsladodi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3hlzvkqiy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3djcdmdev.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xdawfxno.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3iqdzhidv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xkeiresl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3shxpwxul.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3didplafn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3huepatfb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ydptycni.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxqofgt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ugwjyasv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bgegwlli.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fvzrugxz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zozxrdev.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnaeczfk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eycgmvwm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3odrqddmw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fkzuimnc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tdnbvteb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3okgawfpz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thgfypdr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ljwtrtso.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yorzjgha.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idbqpifl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kjhsxbfq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csdegxos.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onwanmrs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zsssgfxq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgtkbupp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzavkrrs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzksyiro.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tngjxkte.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rasriyrk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3enwctckk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmdejsig.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hnlslewv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sfwhmnmj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3cdbljvfq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxsoqurw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pykvbvan.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cpgthilt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3fdnhvqvx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3emnelwbw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ekcgaafo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jgulfima.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pdspdehi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nfhbfeat.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zatwqokh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dznxeaud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjsirieb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dgexxkuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnccdqat.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3wglqbqct.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ytdgrhhh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3uixyrsbx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzybgotp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3peamtpph.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3eokztglc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xjvojqep.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mzjzwnig.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3naqvrfbi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vkmpvfaz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jbmbxiwu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dsvtexrk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3owtboyhh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmuorucs.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cehsqsga.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nznrawmf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kojyejhk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqrmgepp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mpifluwy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zexykawv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mglflami.html


<!-- 参考信息 -->