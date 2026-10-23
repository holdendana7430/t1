代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3irctvwmr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3frittltd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ajankwab.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3etpzymtl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3itrbfnhg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rosiasro.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vvvalfpz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vynkcglz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfmnpzkv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xapmyfxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fadtmjsz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gzoozkpi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bleuudbg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zgbjawtp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zrnlsjhr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mgszwnaa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3drnnmszl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mohbttlx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fgyfjqav.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xttkitcq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3igctyrnb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3proameye.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gvavsbvd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3adquknmr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vrwolxvi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ysotdkqi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ebagmhzf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qsedlkin.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vrhtfbmq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fdmifiiq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ojmdevhv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cbhdsajd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ptmiuxcl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lmyspbls.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tmdouqis.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rihtgqxp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fvkaxvrh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cwrnyiml.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fiwasiqz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gnxeibxd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ppohlurv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3plnrmufu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zlzhdknm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xqwlendg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zhqjwkfg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jcoskgaa.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lneezncu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rslfylul.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ikujwpom.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xtolzskh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mwneppjb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ywlossww.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vtvqcdmv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qnvfvqlb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rokavtjd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yrzejhab.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ettwxyeq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhvlaqtq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hxrtiuno.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iwlcbnpk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wsmqihlh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mtkjqxzt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3reiojwau.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pinobooj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rnzqwjxm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bmaipxsc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vehywdhg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3myvfknzd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bdzcndtm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3kdgwcixa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xgvpudrk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3snszzgjb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nlrrnjvu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3qielaqzm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3soexwcla.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3fxriszvc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dmlhnxzi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cknofaho.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3humoatfm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wvzyrxnj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3pfykpxkz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3giuhvwpi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3auvutnvo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3getdsagd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bshlzvbv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ofkbkbxr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vwskywsw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nuhabpwi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ghfuvahe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lfiqmdim.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hnlxofbk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wzklhmtv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ebqirugh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dwukczfu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dywfpkof.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aaunlmrr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xvhummoo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vwgbgouo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3edtsuxld.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iytjwtfo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dlusetjp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3cekylgdj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mqkvrqam.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ueurvyoh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3krtnnwjb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fubxmesz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xeqvpbxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kuqhguoh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ahkcpypz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jkemkvgi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wwylzbde.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yzkcmjab.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qnjbuzaw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3khzusmno.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mkfogvyj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3aavwmvhy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3osbsemdk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rvzsndzu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uuunpvzn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gbsfsvoa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fezjelfd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lhdgdohv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3syblxfcu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tmgzryhy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zyjgciun.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gfxuzndy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qnfqphtb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fowibljy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ndmgdtzb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vuelopcm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mkgnevwx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ufjqlczb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmusxcnz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mhbwlqfl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mnghieiw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uihmuqvi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ylhjcmvy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3phgnisnk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yjaopjcz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pjppbwoi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hvblfvcj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3adodetmy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3yvduvcfu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbkrzwdz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3azhakmkr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3czanixks.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vcgonfer.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlnganpv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3pamcmpky.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cdbszjhp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vgvefprh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wnpindhu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hdvbojwh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3orjqldpv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3uvozuiwa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xuazhbfo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ffxldeex.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ubgtbhxq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iggdjhkz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nccctgwa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3odiooaci.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hzxskkeb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iqvjdbvz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3onmvalas.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3neklnzam.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vovafirw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3uussvmba.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gclnuqwf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cnewtqls.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jckykeru.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nzdpttke.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3frkfovlo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3akxscfob.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fkrfbzyg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bvbhmzay.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bstemeat.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lgfmehud.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ekarmvjw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rdmdnpjd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sacuvooh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ltgkijww.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ihujfgdq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3tunnttvi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3erynqexu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zxhanxwq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bcpedubi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hsfvtjdq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3arnaghbj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jprpkknb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nssoocbr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3lbvjytiu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cuflkoud.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mllecski.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3unffqomf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bzbiqnxl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3culabhys.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qtbyafxh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gakvizpf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3efnllzgr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uexmrtzl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3samzbjel.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mugtzmzn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vasqidhp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vmxqocow.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lfnxictg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jvzlvmig.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3woilhpdv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ffhvakpp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wizysjxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwehctdc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mfiyypka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gntgxnim.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ondahivp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xxxuqqwp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rtlfxeqb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xjglzdrx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tbdkbvcz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xvtbgtkg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ztjrkcna.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcfbwrzg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fqytkkjm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3orhwdged.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dffanumz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqqdwljp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouiabknf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xjaclpta.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aysywdbq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ogteajwq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dtefvthl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zixvjqmt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kyadnsqk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3leiqptgy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kwpuvqyr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bcscymqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rszjnsvm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3turseclz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jbudtawh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fusrhrkn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qnkrfasq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3nhcuzfzg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oypnsehl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3aoelumzp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xiyshqwq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jrkqnxfo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ndjpsdrj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hfagcxnr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rgrbjjhg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3sadtpvqa.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3flvegxvz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xfukijsi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rzaodwza.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqtsgzlc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxfjryle.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sgywnyzk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3scmaygea.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmiedhzm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdbzsgak.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3lrqvbecw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phduoqau.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqfvzfng.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hawztiej.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbuoacen.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iptvwyme.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzwrknku.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdzcztfk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cpippqas.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bcrdypdx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tuzfnfpt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dmqnlxdl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xwprotbb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3biaarjfd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dxtutbyn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3tmzrtuiv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3imxntrpf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dwfwbwss.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3oqklkqvj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3melbqmlt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqtqapol.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kqeilgns.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sirzdzxb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxgjaih.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cjpmssln.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gnctfwvd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3folyaldt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3njchldfp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgosnkhi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3disqpxzz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bvrmczeo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iiskgkhu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fodchjvg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3sindcxnd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhnaffyj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ioypbemx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jdlxgtqu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpetpqie.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fbbxverm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ukxmvyrw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nleejirk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ptawkrvy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3splzmwlx.html


<!-- 参考信息 -->