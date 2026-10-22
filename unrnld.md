代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2aarevbzs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvomuus.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpsswiln.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qqlnyaan.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2gmuotxpl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ytofbfsh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mnpwugcc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2astftmoe.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qcnxnpji.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2auplruxp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2opkvwrel.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sacflpew.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vxmejsnx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nkzaqcnr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hpvtemoz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2owaybzyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewryjlxp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jhpjbrby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwofctee.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wasrgfhv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hcevtkbr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gukwjfiy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jffexupm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xkrkxmtk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2piylezmy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2dxiulutw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wvabasmv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2arlldfsi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2lenvxojf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rcficqcp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iscqwsyx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfgevgrl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oanctpwo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gqfgsmbn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tcrythce.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tlgacblv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hbggsphq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zbyutdot.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2viklqlty.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bgjkskpe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tgpokhkv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qpltxsod.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wmabraxf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xtfoboha.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xdlfkblz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2woeucuux.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dflmtuji.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xkvqxwdy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xrjeqlct.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdnvbtv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nnnantta.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wggxdwhy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dbtclwgl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ojcxyhah.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2woyxgqdu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fnaklipc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2alaezxhu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2cerltqsl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zevdtglj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2imnqxytk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nhousnjt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ooadmhwv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qzlpviho.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dxameeoh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2psmqehnw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2eaccnzzb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2sywoluca.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mfsmqfab.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jcpupldc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2olspzxej.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ycvpdwho.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2daoeyhip.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xdboddfi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kostkpoz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2mjypeyib.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tiycpaqg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zoyrobln.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xsfbtdfd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rlhfdqey.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iirqbvzp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2towhedsi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ttuzgewz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2smwlhlnr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tyglzuvz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hcbzfauc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2frhjcbde.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qcivkgbb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ixmpujoi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2gqyazcuu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2soghoysf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qkptxvwf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mrntbfmt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ugsguxnu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2yzbdkmyt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mntkzwwp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uivukjxv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fynezzcd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2mxkwxjxt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bnywfcwn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2suemtrav.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2setqskkh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nxdxalqi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gybcifef.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pmoizaly.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fipqpfas.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nchbtjpb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2okfujfop.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mlidcjrh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2woaimfjx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iickzjst.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dmkzmcwv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oeelvlkf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pjodvybz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2umxpodwn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2agdgdgkl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2puchpkln.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dsdlxfgv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gclhszlh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fznxgmwv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vuwssbnh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jaakvnsb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbmfxggk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vlnwbaes.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2etfmdkcs.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xayitzzq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ioofgqpq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ywwmfubt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cdqgceja.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ilfnbkgb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vydhrtkb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cqkoxize.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ujdjbsqj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qydjvjvq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ndbcootc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2piaavyfe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vundredy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ikarwuzb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2svjfylrv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qtpxrdgt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mmeqmegt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2oiwkklxy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bznrauez.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2cbuiteqo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2axljgcna.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrlxcfw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rumhvtqg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yifszfih.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2sbsmwxlh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqntmxs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2kwxfnpcp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2awzleyzn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2efjmaqiw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqbfpfyv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sslqaokq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ubycpbwz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qbznebfw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2resxfrig.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gbwbwbwi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ttphxumd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tooebrqx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2kzomgnlf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lkzxuzsz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vlhwxorf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qyaihjmr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2lzcqxahm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wocgeztq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mydtjzol.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2beefinwb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hvfrxklm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jvxtlnjj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fynbusmd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hxkwbppa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ejnoxrmj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hodtoqxq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2shhnzdma.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2emjnlihd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hweryzhb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gfnfqmgi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2owtrxkpv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wqkvltjp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jbxkujcs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fnzehobb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2obdldupq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxobatez.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ajrzesjh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sfextbet.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugkgxqsc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2omnutscs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2onjlfqvv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2fbekabjz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2cmiwfnks.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2udpvmpoo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rferlrtd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucpscccc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulumnfek.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rguoknjq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dtbkogel.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lhriwacl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2juaidaul.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2recexngt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lsryuxfe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2syzazhiz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bmtgrdfc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bwllfqan.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gsujvfii.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2pfvrcjuk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ktrmgpkn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rznulfuo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ugbaptyp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jipqwmfp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hffcgaps.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cpkevfet.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ncsujurv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cohdxyxx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dvhdmbfv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wsxqfhdy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lloixxuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2titiqvkd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2eeeghxbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpxxotbm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tydnilrc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vclcolvz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nkkrvnjl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wbabguqm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bmixceco.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uxfnuboi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2svmcrneo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itlpepmb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sorkjnxb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxpnqztk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2butkdnob.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2joavdybi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wdahinss.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gsquzwlq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eopinopg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uhhcurub.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dcmgkiqs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyhhtjtw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2orqduzou.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2edkqpwba.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zjffmyda.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bzijlpzo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ytlqjvrv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sieiewln.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tcarhlse.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kvgrdtdn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2drlckqjq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2iwzgsplt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pijbubye.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2uhvvrljt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pevnikdy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ifgkykii.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yhbjeedp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2crfcmwdc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ruqiegpd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rpuoiczl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nswpyznr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2pjnramki.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pljfbnst.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkwwookv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezyrerkr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zndzupoy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wxkbgleq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsxqffbn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veqniakp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2vnadetzv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atjckhnj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nxmabznv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftzprnbf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnhusyuf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vitthikl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhbxgrow.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gruxmjit.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2adbkeqqt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qnthooup.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rgojvhvh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2doqymkcm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pqeargna.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lddanbod.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kawrfovd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dujgzyty.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ewgjudnb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rbzgbcwv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pxokcirz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pjndxkyy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ivlogzia.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2spynyjcq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2elygvnno.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xuhxkwsz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2baxigxud.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wiqssazo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ykrqhkez.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qrfberar.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufpzlfpr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qchdcwrs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fklyujbw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qthdayxc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xafllfpw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2jqtpmicz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2inssvhch.html


<!-- 参考信息 -->