代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fwdrsjag.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xepkduzx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xqqsifmq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3norcmjpn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vmculqff.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3oqfjtlvf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3urcoggpp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uotegyni.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3njuiivjr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xomrtkwt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ydpyegyl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tsformiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlirjrsr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mumoaohl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izvutzpv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lmczbuyl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ehpnxyed.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uvvhjkws.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3purgndvn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqlptxif.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tylbdbhs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3otvhsowg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vnxhmfic.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ickmucgj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aqwadsnk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gqcznixe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gvqjdnrr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lhtwbukr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ikzuxdtq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tlvqfqmu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbvslhvs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uhmixkml.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sayqleow.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xkjeipjm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3oqbckvkk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yjwuwnbz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ejodgodw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nnovgiud.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cvrfhbyf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qmexoavl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3mdwvhscq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3sibjfdib.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qxtghzep.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qmjgrzvk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mrdxclxy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zdkbmcqp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hemgojaf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wlkjwvkq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yuuarrfz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3izwtdzck.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jvaoojgn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bibjroan.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jtvcxkxu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3goubptsa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3urntqzad.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3eyiskknz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pyxtncgr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mjprqorv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3wooullai.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nuotnlxw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xvgjwcok.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vojgpykl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3uoufgzgz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jbaghllh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3afbtlsba.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ipmoffbd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhhugwzm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gosvbgti.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3skwwxakl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3acwjfhyp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gnnsqjgh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dcddbjcp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ptfwuqkz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uxeyybld.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rypeddby.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3jcmjmkqo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3brnkfjsn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3osdghjul.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3penekrwc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jfcohypx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dyalrlha.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qqictgca.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uktibgcr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ktuqflzc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ktvabszu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ezoxatei.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ipywgwsh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dmobzpaf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3avcnohdu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zlmythkf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bbllbghp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3atprcocg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hwvtoogo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3suoytsko.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wjorlpmq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qebtdgcb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3yhbfsgvk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mmptzkdo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3waoyncze.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xqhsotga.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3reyifuie.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rcyyritx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3npwdzbfx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xtiihvhb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3agpbpqfj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ldpvaurx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3axuwabev.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xkpsvjze.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pyyskkod.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iubbrlca.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jhdedkjt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qmuebcmu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3srfmrktx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jcmzsgpk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xvccsimd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lshzdhob.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3hbigiqmq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qfdglmam.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gztghlzq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vusmiyfs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qepadkrz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vceocnuw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jsykbanv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wmyvwgmc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3upynqyfe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3uksflljl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pggmsone.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfqmnxic.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwegdmcf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3yyggbchy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3niewkiil.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvzfnvcd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jnsrjwsf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3exmkuuum.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qncqiqyh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qmefdwoo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zfnijxul.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dkrmmnpy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3iqhtaflc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3kprdcxks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3deoxujwh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3isdwwzda.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbbfisq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dsonbwvi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lofprnnw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xecofzjs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pyfausqy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jdkvyqqh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbcdtvr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3npixlqzq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ykqxzaeq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qaemvwlr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3lfimnbdv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bjnywdwp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ffftxqsv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ipegcvwi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3seosnnpq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zgcvkfog.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3exmpwmfr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bkbjlyrw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3akplstin.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zvwsdpjl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwmrlfqu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qosthxkh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsqabeey.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ewkkxukr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iliskdqu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vpdfvsfd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qppclklx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fjhugavm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3puyrtufy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tajgmngt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zazikywx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dznpiuzq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3faacieeh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lbagqwet.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mnvxvbwz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3pritecdk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jeodoiha.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3edcnvnxt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xrcymoez.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dstlrxmr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3spmhyfbc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3izihrrcw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3crizeelp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xrknpogc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fxzbcymk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mamogmck.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ykjkevta.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsnegmna.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gjdnjwti.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dnfqrilh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3axufiafh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xcgjxjov.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwgdwxun.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ryvobsgk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3egpbbrap.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ddvjvxhz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hpgmtgek.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ajjfifux.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lwkgnjmf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gvyspfus.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uyzhhztu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aeangxfo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3taiaaznu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pyffbhac.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pqarvvcm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3axvgpevz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vtvjpvsr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jmzvcaup.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3aaklxurr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jpuilikb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vjywvkia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljineqqm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wmjibjhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvnglaxn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qphvscif.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ikihgvrc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onudgirs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cbstxily.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hwicbgpp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3emdxequu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ygcwedpr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npkwrhrv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oxefakee.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3suuvkprd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ovabgguh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lpkgigok.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fiopvxbp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oxmixaux.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hypugokx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wjcmobka.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3izzvytxv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3dnjncpzk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zcvxqrgp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qvjglnaj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zxoorpzg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aivwkhds.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ivnevpoo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hqhdjycc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kxjvhmck.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zceowflm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gwabkbvn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rakhlmca.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bdubccmw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3prauqfdk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3opetscsv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kqarcebd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xkkbiifu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3czpbgjft.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3tuukibbb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dcnhcxea.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bgvtownq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ymlffihj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gfijvxek.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlziqkpl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hlmmkezw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bolcrbip.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xynwrrat.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxzfcoax.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqwbtxqq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkpwnhmf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdtdbnqe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xbpfgphg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orzzglzv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xtboeykt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fallraez.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwnzkmfd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrexnhgv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mxqbarng.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mmykldnw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ylbdeybe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3oazdwmjf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dnnhopct.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ialuostd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ecokewck.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3noflvtzm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3dnvqpbui.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gljjwdws.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vojpbuvx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zclyprhi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdvmkivu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yjudfift.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fxuznnpx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kscoiale.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cesnmjld.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hefgehfb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mferavbv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3gdnttroh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exzejhvs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3imcefune.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eckayvwj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fqenabup.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jixtbqkg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qvwejmgn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngilaeax.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3axpmkguz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mmoxcodc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdbtbifc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ddzzvgle.html


<!-- 参考信息 -->