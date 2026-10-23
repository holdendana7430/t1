代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tptafmby.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jsqvvrdf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mtgdpetr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bxkmslrh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qjfbfmgp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bpmsklsd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tfkreesd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hqikskhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svpzzytp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gkcfwaij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stdmvkha.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hzhtpost.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3viqnowvi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tmftayps.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ekorzshs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3slmvhqdv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3yqmmuven.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3phdyaefz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ivxyxugp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yvfpxxuc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3abjgplqh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3irtzvjgk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wofkilfn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tyqweitq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fwopfqem.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3btymdgei.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hjxwvqhm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lchvebgk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lwtddyrl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ihwxefty.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3dqvfyrpb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3akkklxcy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3weohskub.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vhbruejg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lsgqtcwq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zcidnjpi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ihgvvtkl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wolvtcvh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3idunngfo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wzfsunqj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vrchtjbt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxlgylk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hwelpxkv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ixyzxjhr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3czcarbsi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pvkezxqu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ctjaczcl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3loyfwmdh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xvtzhhdv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xkjlmryg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3juyuedpi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3bdrwjtsq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gvmctnwd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vjelmjtq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tfiugtlh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sxdpzzbh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3egntgmqo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfcgttjb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3cmgdyvrn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3juendqli.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3akbrnscd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3woazlhsz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3shrzkalt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cwofxmve.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3edxyijft.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3otimaflr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wlipwqvr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hbnmjjay.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ahrqoqny.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qkvbtwxd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fyzfmpzb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3iapnwebz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lkkpvzfz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tqygjxzp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hsecdfdm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3nllqyubj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hlvsmbza.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3igpauvpq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qygvrajz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xcqswlgj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3reztcozw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kcigubrb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eihsoqyt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mqoerlll.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3gxodtlsk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dqioueaa.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tyyacqgu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yfnjfdhy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ykwjesyb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mjcavtut.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3iijwngqw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ezsokfou.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3uqihwbkn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pkazwsjo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gwljneeu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iudmojfe.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3omjlrfir.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3seodwpqo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xyjnszdc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rthmrqkq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ijpyjsba.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sjtqsblk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uzbxlyep.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pknscvsc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3srxspsis.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rwnjxszh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kmhaiuih.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kiwdojpp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sotliccs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ngovyjhu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3btscqdhi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3axjfunzb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3apauiyve.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3owvddlkw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlgdksts.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3eqhmnsnj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3uobjxwkw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cktwkojo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ogqpqiye.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3iagznocc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hjztihpm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3irdxtehr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vcwwjjlf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqjzpnmn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xcakdqwb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tfgstjvg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dmenpihf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3owlzmkkd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hwuvyykm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tlnctdle.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgvqknga.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ngiyluxb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hjwndssb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jysodovb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3krsftfpk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cnbscvur.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pdbatknr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ydfyhnki.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zexqruao.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3daailfqh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3aipypvdp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3oddefvti.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3whawtrzk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jygnvlvo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mgqjgsvq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjiknamr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ivyessdg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vwvhboch.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dgquyplu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ddqfdlyj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zmieswyf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3sklpeaqh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3uwohtrok.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xonlhnjo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3opjtfypg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3psleemgi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zmvfnvkx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rcfsbcrn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3waespiec.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuvgqti.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hrsjkoum.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rsngwnei.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cvevgdni.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cioeremg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3eetzwkyf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vccfodzr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gwahovge.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3whszgetp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cfkrbsbb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vbwiymer.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aihhgsfu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3upyskwlz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3enrrwbrf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ypwppxij.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mkfiudmy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nxwpxywm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjeqoxd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bhjyhytr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3comklsqd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3axwofszu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wlaobbsy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rexasdsl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3lqfiwxdk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hkmppvlt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3vedcrevu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwrdmkwd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jmblhkqw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fgwelrep.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3uwrkouar.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3pzpyrnfl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3neljdckb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ywknwqab.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zotnumvq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ykcbkjjt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nskvbbgd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hgcfnudm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dtwptuyo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3dtrxuzik.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3heudsnlf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pantrspz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3oztciumg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zuzgpcjr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lgyqcwec.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ccsquzut.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fgiedyij.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3oldivdle.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ofihrmtj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bctvvnbe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3oxruutzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seaeeukd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ciolxasq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvoxttqs.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3eetzerfp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3stwcawbu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nehyqkhg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3teluaebg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ulpedqvd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3amkriheg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dknuaxks.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzyhfwpn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kxmlzhbx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgaookqb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gthzprog.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nigmysnp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqywzjwu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gudiuxzp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tjnafghf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wslszrul.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cakdwkdo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3prfpmlec.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mtdwvndx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3sheveray.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3luwsgevd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mqkkzard.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vcgctpdo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qthvkwbm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rkkmmstm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nvgsigtl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jpvknsgy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftoiymgj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fslcazkh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nkhsnpgr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mnjybyyh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ppgsnkzr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3rqbihuss.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3reynuppy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qjpaxsta.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3koijieuw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3iojouwia.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qnximtrx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qbkxtnpa.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otwxdlea.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkilwovs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3riiyweav.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ulzenwiq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hibbjqqt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fixojrru.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3awyirxxl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xogxpcnw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fkgfiity.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydvweilj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdccnfui.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qdhlvivs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvzvkcec.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbmjohig.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lcbmvnpt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ewsuhzfo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xnmzhjoh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lxjsqkhr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mbgpvmug.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uskxmvwm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3gevoykhf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3sotidkaq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qgyfhsng.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3geipbowm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ytuhpmra.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3guurtrje.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dmubebmb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ksuzjdcx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zvrcdepo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3drzhzrlx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wynqpnfv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3avoeykfb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qvmjqyzi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3kpkjuveg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqycnmjx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhzqzlne.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3apzrvpze.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fvcszoit.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aqwjfudw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rasyjcqt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujuzqtpk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rwblbtaa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hqnnnnux.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ozqpeojs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fliaqgue.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilnvxfbp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onuymkkc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cquirqkt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzkpdmxr.html


<!-- 参考信息 -->