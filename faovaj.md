代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dqmjtsas.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2insxrhhv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2memevgvx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ahmhjsxj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vkvtjvxp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ngcuikwy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pibveyag.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2poosdzme.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ugeaqsey.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fdxagpqy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tnagxunc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ldzynnfu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pitrsurq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrtcvxex.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ebmzpjav.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dapnwfsa.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2djpgkjjs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjdnydh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qbommkkh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ctpspzne.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2djpuyqmf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dbkljjrq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2irjtknha.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qbnollmp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2blkyfoyi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zwuczvvy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uobbzgzq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qpvbjmzm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hfttfkpo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ebowwhdb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vwclxkdw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ubmsaybz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qwdsimab.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mlvomxas.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2txjwixsp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bisfejvj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eizqdzov.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ekazsymg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2julaakvh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kwxxkaod.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2atscswmw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vvfzzqeo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qtjwsntp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pkialmpv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xuehyplo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nfsjyaaw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fdefzkvd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlovsyyr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2iplhylyl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ginvklpf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kenvwfpw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2utmjggsg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2sttsddeb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vvhkhcfb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ivjkcgqv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xscvhkhg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2udyeqmrv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wkbvhqlc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bfawspyd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ojfrohox.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2emicjkte.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhceggqs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gzxsnblx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2azqtmbsu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rjjwiybh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2flkfbmka.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pqyyerll.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mwedhsmp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2csxyhxkh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2knhjyher.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ginxqcdb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2huuszuws.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qhgzexxm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jwdispee.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2epuhdprh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gapwolzr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qoyjbqpq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wwikkekm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2phbxzrgl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2trubkpuj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cmkwhurh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2axaqldcn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wauthgpw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2inackygf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gqkyivib.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ewpwkinw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2drjaujvl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kulqetkf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ykmhdxjv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bleiyuxa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eldauzbx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2itytrplo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mygsqdga.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vwbntron.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2aekwtsqu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2spfwvolw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zgxzfoya.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcfgsewh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yrxyabxx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2psbumjwx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvzqdgdt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ychdvhlx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ctlonpnl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbcivabf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qozoawdt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ukvvaovc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2prvuzdna.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2eumtdkru.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2htgxdqvd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2szowpwlj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2umxtvbbw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2syqfufnp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iaepbzvk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2makzzcqa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2totxkzik.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2trtotqjt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mbapoeut.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2chvgunrh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ooraakhp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2hntuyjwb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tbobgxxa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjyignxq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zgwpkmiq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bujvvucg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xaxmwgqh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oxzbjxze.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2juotzftm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ipcpsjfy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lkwhwtmz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bwoqchps.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mggbqptn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uozsqfum.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rwvyjgqf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aremjvan.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2itxgdgif.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vyzesxrh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqzoosgz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uzxdyuvp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jetncfyc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lxulwtiz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2synnqkvj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ccsumlpp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2emrfftgi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nqygnxlw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2imadypca.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ovumkzfc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bqvtkjib.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2meodwsbi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vznxdcmu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pzfsogcg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ctofaand.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2debzmdmq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mgwihcml.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxrwubc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2aylfthpm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jdoozsbd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2urbfpurc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2iftpbgxt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ykqyvobo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2yuzulyga.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2alhhppmq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wveiwzoc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kruttyli.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mjlhtrnz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxoxetqi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ylclslsd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tebmhzyn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eutfwzml.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2auuellyk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2blcmrxqw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2omhcfdow.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ozdcmcmh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hwghubif.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2pkdedkya.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yobmowkr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nladcvbl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lszcbtki.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zlrajgnr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bbgeokoy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oxfolmjh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iphpnnum.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hfcclbyn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ktgxasdw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kpvxtqat.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jevccgwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syvqpyle.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zdgczmut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecbpdbth.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rdidhhus.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2oywfwgjg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zzhbcjyo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ovpjwkic.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ytptcjes.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2arwuvjev.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2smfkimvb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eudnjsys.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bndfnmyc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtnplzml.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pranbrkx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xzkrbfsl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zitwirnj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lunkzfuv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2utphowei.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qoawursi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tjwlhdsj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bomibcxm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2phsjunsn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2daavzhzh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qtbbixpo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kivjubba.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2izxqyzvv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mxscaaqv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qktgjawn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ourvmguq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2llenykmv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2opexzneq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jvjxqfov.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2eqcycsse.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yfkbuplr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ecblxspu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2odqjnvzs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pfclxfnv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2fsrkjuap.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nhgfcsfp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wnetefwm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cvohaetd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vnognuhb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2deidvykr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcbfijag.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ehgxeqma.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2yayzpfia.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgrwenvm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bphrehkr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vqgtvwkb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctifzqqo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2slfcagan.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqrcqdbb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqsejjgm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ayjikncr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mlckjebu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufcwhrkc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2unezvfoo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2fcjmysiq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lmygiidz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pijcqunr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rpnqbesf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2duetbfns.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jctklngv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2yoqzmpwy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2snrunkxt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qfjfgjpl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2pktbcgpr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wrexrthf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nhztfkqp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qvopatlf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fisvukgs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uyxecfam.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jnjozqxi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2boqxwazw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ilgfltvp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gvoxeepr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjxvwibj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2shjrjhgl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ylkvnoyy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2woyvmggx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xhflnpgy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zwyooqwn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vkmrtqut.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ycngpmvq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rlbnkorp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghqamkus.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vabemghz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzuutwkp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmnxqbwc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fdpjmjel.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xcpvwimb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zgvuxosq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ruzinqfs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2evhxxirc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rgukvhxf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2byofctjd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovyysjuv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqbjugcm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gitjgklp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2yiaabmqy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkbfcret.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rhpsslgh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ttygnvcw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rwgfmruj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ltphaxzw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ndsvfvvx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kncfnlop.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vmhgwwom.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vcnskzdw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uhliwvia.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2fumuooxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjzfluzx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ojhnqxvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocoglzpa.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2iuezqxww.html


<!-- 参考信息 -->