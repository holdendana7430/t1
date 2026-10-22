代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sygpytqz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bigaumzn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nfsdcdou.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2myawimfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znfmydea.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fvrlmcsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heohindp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yhuafjhf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zumkpfca.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2uezbpuiw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hssntdna.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xhkmocwo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2guhuqmhv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ilergrjl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2tqxmevtl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2covzjmgw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ndikxwxy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jgdeqphv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jbwyowlx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sgdagxfb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pxbwfdbd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2psubzxvh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2niexwnlm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2emmywter.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2sostapmf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ppwejkri.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ylhuhaos.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uuqldjhl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vnlbmqjp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2capndkqc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hpdglzyb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kbkhygvl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qonnaeum.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2wbsddlnz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2uheiypys.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ontovzvr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pndvzitg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2orgifnqn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2urfkolyq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xaxhdzly.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xlhicghx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tasldslg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qtczpsog.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2iealcufw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xqwrzmwx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qhpycpbw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fujcmkxd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bmhwovhe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yaehkpbg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bgtyvdwm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yhvuurjx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2quclazgm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ygkhhikj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zxuceoop.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rjdabprj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rzgjsubt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ysruttju.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kakoujqm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcfezbfn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yohkqcvi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2argkqwgr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wpzzbiro.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hlbglbmd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tyblnooq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qnyamlcj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bgspdqhs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fymbdnjp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tlockcgf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kxrtmycv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2oafxmpll.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2puqanjfk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2uxajwpzn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cxncsuyq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tsylycyg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fmjtmjir.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2znfkpeah.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mqjcybcv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uerblisl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2eaqpklez.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2sqyvutxv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hvpenyvc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uyxmzczj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2liahtbcm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gxlwigss.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2plzjunvh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vvmqojfr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2paxwnlew.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vwqouwsc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kurmedej.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dfpcinrk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mnzubnsq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2koskgujo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lcimblnd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bpavuefh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2egdzyhem.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cvlbjgor.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wtfwmlcj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cqrgqxmx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qvbgrjjh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kxhzauaa.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2omzwuypd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2saaewwxg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sxambpxi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hylffmgu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2veehukye.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nupcbzvr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2knwujmlt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ztdxzocz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2utjlhioc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lppnmkxc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mahbekyj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cibsuduy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fqkginqu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vdbezgdk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ospntrij.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eitypbvg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2dyddljbj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehophkta.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qxpsbqmo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqucfglp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nskvnpwg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fhjoeyin.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qwffuadi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rfbdriwh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hvftficx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zenrnxrc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2prgjchkh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrjhzww.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2aplvrcvr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hoblipzm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xzckbpoy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kmbnbdql.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yjguxjan.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2pauxyxud.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2noiosllu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pjzeuemp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywuyzsdt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vjqkdacv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2itpjcoec.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjgnhczn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wdayayog.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2irfdjgil.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sbjmjsgj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zkdggtll.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xhxvvpoy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ycmgqxpa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2trmkhlpg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rbbxxwsj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fzwgcdcr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bqkfpzhq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fxfcxdml.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jlobvuue.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2foerkvhv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2skreumlc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mflthbcj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfoyiqvs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ortqlaas.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oazdhryj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2brzcjkkf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ynazpygh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2iocgvpnx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2sxclifeh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2llbvrnqp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kejwhybk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2epdmkexd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2assttzcl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2naekggkb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zilsljfz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sarlsosx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ctyoypbv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2spdcrdlq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tpcarvzw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zlwfxnmn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yambcevj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2sbfdugfh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2iydcoham.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2efhxpygi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ljomutwx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dvkkyqnq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2czlbimrz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fcmqwvlt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xivcelpn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2njrzzatx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2goyvoctp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2iitfrnxm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yzkpwvpi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gggyfwuj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rtgtupsq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2geptirlc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2odploiqp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yndabaxv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yivmbfls.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2voanqirf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2yqxdzgrb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2drzblwbo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kzjjrkft.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zemgqnvx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfketvnn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qxlbwenx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jyldvrxu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2macsskth.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2phnvqkph.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ijovbaip.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nqjizgqk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2drizhuin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ushvzsxp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vjetxwht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjxqeliw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxurjhkb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2yjweohuz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vxelyket.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2frptltvu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kiupebgz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nljvqjze.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cpzfjukk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2grffvtwf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2frhnuhio.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rylvwbmj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2oqggtado.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2opjljyxk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2atavluhm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zuqndyha.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mnrsmyys.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kqbvndxm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gthvplbx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wpcjwvfi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yzazjjyx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bzygqsvz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qhinpqgz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xfyiyqmf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ciqdwoke.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hymbrnhu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lhhcinov.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lypsbcgx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vzsoyvux.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwgfcxpu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sbjrlfga.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2grxvhmqm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lnmtfacg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eoivftaz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2amtpxafo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zlmpuber.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2tnigizwn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fqlrekqy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2sfxsbfha.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xobikuyl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dgvosvtu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxocvnik.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdhmwlaw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fsjofmuo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nvxamrry.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ulbmiobb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfhlqnvz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yqpyufcl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mokssbcj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vjlrnpyo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hltfmsxl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wscyuecn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vvhsuzcp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcjcqrof.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hygkxbuj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oyxyrdzp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vdilfuan.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fghqhxij.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ckngnfdq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2umurjwzz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ukhedxfj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mdxrgynr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lsnekiiw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rqklwmij.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hcjigsbs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lxiwrpcx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pvfcvjfc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhnouznj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zqobheuv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nzexoika.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eqgbemco.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cvzjfyxg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2aibcghdx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2epyrwdxx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2etipqlmd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czrwfgje.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cefcsups.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tpvbgnks.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bpuzhscs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lvwvjizq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2wzuuwcjw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vegechbz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wcvoouyd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zfbgsfzs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sefozrsz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ahkxkfmk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avwryfgm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjlxymgk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2exijsbkh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zibnefyd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvubtljo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbpcjlhl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lylynxkk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htuwhbii.html


<!-- 参考信息 -->