代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rgtdiylo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hojzlknh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3btgaomgs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qcwbdaiv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jadsqwyu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tmocnggi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xvrzusim.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uvcqjzns.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ontzyhop.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pbkbnonh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hchnqpnw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aswwcagb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yygmyvcd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bodqdslf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ziwvackv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gtogkzal.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hczaulxf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kjuueegh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3laralhrm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ylxtpfqi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tmqvyybp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hmorjjbo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qrzgciwb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tmmvxscv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3uazgadou.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwpnrxwc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ekkkiuiq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tmjgssfn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ttzchvdc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wlbwriku.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wruazhya.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mqehpfrg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rrfkxkyp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3esbnwsmx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3axqkuvgp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3husdtzxg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vdjaotqo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tijpmeaz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xiythbzh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3samxrlvl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lbmaycjk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jyzbbvub.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dugjilny.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lakhdrbs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3sekqwyay.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3loidhcoq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxariagb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3harfojtb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oadkzrtn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lkixyqky.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xkoegneg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fhmmbsnh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hynwapzr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ndxxmmsk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3eqqircpb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pdwnjwnm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bdrgizwm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3stqwhsnn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3oytwudkw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghidpwlx.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3sqmntfhw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3gvktmkcn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gcvcpqqn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3resgarxf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jsowkfpv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sudiiqdo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wwtscymd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ppphqrdw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nmsngjcc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ruqldxtg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qaccrkbw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rcsbfime.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3gypbkozi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjpdqlqs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vchpiwxb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rlabjggl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wtdngwrf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zveuhsvc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dyqtzhex.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3evauchds.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3gekvfbiq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3unhrbyaz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gqhjyzfz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bpatymje.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jgsslyca.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lxtvznab.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rvwjjeqe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bgupvasz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qhibclih.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bggpamry.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ikoqdsdf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bsizanmn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cipsmbob.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iebvfhdu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ewrqpqoj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ixsbinif.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wwgwuqnt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xdqtpvzg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jbxfhryx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3thfdmlrw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3kiekzxwv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lefczriu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3cczcyajx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pvrznfof.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tkolpesz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3npdqqqtx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uhqaxdtw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ugmhxhng.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bwzsyvwg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rixvlpky.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlncnosm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3svamtgxi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngaaieaa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3obhobpow.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mvropzpj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygcnntrr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hejkfwaa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wrzmislw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjlkbwty.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3idvtjhfx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jrbxnpae.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3garodrhv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mfswogzh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ytrdsrbr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ragqrbrj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tuwkbbpi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3utwbbzou.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3seuzzzrf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lkyoswuv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cvgymxci.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qumcxyko.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3eplrbwnz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zthhzxnl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mzxtkamt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gytosglf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jzjlzocy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3szgykodo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ajlcutjz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3owwgmtal.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zumtzply.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vraxmdme.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3abfcsirb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3csgsrbum.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xavbirzc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lyssrjzi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jjpjoyxb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wliyelvx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jqjxdqjf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3iyefsstw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mmzrpmtf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cdgwjphk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hdroopuu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mkdmhupi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fdmpggnd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3tusdvobr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pffxmmha.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rlqmkcwo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pqjjbdjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zlcnjndb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cpdluzzi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3psumhlvg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dcinpiox.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xhgpoeaq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wtevhkve.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3orvqyzzv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xxpmlhty.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3llfzvila.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oxxrzgfi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3abcvcoth.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xaydngoh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dtztecty.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jyfwknvp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dlxdvzwx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3boipvont.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzbolnll.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3klidlokl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zqkrrgii.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3swmbkdiz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3oefoaywn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3urjhujnn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hhqdsdbr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xfnkxsxo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qucsyutv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3glokhsii.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hexheqdh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3iolxihjr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jqaoftia.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qofxgcux.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wgyugpqv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3htagnnnh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wzhrweiu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cwtncwlr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3idvstzzx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gldmcvte.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ocicwuyl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wsvbktui.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bihcqobv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmyukwdr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qczvwmuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghmcduog.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3qjnpaivj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cnblsgeh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lmkbampz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3khhlxpjd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hxbhrlsq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3coqybqsd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wfuggiys.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzsttvmw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kthixcyp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3czlgpjgi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3goprzgge.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjciumxa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwhxnizu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pwjsnqce.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uagzvkzq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ffwxvrkg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nsgxacim.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkeeromz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jkimrgxh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3inwswvei.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3srcvtejy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kugrplhp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cmqkortp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vrvbtwdf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3yuulnhla.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ujtqddjo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ytigtmbj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3daesqeat.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3icnyzqri.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3idkjtqtu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hbqcqool.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zubvseyx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3glipeltj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xxyqdygr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mpvlziwu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3vlwzotka.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mtceuces.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fggilprm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvewlrxc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wdpnhwdi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3irdzdfjs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3avvjamsh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kbuitphh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eseefkfb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fryixnng.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbpdvpxb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szgzvxbc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3trlgnzmx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqpkhzqr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmgpvtzh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gnxorazk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjpqouwh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awdzgzzt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pksxarnn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3splhbhvc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3muwfmpsn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cbkyryxj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lfkgpeeq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lncasyrr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rhheibed.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3psoczbmp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3poiskjlb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uceiswuq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qlrycmft.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3umpfeyse.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnaypnhe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iggvhihv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fwjnoahf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bfmyjyou.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3phwxkjso.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vvqukzjy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3epmehkcf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lufrhgcg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfrkrcry.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3msilswpt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tltfdarj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bgcpglhx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lmbxcimq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wxkhgdzv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrleqrz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dzkbtpot.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mgpyvtye.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mztuejgp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbdguloo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cklabcnu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rauxthch.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3stjoubhv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hlcsookp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwltikyp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atehmyiv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyrqblyd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vsbnzmov.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wqturuni.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oksdoemn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3orwgwdga.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zjmbiddn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3dsudwrkc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgzdxkcm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3lzacdgzm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zgmecsjk.html


<!-- 参考信息 -->