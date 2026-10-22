代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2iuamjvow.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wmtakuvx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cnltkqfq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cfkxtlnr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2axzzufue.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2skvkyxgg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nxwiucgi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2amhsfzfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqshwraf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fjqgyfon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgucsvoj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mrjxmiki.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2dhpgmfeo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wdidoabb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bzlifkxo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wecuhzqw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vsjzuxle.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2obdktfeg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2dsafbioi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fqyegzur.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zutvvefl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2okcdkcfg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pozcekam.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfqnnbk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2idqrgfyi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vskguhyx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2dyxtgqng.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fomceyrt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dzxxfvdu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2okbodjkm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fnrrkycm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oxrvdsjd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bmlcomny.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ihotfsbw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ivkuuhlg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2klfqilnz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ghcnielg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mtagycqj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mipdcgny.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fwrzbxit.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tnilwpgp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2afzreagl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lfxgggob.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2teicipko.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2pvigldgh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hytpahhk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eclaqtjp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qmzevxme.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2iqsetpel.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ouqxafzm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2avzdzbtl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wfbbkrmc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oypcvssg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ojwbwvax.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2euyngytt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mkucaumu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2eobpnduw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jyclgzlk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ffnvzztg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hqtfdayq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2imytkusv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ecrnaqiv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zptqbqaw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ifigrgdq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rebcfimr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xzhmguun.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zhkzpaxz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cfbtavrl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sxengndp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vdoexgyb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2etapccsy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dzxpadkf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cozldxmz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cfylqhma.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wsgedexb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hxopkxmt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vqokiaac.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jvwpcllq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ktywlixy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2brkmaich.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2oncovwqy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lsebomrd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xurnmodh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fzodgshg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qgfekitn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yzplzaxr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iiieglla.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bwxvvulj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mlwpkxcg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kuzyjpzf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qycqrxtl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rbkfmcqj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uzbrqtct.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rlmjwhft.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2stggxicj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xvubkpis.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nykigsut.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xwvmpbzc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ahyrqgea.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mpegzqgo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wnexlzyg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gspbkpyk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kziozpvv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xcwtgqfl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ifljhzoo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lqpbzzfa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aqwzyizn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jnbeniyj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2auaobqll.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gltbjzcc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2avtnxmur.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rjpflwcv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2suectjmk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xihtphei.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tuexbtpr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pwcofzpy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2wpubbtaz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ipwpqubu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lhapqbnz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xyzcwpfa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2snylxutz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gcmdmlxw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vpipmemd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kgkzjkzp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cydijmxw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zykfconq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2zzcpxscu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzzhjjvv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tidurklh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qrgdwrpb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2vriklbim.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2uvbyhyhr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ncogmixl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2osgkfnnq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kstxpmpe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yjmgcgza.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rrofrbdg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qvsxxvxz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjgobyu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2drkjyuvu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tbriglxu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pznivxqx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nvbuqjfk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jwrvptyi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cvudvkza.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ygysovdw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qobtofqz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ouajfnei.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xkeaxlgd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rduvzjmk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2thtihzqv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tmeydeds.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wsjiuptd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tzpnbgyv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2holfryje.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jpmygjqv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xkxqojyt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zodhdxjz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uqahchoj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyjrvekp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tteathdr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jlhsnctu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xxehtxkr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vbaxyqdp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2brbfttxf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mzxiksqu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2juqbimju.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gtbpbfoa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kegskigj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2clknnwor.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hgmwrcce.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kyirlcmm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2doaaanmw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yhlbxdil.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wcjyilji.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wiipipcc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ubegzips.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xeneldvv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ypvgjrhy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2clqyifop.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2weodxgxl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ytbqmtgk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qtcafsza.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mgwtmwkg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2clnokjjq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwskxaxa.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wkxvrees.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbqsyvym.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqehzjhl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pznkwjqv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kxtkfbud.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gmrkpcpj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2agtwzrsp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tqyjzijc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2atwtlhfo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oxtymnra.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nfvdeygh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qnkbnupr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xdaglypi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lfcnzrcv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qwkqhyni.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dvkruwcr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kxwrdppy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eadbaknu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aaiwhztm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2idysagml.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fojvjlly.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ijdwikzz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gamtvxeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydlpzbje.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hdnoyhyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypkszflu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2asiyvqru.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bxxsgqcf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ajzcpvwp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fmnjhckk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zqhzwhrj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oykabdsr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xwrsfavp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfjcjtwb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rrtnhtrc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhtwjbbc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2arftiifg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sykznjfg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbgxvekp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahdqgaah.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ocsaaewd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qpyqkeot.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gdvqmdbm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxuatsfo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qbltvbnx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hrmobrel.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2abiowocz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vpdaznel.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ttlhublh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bmfiksic.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fqlioant.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pogxhmdd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fntssrwp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrumevip.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oelffwtw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ecgfmmqo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pcakgfkw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pxclsihz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cxicjoxc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ponfrwzh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tstnqxai.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2spinabpo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kfxjvxba.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qhkohlcc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hsdgyhce.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hssltigi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzivmloq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yymypuwd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2tauuonsx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qmeoptuw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krixvsmq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2crhyigie.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxbngmyo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zqduuesm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yjdzdxwk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfyevvws.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcnqyjek.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wdypexif.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqrqtqyw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tfczdyfx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2fqwwnvqu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bgwkxggo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nkyxnwwi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gzjmtwky.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zqzkdavw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tggzvflq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxldhax.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rxiujqrq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lzzmxpnd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2roznopwc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2upeqhsdc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2iptjxilk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lejswaxu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zqrkgpzh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ztxkvtqz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ayeaepgr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vbtosidb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qqipvpwb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lmwfkrqd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aipkjrgm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bbuowgfi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mmmueyfn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rmukgxeg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pwlpskvr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qkfvyzku.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpafqlos.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jlljvjap.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2flbxnxlt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdssjvag.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejbrernr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgklnldw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fknbjjze.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ylpjavpb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzugubih.html


<!-- 参考信息 -->