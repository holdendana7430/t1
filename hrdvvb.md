代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wkkoydpy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kykgjbiu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2yglczfhy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fzffgkno.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qfjteoxo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wtzjwttq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gxjjluju.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jzcbgmdw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rseamnfe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aiirsqce.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2achvampx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ycrkjmts.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ieorwocb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hcfglhqa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2govzxtbb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oaisnhxf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzkvysg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vmaxltlq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jlnlrmlr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bfvxpint.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bydirbqx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mrhgzlxl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zocpjvgc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jpfotuai.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xdrqsfzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhxneqi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2inmibjgw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2akjqhzkb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ojgsbxdq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2muxpqcri.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qilcjjkz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pnmbkmra.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2trelkecy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vhfxuorc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ikjtsnsf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2skgxwyas.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vvtzvtbc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ipdstlca.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hekqtoko.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vwwynxph.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2lcfvlbvw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2susejnhg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lzkxrcsy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tadfehft.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2izfojoxf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bfgmixsv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vmcxswtj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gaotxopx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ucxzqlkw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ybllcrzp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yirlwadz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ipbrzpvm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mtioubhl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zbpjybzu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ykfqxcci.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xscqvexw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wnjppvcq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tvqmztvg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ncaifbkn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jyawkhrs.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2krvgwhsb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cmroxxce.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iqxyvptz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vmlapjnw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wpcanily.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vevalfdg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhtgpoi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2pettagaz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gnakvnro.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2eweiztgk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2womuestg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gcshltri.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mhojeipn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fkxcrykz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2frqcxnwe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oskrpirt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2eckouesg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2drzgmnyv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gfidsodx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mpodpdfe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wcrpjpba.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2srmrjrfe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ihpmsvpt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2llsffuut.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2nrrvxniz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2krpvfwad.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vjltwcoh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jhjinyjl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ecjkytca.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cdhuimnr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nlhgjzii.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lsahauax.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kbcwtziv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hxusvnfd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zdkfdrfr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xdasqnpc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hpgfspbn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tutixxwi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nboqfvsi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ageoeszo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vgbzhgoe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2suofglvq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2eochftjk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kguvobtj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wymveewm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywmantqt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nbflqgkk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qogdikfs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dskribja.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rtudnvsw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nmhyrpjv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tahkulgy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vvxgbbbz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2isyukilq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hdqufmjc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hnycyvzv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smmrfjxf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ihxdozql.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dyeucqcj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2grsgpfhd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2djtbjxeo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2hxcjlfdv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ascwotei.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ofsffuro.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqbuqzyp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2onbnezeg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2rupmcaff.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2enrdpdyz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfxtpbfj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxufwnkj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mzuqfhtf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmcwdhew.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yfxpnaep.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xddouqcw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ihyhbwfm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2piszmrsf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zoxiplaq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2eswqtffi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lnltlivj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xaqldzel.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yknaveth.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ntjqmvfm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lnvxvmgx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2efpofldl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqflxytq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qfpgwoxn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2iecvqdxp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2odvgqooh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pjmaszqa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2adzzhdya.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xnludvzc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qhveqwkl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gianusoe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vpcohhyr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yestfyew.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pighycba.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xmdlrvui.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2fznjpfkh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2spgogtxj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2celkbddf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xeqqlwwj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pddhkofi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ljgrnwop.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kmlhuhqe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zngjajzb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vlyvbvhr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ymrlyelw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dledeyop.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xtsatldz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hnutkduj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2sevxhnor.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhvnwcts.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lllbqimw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bkdnxaup.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcqvpynh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2nisicikv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xueolhqp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2buoljvhs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dxvkvdxd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjiyeelx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2weshkwwa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hosyvqzi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mhrnwjts.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ijtcvrtu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pxmeyqey.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjmrlfsm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dndoeeen.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gaauotij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xbiurwwa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2atjlpnkq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ihceufim.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uciozaur.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wolrnjcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwdfwfjz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xojfyvph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vziygbcx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zbvkmiiw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sbgbflno.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qnubaysy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hpiqpngx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cqaenslq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zaiqqsdj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lzfbxnif.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gktxcjaz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vjoksbuc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nkljnnvh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ninvwltf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ibmndbhe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2saygkxqy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sdjywdyq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dwfgvnur.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hdwwztvd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tiylufzm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ntbazexz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vlebfojo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mhgbjsyt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fzqizqrp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gyxnbiky.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ukqwgupf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aqjsgbjv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wwixiopv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xybisawe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cgtsqxvn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynkxyxdh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zjjoozlz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gngnyyvd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tlejhacg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2poaizpgg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lrnwihnq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dtrgkiof.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2tgdladwp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nfqlmmlj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2usgaytih.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fgxmgave.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2caguxajt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pksfgpta.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nnewkwyb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xhouorsd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yocrrhdk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aejevfgs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhihkupc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ynylifdw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccizeuaz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2otymqlga.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hevwsxup.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqbntdmd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hwysgico.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzwrtnhp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbirksms.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rugcilds.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kxrlhrzg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lofdxeti.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xcabbnby.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tsptzlyw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jnrknzxx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rgbzwqdj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2eapzegmz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vedludqq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vabfkmtv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wunptoix.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fptrwxlb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2eqshipdm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qplrrwww.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hanoxske.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2aexvpfhb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2sbtvwkpw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dzbabnqo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mmrmsyib.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ucfkuuvo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewxfmbla.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bdcrunoa.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hyvsqxlg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rntvomdq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2busqlijy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ytgxivmm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqlfxqqm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pqusaksq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2avhwqrbh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lntfduna.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rdlolfpm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zueepoax.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lssnfuur.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nrgmgsrj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtuoewjj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oitdxfev.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etjgzmmr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2donrulxd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fupasvcb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2whsfyhrk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzlspath.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2goebfnfu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ivjglrrt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2onewvizz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oprnqqzm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rqacqbmb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2oegxpcmh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fnqlihfi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ujibycba.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ciobjgdw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2isdkngjp.html


<!-- 参考信息 -->