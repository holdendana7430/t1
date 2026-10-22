代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cfwnnbow.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ymumemgt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dreqhaqq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ppbvwadw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eozqtoox.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2worlgjmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpyhuwtr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pglmiaql.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qfnztqlg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rrcdsygw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2srnoopvg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uqjjvcvu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vkwpswcg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2eczarebk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2shtygtrb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lkmtyawg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uryyiwhj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wuqnavsr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cvllxgxl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmgrxmy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hcgerupy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydtmrqzq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2plbujncs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xfgpzfuq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2aktypiwf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hwmrschl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jnmsegcj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mpkheeza.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtqvvoe.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kczaevva.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lxitacri.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zuvlgwnb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mnnuzeiv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yundjafb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2plosgrqq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xrwthdlc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2etnnghxm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wfulikpw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hzbtapph.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ltqxyzvk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ohcshzux.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jsnxtuik.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xsgxbojg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2kkqqzhqm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qwipshnm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zegwblro.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gbctrnpr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2motuindf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2faryvdxj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vmbzlbnq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jxowmbbl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2urhsuuyv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mvlgtygi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyqbhuwy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qvjvwgvf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kknnbecp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ixlxpmoi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zewuekff.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xwemdpul.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jkphmpuc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dkxotqfj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mxroaijd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fklsfgrh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vkzozopg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hrbvpkct.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qgtwnijy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2stnjvqky.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fnbmvyxe.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kcvkfnmy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2awiuuqin.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xpeubwfx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kvqpkrus.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fmsbsezn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yttjgqlf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ecjnvhvn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dgqddaun.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2whddjbfn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2htdagkyj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ueafiskq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2irdnplhr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2baosthqa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jbpyzwtw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xsxcuqjd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sdjzmxdd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gmhvjnez.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2cdscajjh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xfslkajn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ipwhybyn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xwtftasb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wxwtddyw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ruqjcqgj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jwuhmtth.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nwhkaami.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zjgvyvpf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bworvuzi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mzmkijfz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mxjbnukr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2yphfnhxn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ttttidvz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nbfolpvd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bgtaqywf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ubxffydq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kvnfjlqj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2okgrpusb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ppbooiup.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jsvnxvsw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2uqyvxkhv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rwxdjols.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ledahnnz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jfewhyno.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2iqjxlbxn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pauaubpa.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2auslhoxy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2olgnexgp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xystjzbx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fvuvrqoa.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ichueiih.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2aomuusyv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gqrmsult.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrhmkbcs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qswqmohi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2erasisxs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pfrtfwcb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2teytmxjb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2otswgfiz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2igcucyyx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lheiruci.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tdyyupkp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2loobpcat.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2evzkcchc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kloqckbv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2oggmcalc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ghbdnddj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kthvqdsg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vwbjobxj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xofwdsmk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2fjqhgxiz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2enpgtdkt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zdcdszef.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sikrucwm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqhtrxgq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nuzpripz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hkadvtes.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2tejzliiw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nundgikl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2njdsvlrd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ijlufmgt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lseqqmor.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2saoemrfq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ghunxvxj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jsshhyur.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kmxygkup.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2osyeqxpk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wtnhpshe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmncfpul.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2txajmqtz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pawlqmho.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mufmqvwj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lfxexxnm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ejjteuhg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jnuusfxd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fyfjeqvf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rhyjpshl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xrvaljpr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qtqruool.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2umuqrxzb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2brqrkoes.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yghapjcc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xqbexlsg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dbaruioc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wsqklpgu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pdlysrtn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fmyhjzfc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ycyzshjg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ipjovjhv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2luvigxph.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qogujkqv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xgckvpcs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wajjkabr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kwmxjaid.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kyqbsaot.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2molgsxau.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2emguvjsz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dkhdlbxd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gxmadcyw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nclhuzrl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gnoswydo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ephdhsrl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zmziuozg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2awxqwnvd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iineakit.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kdhxlbfc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2okhdmqwp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jgonvntd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qpdclpkx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uepsnwmt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kohgoqas.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qibrxcyb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qenjoaoy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zhfjxsek.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2casgoqal.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2azxxsstb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rhqzmssn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fpgnyxmr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ahykzdvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzmivyhl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rmecjwxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvnfnskh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ndyvhxpy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2cptjvndm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dnjdeugz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wpqjbadr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xzrgvpqz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2teltomrk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2yiotyurj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2olyuqcni.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yqjhzxnc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fyjkmaig.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2avcbrqge.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrneifxr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sypqjpno.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iaxgvmwk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kidtxlbx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2saysxexr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hwnijbtx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngusbabt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jylowgut.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2irbntsyj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gfpuidsj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pljjjovr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kbpfpunb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rzzpibrq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yeeawhqq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pykchtwu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iphvzbbu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zpwhhzri.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yrozduwc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bmulbcoh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vjhplygx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2luovejxr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fkajyicy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qpsyfrfz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jtcoijkb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dyfgpzpf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mgthipmn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2aigaveav.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fpzsfers.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwxfkhyo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rfkcfdef.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2szzkwzvn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2adodufie.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kawbmubc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgxumzkz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2voilbljf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exnphgic.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awzecauw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfmusqjv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oulceakk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sliqqehv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdymxpst.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlpzvhdx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2svnmqhpy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sjtfwqog.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jegjfwfs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nmqkwcmy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hkzaedzr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zairztdd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gxgrnpjs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hehwgrdl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kagqzhnx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2lxrznafr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xyiosrpc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mwfwrivo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcklkrow.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ugqeyjza.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2icpqgvih.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2iviaudgw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tqxfsajg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gwopzgvz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mmgquyut.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2eojjmllp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqlferyu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jdoagani.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sywdkhov.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xlkhekss.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rhylviko.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kvekmyop.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2erorlcbf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2itjzwpzr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cwyzyhqa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eyjeyzfi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jgadmczd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqtyjcea.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcbrdkiu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wdzsagev.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtjlhdqe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bivyvted.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmgbpois.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rmfcricl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ergiidjb.html


<!-- 参考信息 -->