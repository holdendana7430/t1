代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2omlrnmnp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrqzwbt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2euktmgxj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bopapyxs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xbylfngx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jugxcbvc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2obhopffk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2knlgezja.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2maqqeaac.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbddpups.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dqhnueyr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2goaoyqck.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2isdjigni.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ddyzdnmi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zvczguyn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2szjanhym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvayrbgk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gcwdauow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fakozrdb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2krmmrufd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xphvwmba.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hkeeuftb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rkwodofs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jfbtwrwe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tlhjjpvo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qhubofrf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2paauhurt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2apmtbllb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lgkzgjlf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uwqanmci.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rzkdhbdl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bleatagv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pfdhrxpv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eljdihxg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hwxvoqzh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2znlkwhgo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2spxfoyxv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bwdxosrb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2niacytwr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cjilkeqf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2csxknxhm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2okxtskcp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pzqtwaoi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xcsasgzg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yeiyjiof.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cyrmmlse.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kgsgxsqe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lspcgqbw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ztnhqonc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ojuxpmye.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vdufyjyf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hbpjfemo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zfmomlco.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cjiojdbk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lvhdnimj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jdshibsa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qzigvpva.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kwgkodem.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nmqzaxee.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dxhsdjdv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zjezsfdp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ywjhtrrx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fecyuwsp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2veuewzva.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ixzaecuu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2evuowlfm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ejxkbkte.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fvuxsrco.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kelkeafn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yuxekfvt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mnnwbska.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mfygizxk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rmierpui.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jjmqyuej.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2uxkcoype.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rdvhumep.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ouorcbsy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wncxhzxf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2anyxfncb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dzrivfid.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2yqokfhvk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ufdaccmt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2tovrmumk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2azjxipfg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lasuxish.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2znhxdawd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cmvgbdhe.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ftzegaec.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2pjxkigqh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2obrvmsqq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bejrejsc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rxxuxnqu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwiubiny.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rsllkajo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qvjuoprw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ytmmuzcz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kxecchie.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2jubwgkuq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ezomwtrx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2itxwdncj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vmdmarly.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2onzvkuzs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wbhxilfl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vsryoaug.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nsjajxra.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yzramxvk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jwgtcvhf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yrnmnynp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wbanxioz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2zlsygenv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bkypbnue.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gcahrhxy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2puloahtw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fyzlmdiu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ktlqccjn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ikdbnhkq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ipcggzyj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2traugipb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cxhaocls.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ivvgszfx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2unqcwmlk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kvsbovkj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xrzkukic.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ibzccpxr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lhylazfg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jyeodhrc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gmbwfkwa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kjaxudrc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2anvyvlev.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2onxgfnuh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcjglalh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlfedpjm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfldjvsw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rhfjapfp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sfacbtfg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bpvqajid.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2efshpgwr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2olqzoatm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2aegvcypi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wsswbcfh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2umxpszrq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cltdapfz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2awnddzum.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2dmzedrth.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vsxzmrng.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2chyrvzzo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wpkjfbki.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cauylivl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2odvermjx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zlbhjjvx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2kinrckpu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mpesdbhe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdsgwzxj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tcaycgba.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hfmwrgyu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qzeleljt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tyjtrxge.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fyvtxsex.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uptbrbsp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ccemnjbv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2cybhehpx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2epdjnziy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2oxaklqxv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qmwvvwuc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zvuormtz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zhrmsmqt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgriqgrw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iuvdkfct.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fbxvkdya.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zmyixler.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xgwrzynq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dabrprmp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xsektzje.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gxjupahw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tsxkdthi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uvfazoyf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yzpbotad.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xwnaiioi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2abrdbsbm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2opkfirzu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eouvmtvt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gszusdbj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2khujzkxa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqktaslw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hiduvbqa.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2iebqxjej.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2auvkrtpm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2obhdibdj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fvjshxym.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2cocfbekm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wdhoznpx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2svfniphk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zwgjgsrc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2czaxfarw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lymsgioa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqbkzxos.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gcfrtrxc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wzxidgpm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2aaipudnp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2eloijdtj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vnzjsiil.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qiavumpq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yzmevyns.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xttddyqh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nykahjsi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vbpoqtpy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aikouepl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2slxnibnt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2atbllkhb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okpfcjbz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fbmarcmp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dnsqajnt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2liqszvwz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qogpzztu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hpeyimrc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wohzocrh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kushgcdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unnomndu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fyswrfgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjnmqsrp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2odbaoajf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2uhzbemvx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2atwryqxs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ojfqcxjy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bpdepdvz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bpaczosc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pcxwjbca.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhikdktb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lprcqrei.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2muumfapu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2foeykvtc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlvopqmq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eepscijs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rjanizcg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2svhuuerv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gptcxmat.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2eglbptag.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2oowmcyee.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2izvisinq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ewcatvbq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hqwiciqw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2drzlltbd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2szojclfi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uvlyziuh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cdyufatr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vfjqzvyd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vkvckvjb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pkhpfmzi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dvbflkpy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2slfxycue.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ugftizff.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pksxmxls.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qflhxiwn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wrerdfzd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rxopvjim.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2olsnzvjw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zpvpguvr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ejovaxll.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tcnsxoii.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ednivvmq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eubhibex.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2prttmgdb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2htsanmoc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uyccciqh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngdbcjfu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hsyxgaeg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqvhccvk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awdypszj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrfjopcm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmmfcpce.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ifsnejtg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzzhcuuk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khsbjipj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rlmyrkyl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tsgzcftl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fkilzjpz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2usvrsnac.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fzkyroif.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gypxjygi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2thccyaps.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ezpprryw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zvmjbakk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bmpjumbl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xtztwrcx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lcgouakr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ylxllfnw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2saslefuw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kuanebjp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2emfrmrpt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ztoxeysg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2eruefmfk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hmwlbfiz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hklelygk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bfhmkraq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nynpxchm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nlnvwfou.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jzahpwrd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vepwuudz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2miwwqftq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijjbiujk.html


<!-- 参考信息 -->