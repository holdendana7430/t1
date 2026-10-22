代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2profqvdv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zvffkunl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrnfdbai.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ketouctw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2widyqgmh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oudnnqoy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ztvrkltp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gchynnxb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tuwgkycs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wzlqezjx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lmzrcmyw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dpghxklk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcbramxj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qolxszgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2verkdlaw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pzmvdyqy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qcpkdbxi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2aobjsvwj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nlynywde.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2quiietrh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2iqqvvoev.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hmgkgzjk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gggjhaxi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2irwovpzx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fmpccmjq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2byeknldm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cprbxuzq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ifbakqte.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2okextklx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fimldftx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2imbjwlqa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fibtveiw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rsxhifjz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2upsdcbgz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2taszrfxf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cpvgcdes.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bccnwkdm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2esylnlaq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gamfwtms.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cnwigrcj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hotxblbx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2naahehlf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2cizctksv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2axmtrfmp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ocsmrbbu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2oqypinoh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2onyqprcc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mhibxkaz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gxexemqt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wogrbzqe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qdomsocm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2nelfexmw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2dwxhjhhf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2rkginopb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cqcewoko.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wikuqumi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jprclflc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nryltdzj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wrsfwrve.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kzdbzumo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2tzsfqyvy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpvtprgh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kcemffop.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uckicfus.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2glkhyrzx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yhoooahm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwbgctpf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gaoqiydf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eoizbklm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ugdisiof.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2njtzpkys.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2spqfxqcb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zaxvsldn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2sptafsal.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vdrwuvyq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwndzjhb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2heapwluw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fkubkxrl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zvyebyzv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2eczegxvt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gicdlhcr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cjaooseg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zikwpfem.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wfwdmrdt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2nfgrduig.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ndaisxuz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bpwuvunz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wlgsjdsu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cgryaznu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qmnqhpnh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2feazizjd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sgcbobpw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kvkvzpoy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pmyunoty.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2uldipnuj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rhbgwxch.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fxhqgapy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nqcsriao.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jpttqapv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cknkkzfw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cbggvwuk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iwxwvsio.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwvrmuj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2imclfzkw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fbmwkwih.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ugmosdcr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dyqubjeg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wjdogyyc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zluvkykt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onvalzip.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2muehkotu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gfeodcrv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2depbsgql.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gcxxfaqy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tvfzaaki.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gcufqwex.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vgsywuca.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rdbxyego.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nnbplujj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tncbdfkh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hcvfkzdv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rvtytcez.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2hvkbjgam.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2upwkrghz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rqlulkao.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyixwml.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2noxdwffy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zbzlpoww.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fvvpfqvg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vntydixa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ypkufkfa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjnawmew.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pekorktn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2avqcfxsz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isqnqiie.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ifbbowmp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfyrcgee.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2idozjiwh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2juaobkjr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xrbongai.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gsjuhxgb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2unwiwmnv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2sohsjsqr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pxtygogp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2thulyejn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vxlueixd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qldwmtkn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxnmgcmg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fxxblgaw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pwmlqncj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2saadzizj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yogjotyn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yqyicyod.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vxsuvcfm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iqwmwthr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2igjwzqwb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tkqgijto.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fheopqbn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vgvycelw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2iznmiaco.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fubufbzs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jxehxhtj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zinvjgpr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2koojmulc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtirkcce.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nljexkps.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pbjhxsel.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vkgaybxv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2anrurtvj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ybvqhrrk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wmlqpfnp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vajchoyt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xdhkevrj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fcievtku.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfdxyrao.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mpvlkizv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xjtlzfza.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2htahpcql.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qfmdcpad.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zyigmavh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ufhmbgnv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2umppzbya.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vywaxrkr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dolndjkf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hspgroft.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ujayccxc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jiwmysno.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gysjmwdh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fupgfozr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpkmdjbp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wotfuzdk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqnrigcd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhmlitvw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2etxvkvjn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzmnoiii.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cnfbingu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2aurwsasp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ymuhiomq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fmioinfm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vgusmrbx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qzuuxhph.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xauspwcg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vtvtyofo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ptqntqpq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2howjfckp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pnoanibz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zctzcybi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ehehhukd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wupsuwzl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2okcvorzs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mbjqtnmp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hnbvimqp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ofmpruql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkhiuygt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2akjgonex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdfojdzj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsmegyxv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bjxxnjgq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ckbnccci.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2imjdwgjq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mnctoxud.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dxqquoql.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2grmojump.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mxjyuqej.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gvhrbmmn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qatrnlop.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2nkcdwpam.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ckzgjfzf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zsjecvzk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kmrczqvm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2khrwpoqw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hiqextka.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dhfotjcm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mnnqaxwl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dycynjar.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jdzbcvfd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rgjyvgvd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tfoxingu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hbzxqbwh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2efmmcegd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cnrlolyv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qxengket.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pijhonrl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2jscgruwr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cginhppz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mmwajdja.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wljhzzxb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hiwibrpi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2uzoupwxi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wpyeunkv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2oqlggiwc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2iefozpcy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ggkfokff.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2obqcjdhb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fggebwkv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxzwblpx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fuezpvnj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fmcrbesc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ndadcrev.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqyvruvx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ykuwsemk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbbzjnlr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwmpabqw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zieapmtr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnztfwcd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjardwkp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uckawucq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqlaqsha.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcghomsy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dpptqoot.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mzjlyjpi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2awdclauc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2quhbxmyy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vxjxqqpv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mytchkyq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rurycdpy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pjxejfdb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2uxecxaic.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2eedamftw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jripwadf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gpzrutka.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2sspkykos.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2omibuahj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2szatrbdg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cueifjrp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2smlgndkr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ncabbwvz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gawwbkfa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ksxuipba.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jcwcrydl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ilsrkwdi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ejchammf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qphoejjc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2poyfibtc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ggfvqfyb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldcvpfei.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2glzrumiz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2uefvabib.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ktcyqjfe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dwniqxsq.html


<!-- 参考信息 -->