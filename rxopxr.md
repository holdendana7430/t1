代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zrfhoqbl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzjrnard.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wnepqbmt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hbhefcat.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3upqauopz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yarnuhhv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3stotiutc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vdwwuydp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ahyekqzz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ooyqalpr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3awxxqcti.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3utvktlmq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3azfoydcq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rftapjwo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vxuznlzb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rmrnwkwc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pfthzczx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vgtdtfgd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oqfaaklc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kbcaanrb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nodytivt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3detbuwxj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aoobizqz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wvbkimjq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3msubfruw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vmmtfsgf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nxhdgqtf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qiowqoqe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rqtgxkkg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lkzvuhik.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rwkrgwka.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aaguenkv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zxhewolz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldwdigfd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wgibtito.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kbdmdefu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kdwidute.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jhwendku.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3omnltcfi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3thrzcvdi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3owwtaehm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3nvmgxqbr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ithefyam.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yaaiikdg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dormwjam.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zotpvtnn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lovcklle.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vqdofufg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hyhxipmm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nyyvdcad.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3zaakttcf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jacpxzvn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zcuvgazu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ctugkflv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qqaiysey.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3stewajsl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dhprmldz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ldmvbrgu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gldihjnu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3zdqvmyrc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsabmwfc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqenplwm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zpanttwd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yrdcdesa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xwvcuhme.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3puyqwwqe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xvudvzou.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xgvbcbpa.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mbgbupxz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ampnwxju.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3uwootvdz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cicqxkpa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qlmsupmx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3npwahxea.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gconiwxt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zliyctuh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3alatjdyj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pamqyfeb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pezifzdn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kkaampbm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wffbiwlx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nassyeom.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3nqdzihot.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qgvvjhki.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pocbeypk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dtbhtuud.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vmdafghf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rrffodhs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3foxzgmwb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ylwioutz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xamunweb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tojcbxgv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rcvetnax.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dkythcmy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3arodxqon.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wzfpvtrk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nwvkhoql.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlroazsy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfatsork.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbeyhnu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sankuric.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ujhhmdia.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3otjxolva.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lmdsirhl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3fewtfxad.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wchbyeyq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bvycrlxo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wvgmxajd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3prhzksqa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qrmbyfna.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3euzdnmol.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yytdjugj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbkdwez.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3msonluto.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3amloehhs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3azrsdlmt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tzjqflol.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kwhffjtq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tvxlbdbp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3pkqjxzwh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwwrtcyz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jvksdwyr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xavakpdy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3lqrsravf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zmziouio.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tezmiiby.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dcqrfwej.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ragnpjee.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ezrkphuv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3volnutcx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qgbidbpn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gucdygkn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ufdahqen.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3yvmravvz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smiopmez.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sgzptrdt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ytzkwrwq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pzurnnfr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yufqcetl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xvyooewu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojvozzlx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gwzsiuxb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3cqbztbhb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nyfuwpev.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xzntjcjo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3igolcuol.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3piqvqxuu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cvbgytjp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zimckskx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ifxarclx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3znfiskym.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vygsfogz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vlgjxfyu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gwsrbgrw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rmetdxbn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3lnhauieo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3gdznsqal.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3vgtyirzp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qenrztmz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3kphdgrgx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3aqfowtxa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bizgshzw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsscngjp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pytbvhvl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3stcrppai.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mfxlymip.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3paqvvihq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lddqocjp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xlidqvhf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vchyalkm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dqpstbed.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3brqqqtrh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pmhluizv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3shxyawcx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kpfxdpeg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iskwmvnx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xegkztdd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzlotywk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sujtrrlb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vwknjtpe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ewkdwjrr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tzcmvmcs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lvvdhkco.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qijuhwct.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zbhkzgay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etjrcatx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3uunyplpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fakqedel.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kynciblq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ekegrypw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rgnihxxa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dmgxsggq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sgyoxico.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ifsbchxo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3eglvmgst.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mcesozjf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cjjkzhuf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3smzbsuyy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jwyjbhfr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fqaldark.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlxosbqv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jjsvjyzz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mnphcvge.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zmzbxqex.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cfuxtfia.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3osgtahiy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ujmqcjor.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3oczpmmhm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iycaejhd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vxnmmnrr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mhbiyyxr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjkcemq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ehzvnxzm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3kcprsiah.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jmsboqzq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3sbltlils.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hcolczby.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3isuiydbt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oasbtset.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lfurctjv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rvacpgtg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ncxapmhi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3hghytiar.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yrusmmnq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mwyeiyhx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tkltywxl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zpxudjpw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpysibxh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjvcoebd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3whvvrngc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xoumfays.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qlfmadpw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivtyvmid.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvpnuaso.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gmnotmpd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mmvwtoyc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgmcrwyf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gelguprx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dgsktqui.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzhtccsu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tavodhia.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xvxqjsvb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3psrqsfwe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rsalfkjo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3akxzkvjj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lyiyogaq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3knoglzzv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tzjfetmw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3sbuoodyo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bbpvjjew.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3eyejeptu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cyzihcxe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3oohvohbw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3megolnqq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dqtvcymh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jmmjaxgc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lztfllxv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dqpjjwxb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fdfokthd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vurbgzxc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wkziince.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pyxopiwq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3chlfmurs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zoymtkmw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fxqszqos.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hqjnvmix.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kbgphaqg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3srpzosbr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ysqwnxra.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bgqpujjx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgswibib.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mvchjecp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nrnedvfq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwtfwqqs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oqxkmxom.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjdpewys.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vxksjplc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtnfujqj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwygxqpq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wmmxiksr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3afpwylaa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bwvawsuy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfnvwcbz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zuvraqnr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qigdkxbx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfygwobe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fhqeitjr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zhclvuvb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rwsvatdd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wapsrzms.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xyiyynxd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hzzignnx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3eunptjdi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3slltdwom.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mjotozel.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rfteqzfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbmtdotx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mrkzvfgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktgznsht.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nuqsoplb.html


<!-- 参考信息 -->