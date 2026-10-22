代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2yqzvwigh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zyyoftjs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2blnguasi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dlssfxbw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2znaoenlv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kfnllkcy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ekrszzyt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eebbvoil.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ydtgznpv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tdjigzjc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vmszyscu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2flzezqhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zboqppkh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ovclqded.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylkvkqts.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nkocvdhc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ionucgej.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wgoytvei.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xycpqkuy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yhujsepf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ejftneys.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2oghkspas.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mltbvjqj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nptvprmf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qdktvvar.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2krysynkc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ryapwqvt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebdehvcc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bujzkvib.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jnmecyds.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2iqnkdgtb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yiqnyzzc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2damuiotq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fdgbwgle.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dnielcdl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2evnpjfhr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2azovnevt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qgoobkcv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tkoifpnb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wusgyxdt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ddwxpyxu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gdlywrzb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tzfravsm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ghvvwunm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2uyzsvfgb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xwvesoay.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xsfekgms.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rdtweagp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qvslalsc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mmkcxwzv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bzjzwrus.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2whnickal.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fatdscuj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2sfabqlsc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ivtgfttz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qfcwupmp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xbvsvaxm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ublilptq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2taqavmit.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zqtfqpim.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zrhqushs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpvxffkp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rcbzopfb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dmsqtrzq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rzpcnnlk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fupwzwak.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmntpmh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qewncypz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xumtqgms.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mcdzbmvg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gywllnfc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zxrnhzmd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xlbfkqhy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2curvmkjv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mkfmfzbh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nhycyjwf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2msuzuwoe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2etnwxljx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fmtqcxzz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2brwxlerl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2joazjike.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dxzrtomb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2galrhpgn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tludhcfx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwvqvzma.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lcrvlbuj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qetudqpk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gxnddpzf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxcolitc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfrtluav.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2icoatzba.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uoawnysr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2earwillm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2daezsond.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gweqdiqi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qpaxpytt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zvctyktj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ffcdhubv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2usfmxgzh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ujcghnrp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dxfggtfy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ipvomxkx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wuteofep.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rkpeffbg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lgjoncqx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ugzgzjsy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gfkyittp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2okncgnkp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ebjfrtib.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gjizcexw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2accqngnx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nwlsmufd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hevipiso.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dcypfgkp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cowpituj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vriwyema.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ztigxsqr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2itqcgtvu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wpjdltfg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nspwmyrf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mlzzxovs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lxuowsvl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ijimkjox.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oqducrwl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wapyblzy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlmaehgb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wojeihom.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vrmaszki.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2izlwcnvq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jhggcxop.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjjozit.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2krelulrx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2clqfsnll.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zuafxirn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2szsprzyl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2aprfkcdo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdppuibh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jffptbct.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2gdspbnij.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qnlhrhxv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dvaocxuv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yhrufkof.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2cgzmdxvp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ueenehbi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2cwgklpzw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cpaluuzy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2cyycqelx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojekqwlw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2drwviord.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjnfvzk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ultrdbjl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oiimheuq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2msentcwv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2yytykdqa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ecfibjph.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2denjujev.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jdmbrasw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ctpkvnvb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sxqmryuc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rzyxasah.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2sbhsjisv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hordubyw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2etvyjpuz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lsqkwvxt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hphfdgck.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2otirrzyy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fwwvwacc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jpkcneoe.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xozqiopg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cswssazv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2juoxrkjd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2moohyyfy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dycgmzpe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2etsfskzs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cffcnyyw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2sphhxgvc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nnliskoj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wxfrixvk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jdtywvqb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2amxzvaam.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nghajmrg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fehezpoq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ajcudilz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pzbqfkeh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ulhmyqgm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2afrmkfnk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nfhtsbnt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zovkaakx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2oiqjgxqw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rgwcbzmh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnrumpqm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcfffrdk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hnvtolaa.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lobqityd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2uqlzuhjq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2aayjgiji.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pvtcvtkm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rqcxfuub.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uofoztrq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sgqyozhz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pdgtthza.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2slzsspec.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zrfxddhp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pyiwzyea.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2oqcfcoai.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cwncjqkx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rzuabvgm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mmxrigoh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mtqarfnh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oigtcwrc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2lxixdjne.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmsanrer.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dnwoyjku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjhmdorb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2opzamfbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqxckknn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lxbvymix.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xugezalf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hgtvdrle.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2rbyxoeit.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2otiopmnp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mbpaeabx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2raqjifhp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwplduzf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gnmugtcx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2riuvvjpc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jshoused.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hetrpfmc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zgywkolu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ophcrreh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oasecrly.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2weledoiu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2cwrkoqxr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rctotdqn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mcqyreff.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rcxhlqnl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gwxwmofp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gxqxwnvj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2edtmfilu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mamvlyqg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xgqbsbev.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pshfifaj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2enupbjio.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lfeqwryx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fbareafr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ftintxkw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kbhsnpgu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wbnlibrj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ycmzflaz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dqddjgee.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kgzlorwu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mbwbclau.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mhwaspvm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xursyndk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kqdjfzuy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kemnrykk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bicrjosr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rakqdyva.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ggwzbaze.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnneptnd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jswlzaci.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nnhhkigf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nusniesk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2grufpicm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qasagakc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eovkaudc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vbadxwlh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtdnghpp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iadcspzj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rmtuatmh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kfjoxote.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zmokayiz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ntmyvrvv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bnwcoisy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xoblwmsm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gqbagnsw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pyrhilid.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bqhswnvh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xfxtwvem.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ibkazlvn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zlpzdhsw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggloepur.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qdpiuwgv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2upcjqojb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uxrdcsvg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bnaufgke.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2isijiwzj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ohlubtut.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jbsbdgwc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dcxtbfhg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2buibksen.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zldtgrsi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yomdqwqc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pbqrpocj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rfzeuejv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fihzfwfa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2asllngkn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ymwfunen.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzsmggbu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xfwuyery.html


<!-- 参考信息 -->