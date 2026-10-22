代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxlgaaib.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tkhokqjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igxgjrsc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2remgbujn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bojsczxx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qxmiufxd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xjgfzxai.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ygvteucm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2geoesjll.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bkmurcxo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xziomcly.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nvcbpwle.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvmgzhmr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fxvtyejf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mggczkst.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2epxkhiuo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dxihhweg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oielscay.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mlvoasdi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yldwvcdj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hwutoycf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lqlhycta.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lpchlrgx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2boqgeeva.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hevnawqo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qadcsads.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rppxbdsp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yrcuvzal.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2uhvddisf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kdhayddk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ophffjzw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2whflrdfq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2puxnqodo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jmbxujvt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uwpjlthv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tqrcwsth.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zpyyzgvj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nwmfclnm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ihrmwlkl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uyujzwup.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bojamxaz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vrllvsnm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2laisrwro.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2iaxlmoyb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2donqvjsu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zhajmadu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ecdkbacl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zmmpcmrg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pslvomgz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cocnughl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nwxdyzbp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tnevcdyc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mncxglwe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2avwubcjn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2btbqiupe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hxamucei.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kfmjyvph.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ktowmpez.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2scwblkwv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vjvpgafc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cwunuyxf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mecmtyzs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zlmfmwco.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2szkkhovv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pmxxxljn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2whqnuqei.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zavaticx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fllnxkgq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2awkprfyu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rqpotxkk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bcmkajva.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qsxokyyl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pgncdhbp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nzfddxie.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2inlwlyew.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2meyzhqbd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2eyuvqhfn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xwjclmca.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lwnpngxa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2enjngwpj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wbbzyicm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2srtubhrb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2stipcrqi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bydlmnwy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rhftvzwg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dfdsngzm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rfnctvos.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2egdociel.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hjanxrhx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fbevxbto.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2liytvism.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ysztxduk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ezlvkahe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vholenmx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2getqwndh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2llodqlvm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yqcqnxjo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yowrsbxp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ibkxjowc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hqloqwzk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tuczcrft.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mtkrxdmw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qfnfchxa.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xyxypmrd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wcbydlhm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cecytlly.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rwjqrhnt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2eiynogxl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pvgvvmoa.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mtlbkbkz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2aojlnpwj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wxholgez.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xvriajar.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2johiujse.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hksewfmp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2viycfjom.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2trjofnop.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ckspdrup.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yrqzgwdw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hcawgoaf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xxradovh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2uuktzdym.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xvsgszas.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2yzvdwafo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjapysrg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qiownhfw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uindzrit.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dxawvcsn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lztzrreh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2eauoqhjj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kwfshsdp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rxwyqvsj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yqeeyfvs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zxktiere.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cothlnbe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqtalaum.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2exngeclm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2yyipkxkb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xlfukqzw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qaoitzun.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qmmovsfi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xmnyhgck.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gcnvagvp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yqntmotn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lqricuis.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ynarezpo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yvmadnpj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yqjoyhvy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2iiqwwcmi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qhknvzuo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2luosxail.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ocjglmby.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qrrxfzde.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nlncrjdb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ybwrgroh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ddvsyemj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bbaatqcq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hnypzcku.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2lpovjxbp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rxrwnpac.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vezphrru.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xsuvpuks.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uwplaart.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2htljzjse.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2efjuucmu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jrbqvdbk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qegniily.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2osucowaj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sdnqpcbg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xipwkfps.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ilwjqzcn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2betrbsvk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mqgyhzat.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2grnlhfod.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ngmgoeyy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2volmyrbm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mitfmhlc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2pyjwqjgx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rbbgghxs.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkbobyks.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jnedxyrw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2upqttpld.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2uokdlaus.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ijfyowua.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dbbrdeja.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jusgpxhb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rzpqgukf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pbnosmwb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rxicbhzo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2owlcpcct.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2waxmldgr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pqiykeln.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hhcfkxte.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxezjhrr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ymijthiw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ifmeptaa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tvxsoboy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rnikqcbq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2seecnxso.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ltumfvqn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tphfjifo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bztqyfni.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fplldgcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxnpfyjx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2iaypajiv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2quurvgkf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2symymrod.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2klbiyopb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rvfvuryq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hqtmhfzw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ndgrfmdz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veffhrfu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gmykcmkh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjjpkham.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zfiivxrl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2blqeykyw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sszyjvlw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ogaravhk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ubzsdkxd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rkvbwwav.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jvfmachs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2opnjufye.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mcdgslli.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wenpwlew.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cvifffhs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sndkuicd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ivyibtmk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2trudtiks.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2twbfvnft.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tewgrktq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2svvmscec.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejcxktxd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nsfzpljt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kzpzoprk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nmiikkkp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2thefgfjy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dpagsqbi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sufqhaka.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2frjxblgq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dqsqsyaj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2chcblhca.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ekfckxtb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cvqfyaco.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxwbpscn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bsgluxbk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zecwgigc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2untntink.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tabimrtq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2serdcqca.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekypsgpk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oskjufma.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2whpxuvma.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tkrtbvqg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjsvswfn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2olwwikdw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vylnjopu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxorqiyx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uctpfuuz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2spmnrdhi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jflqzekj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2inpqgadw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kcmlmhkb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mdjgnrnu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kmmnhfpw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2yzevnktx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qichvxau.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2klnkonhn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2thlvlvxv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ployhvlw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zytbnhax.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xqvacdqh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dfvukoqp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2adntlzvd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qyuaanfx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pwhppsgi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mantkviy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2xvawozhm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjpamekv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2enlsxaqk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2eeoeogvt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2quuenirp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ihiulccl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xclffcrr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2szlfmshs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wtetaupg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bbtlvzvb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ioqezrhf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ozjzkbos.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tntqjyxn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpprhfeu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2twkvafii.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ceuoocxo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqkalosh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlqlsipe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtfvhobq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tewfbdks.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2sbndlnne.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbwamjar.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gitwrjxq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pzkrlemh.html


<!-- 参考信息 -->