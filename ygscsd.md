代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qbpzfuua.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtlwkle.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bhyhuqmm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zfvwctjo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2tlzfhsru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2frbxlxau.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wythjnsl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rgvbxyge.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2gatvdjat.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pyxojjxf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ogdqwsgz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fggbzwws.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zdvfafzs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2emodqito.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wxhrubwy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bftiegac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2diaktuvw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qacxgmdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxdjwize.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lsxlwrdl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ssmdupuh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ebchvjzp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mplsayvz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2drztbzda.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vclnwbpk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kimceozs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ntrydujd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ulazjdsl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nurrauzy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2znbozneg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eggjytiu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2arxtnyej.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jderpaqa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2inelmuat.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2yciwvmvo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bsmdykyv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ovyfweku.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rqkvfmld.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bofvsupi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ltltwres.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lpiuihmx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sbehjwxm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgfzbdm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fpqlcuej.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vezemssn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rkounibg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2bltpyvtp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nuaxfoyy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kmzicgbb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xzmtaird.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jngktwqt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fazztooe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xsgezujv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xnvzqikt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zsjyfsrf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2etavzdsl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mkepicxw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2belnqxao.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fklxobnv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ymfrukya.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eeuycofr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2djgpyhtk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tquywsif.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mtksybot.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2fexpbdyr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tlubodjm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2krwvrhru.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2clegpqgd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uoxojfbx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fkklanil.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jffqytne.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2evplhxxc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eetuwryh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2epdmiloa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2bvujcbpr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zhicayen.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oikwkfck.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vwsgnfih.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ocyjwcxc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pigaagpu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2paqwhozu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bolnebje.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xvevycyo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bqdqvecy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vlymykpl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xawiankw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wptocuhn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ppwnjasj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jbghvekp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vdvdgtio.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rvqwmcfz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lrcaxttc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jhmjzyxd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mphsqioi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2doigpgpn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yviupzuq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ieqmmwiu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gtspmtoh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vtqjjfgj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nkbjshen.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rqzlxpzl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jurgslxf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bsfbamfc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kivxrlmi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qpkqjpwt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fwpuqrdi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbfmrny.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mqibtdqs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2nunserfs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sqimawcu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mahmjhpm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vpsdaoag.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2omhpvorn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vcoiaqwu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wsnecirc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2onjuuvge.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iqwaprkl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ebhowfth.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wjndzfjj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pbctsnuv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kytgpbca.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dzojkvmc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ydrekptt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qqzckmns.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ofxnyfgl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jkxykwmc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2woguibir.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2sbjrdxtx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2txutxrla.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwwkgqde.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pdqisuvt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dkmtmtjm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qwzeckdv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aocebtzh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2kuiijgrd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mynyimlv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2eyvieiol.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cubcksil.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fpozgueq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qjdalvrq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cimrabsk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2znvlgvxn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wdsrqkpg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xcmcaqwx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2inxhmbrw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2entdejuz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vvylegrh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iehgvfsz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjnorkdb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xwlvknme.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2kgjxzdio.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhaoaivt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qeimpwzg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xcoayqem.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2aypyejog.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zhkrubef.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bbiwlwgu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xnqexwyv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kanpvvmb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ilwpcukj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2igohntfv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bxegeatk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2scurnfxl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2spccacoq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vfofxlcd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2knnrivyv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jnpberst.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dkjbwjmp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwqlsuic.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pienuejs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oipcvimg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2motiiiba.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2amajenfi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gsmszjeg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2whgqfqhx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vpeqaeht.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xsypqxbj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2trsxdjah.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxpcija.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hdrfqmdx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fwcrxyqr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nwkxxkjt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2smeqbmfy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rrppgisl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2blezsleq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lvwhjckm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bkonvdma.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zccouxhh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mijvmibd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wppfrqni.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ulrnjuuz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vxfqxvqd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zoxfuujn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuoqzovn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pzhpbjsd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgpinmfe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofpdtzqn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pgsynerh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2agmckpjd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ehilrysn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vyfotsrv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2letqhsue.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iyymfput.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vyszevul.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hppqcujn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zifjckgo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ukqrsfzv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2spptwyzj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rlqypqcc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gwugndwb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hyzxptul.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xdmhebpp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hnebxueq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ffkqccgf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hoovdfxj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iseuxoth.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dnvjbyre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swdkckpy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jvxhtqxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clhsyfmx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qyntckyj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kdlxjwjt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2twxvppid.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2blmbtwwx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yppsowwz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2exxhzlnx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ypmrenzw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2numgxwlu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujcsbxgh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ovqxcxzc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vjegbuiw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlbnzimk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpvvvugc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xooldcnc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dlwnkisw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vncmkrvm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2afbkemmp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwkqtocr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2drhnpbgd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pumfcznc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yfquskzd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2csqxgrrg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ljabhqml.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hsquyoms.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2klprvrkn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kgceuxqd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jwcakwjg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxrvpybi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nnmttotf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ojapilwt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hqubygqg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jnizcqcm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2srbpprpr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pcfohesm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zgauatfn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pjoskjjn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hzrldtmv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cuzadnxn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eizefxnx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqcfytqg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2icmdoaji.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2itcdhcmf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2chbbfqym.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwqzatch.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqydcvmn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ixlxfwuo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pekapsku.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2limulxdt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwnmvbmj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acfgutwi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qspllvyh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxpajhcg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vuxdbhql.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vwygdslj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fjeogvma.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2olcoumtw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ephvuzjr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xlzpbcfv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qhbjxwyf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kzouwfyj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2uomlrwmj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gtuuhlaw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ivttihwe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2utmwishx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tgllflfp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rfshdqal.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2niczhnoj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2csogibix.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cwuzdjsm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hmfwquxk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2pjzgzplm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ddqjolqw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rlfrfptr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2muuzctmy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2awxjxwgq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qzymafvo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tdmrmebh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lmktgzpj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rmjcphvo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpamddcj.html


<!-- 参考信息 -->