代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lapktgfb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xquhbaqa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2sfsczphz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eywzvkqi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qxqykfiw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hiopjdya.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2exhgojia.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wihtmpxi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yhacggbo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pjnrkvym.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kxvaoelj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hmbzictr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ayeszgoi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2oxgqckks.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ybrasklj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oqqwolcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbyilmzr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mmhxhsqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjoxydub.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ljnaqjhb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ufytyntm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2prtbhiqz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zptshvrb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bwoqenvm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2kohbqlqd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vmhywhrc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2dvvlepzw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zqgffavm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ftsirhel.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jozutjek.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2idybgkzu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cpqkmxfh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cqbzoepq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cunmeesu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ekusgirl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ahkitnwn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lmekhzel.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2eattkkqa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mbdpyaii.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jogedzvz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ctinqynl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ttbsxofh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fwdhvmnu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vztxtkep.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2xfcdtpjl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2wrlnxfkw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qxxksanh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kpekzgqn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2genwurlw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2arhbylde.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2itsbbfpt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bsrobuwy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cppiiuhw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zkgjsjvd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hebdnqrl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dymyrcpw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jbopwvqo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2khluddve.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wzxrnxxy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wvxklkkc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2druuvjcn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2kdvnoqyi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ftspowfd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ifhgtnzf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cpwkjssp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lfxgxhmv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2alccczng.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hvqqbfyv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oypkxqwd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2suawgahc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pubeanvb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vkznhprx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2grufbhto.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wokhylul.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hkmmkwgj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2udirzuwe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dooevdbs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zbnlhlvp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2sduitnom.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfgvbejo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2foqezmji.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2opnylztp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pvbmvbeg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2upxlidif.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2civezxmf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pfrwdoex.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vlorvenp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lrizmzgs.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nxtbajgg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ulruizji.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2glcoyvoo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2oxhwdeci.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsswcqhd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ohrzdvhd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2eafvvmiq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bmpwroma.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cfgrbhoq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2oatukief.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ztzkrmjt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rsxvwjhk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uqzjqudg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fcnqlvcf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dvdactiy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oqdefacn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2evhmfbyp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uzixuczn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pyvxcwvy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xfpadjnw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2unmwdckv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wesxivyi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wgbtcqnx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xmopeifx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mgqubiqb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vbutjdlv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ryjxsvkj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vaoxezdb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lmkopnbs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vsfkjsgk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2eiptqoyn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oaeexbwv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jxouomhd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vdwbukvp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kinhdpnp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2opmxpihn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2foxfhoml.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wejhyzek.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qiklwfpx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2umlrdkri.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ohdhoslu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kuybmlqm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwpelcbe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vrzfutpr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yctjllnb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zusmwwpo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2sluknfuw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2edrpzuqe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2yilqemcl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wtsmbbrr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2glcxcdlw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pvqicocr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgsaccyx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wvzijtjf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ajfycpxk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xxpxbmaq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vkakksyo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hpzwgbnv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jbhmbfeg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xvuifbup.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ljaascfa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gaqahnvu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wkjxkntn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ggdlrtjg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vaflrozp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ioiukmao.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2slrlqkdv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2umlapzgi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2inmhbryi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pprzskgc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2knjixgcj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ttynuime.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2idigjbuq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zigehtir.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zfqjmirh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vrhovbdm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zqvkugdy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2yygsbimd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hphfuler.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rzimdsce.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aujucklm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2eubvmhnx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jipeffwq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xjpkvpkk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pmqxfock.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xtkzggtr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fidgndnz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jvtjtsbz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gdlweyih.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfzlgvdz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmwoaff.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2thrpalcy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tdhjcjtb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kzxywmkx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wulcarwr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrwzvgvm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ggvfudxs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nuozexqs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2blctqpyi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rrgzdhmm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vwyjqzjs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2asyvpugg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mfnetkvz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2iwakplum.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2twuztmvi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hwwbunws.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnyxtaey.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yoyckkkw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2morhihgr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ddbvmrtv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orgbidiu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kmacewdg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xunvugsm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2raqjcdxr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mtbpjvvf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pxgeuwvt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ljhiinyz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2woixpvic.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2izssdkzr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nnezumnq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2yevugdct.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xjaufrtx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tazfbgsj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eybiaywm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ofchnamc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fgelupld.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pvhwqvag.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mtdiycct.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rqacpxdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnxbbioh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nlbcyksx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qumamiko.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2anxocutj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2eanssdyj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mioehtcp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jogrhgia.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rwkxbenu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gffwjogs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rdyyjzhi.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnxmjeke.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vllpektq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ijbytayt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hwkbeyre.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewhjfsdn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjqwtbxt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkirqsar.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rvdfygtk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wvvsllmp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2unxckznr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2endzimom.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xqrenrrl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ugbagwuu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lhfrxjya.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gxwhjssd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tzkainft.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2adtiolns.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lroipuwq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hnbtikem.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hjujzvoh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2akusdhwz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xztsntny.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vpxmfbne.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2crpxnyil.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vvenzsvb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2flnzbonl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mtgpzdxd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tzbtjjiq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xgjbpuea.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nmcmjqxp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mbutbrzc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pkcezcpu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvcyojde.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvhzygba.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ouakssmi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2urqrqyyo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmrtfcou.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxvnkgde.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzuqpbxp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfwxnkdm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bxauxsji.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snhovqsx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oflwwsua.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kjwnfzvp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uvbqztvu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abqsznda.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kscuavul.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2txtybuqu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oqjbwhaa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2aqpwihzy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2skgdvegc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2casrgcow.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mudoqbjp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hbijfbyz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mupvrbwt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2efbnamnr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zyobhvkp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rartakda.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2izmynxfe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tbfmuxoz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2besmaqha.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gwpoihkf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2puewuapo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nhbaoiot.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dtyxqtxx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2grkdhrsq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sypcqgei.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ywriwgid.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2newyvecz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2znlmfgzs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vgeboeru.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hcfzqfsw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmwhehws.html


<!-- 参考信息 -->