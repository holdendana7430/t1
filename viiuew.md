代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ppzlufdm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2smlcsfgq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2tspaepbr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vkmgnrnl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tzqamovt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fitncsqu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vbakkrun.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvcrcufp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ipreptie.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2icewgdgx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xisabumw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2chiwvugc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2biuabdak.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2csoingje.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xjflxgmi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2neqcxjsh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2exlnrcvx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2krkqkwjr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uyazirhf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lnbugddg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziyhihih.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gqjpocgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxzmqvbo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mheutasd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ffabwmqa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2saxfdtsq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yowwrnsu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rszaqbfz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fwwrnmij.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nbzbezlx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vsgfdbcz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qfjczanq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2spmuijfj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2opcxqnee.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kylnuoco.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcmxrfs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2axexwfoh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gzouaoma.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ftmbzwio.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lkrnsjuv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zprhuvbx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hconzuiu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fjdhjitq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kjjizybt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hlqrxdcy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ixuvypft.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2brnoiklj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2knkptysy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rphcjcvh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bvnlzzlp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rrhuhqqx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vsrfxupx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2iopsawof.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rexynyiy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dffuutge.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2irblutup.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2bqezhcrh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jfvthbmp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wlpvuhcg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xrvijula.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lxdugivx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2irnflqlm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nyxnriar.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xtcjydmu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zrsityhh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gezixlfp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lmrvpcew.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vsdostpm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hxigjwuv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rmrnmfys.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yoaouviu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sgeegskh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kbpbfqbk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fwjhppuv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2emycqyyw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uyxpwtxp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bqektefo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yjqccemj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yffsudny.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2otzqngjg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ytnrnpiu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hjosqeje.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gyacnydy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rjnkygdj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tzpxtgrj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2unsdcxoe.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hsbuoupf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fiacjaat.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2actykcgx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uwysmawe.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kyhqbwps.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2chhtdjlf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ztnmzgfi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jhdudjzo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hqxvkekt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jvqubsno.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2znglousx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qgzghmwk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qjbhascr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cxjuqbph.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gsrxsxxg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hlylnxkw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2kdgimxlv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rmxbjwiq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xsgahtpa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jlfiwwin.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2myfysdor.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sfcbwcxz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lpvhrpda.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uycemptz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qlfyudxu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nbqsqwqi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2whoukodj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lsqugurw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fdiidzgr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwxunblt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ftnbrifz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lqnmmgtb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dbkvpzfb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2exuzjtzk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2drgxcgaq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2okoyhywu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fcvqjyrh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hckmnddl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zlozckik.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dyvvasmq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2etcneeno.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2uxhmiobz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dwnwzlos.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2axayftfh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zkbthuln.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yyiebdqg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wjsxfgbi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ghihpbpt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gkzbaexk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mdcjzdcc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ymrgvkpt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hfdkihai.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rkvygtmb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxzwybqy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2utsojhbt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mzjkwhlh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bppzscfw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tkijrxqr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2afwuebnh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mvlgiavt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pdttxqfm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2psluaaqt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xsitccdh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ocmbrnnc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2buvbsgtc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tjvmcgsn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pqoxbzsn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lcvfqohf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2utexrskh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2egtbdeyn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xydsbapr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjrsmwjy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kgkuoaor.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vnnfujav.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vwpuhemv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jbpfxdcp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2euohjttj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2clbkoroz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mtaorhev.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fbyonwbz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2kfqrycva.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ggwgwoyr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vkeznspm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqoifyzb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhefafae.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjfotclb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtgdmial.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jkbcgdjk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2shtnyiah.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ldbbzpcf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ezhygxpm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dxgxxsld.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ggjimflc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vwqyerud.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iraupktk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ndieawpw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qgmzxfhu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zpxxdozt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hrujveiv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rteyjjxe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rvgrjyir.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2reulwwvz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rfdzebyh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wmqcmbex.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cwoeygtc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kbdxrvnu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mfduxhyo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kgnxasro.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mlcphxhw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qezsjnlg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2atdembeq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrmvryvp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2swuwqncl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2djumvsfk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vqiudvau.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ywjqctsd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nbjvcmct.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cxaviioq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vkxjxjep.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ilhwcfcx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fbpadakj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xythizfm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rorcdfcn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bipukwok.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wkccpuhe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2egyuhkxl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wgpzlpgh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aunzrmuv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lkztlysz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mgqurllg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fxnbthtx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hurrhkts.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qcqveemf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hpwnnjzh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yvgmeucz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chajiiee.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nmdqzmvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlefifgg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bmnlcjjx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2btxgepgt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bpvhxtqf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bhmlvtnv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aenztpwp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sbebxgas.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mlatwpwj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdrpavxo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ukxvbhec.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hlmjrevz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ninmavze.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpnwaifv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ldvbgnbt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jdnrwvvh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wopicxly.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2iqsavjgn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fbqurqpv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhygyhcs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tbnqnkiw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nsldzses.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sfkcosob.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nincssyx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vtbmtlpd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zuoxicxm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ksaytpqh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tjbognmj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2avvriynl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bjoisnkb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2frtcyqbz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kvxrkxhd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iulavbfp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zertwxvf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2luqnymhv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oulhpsuk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mckcxfyn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2iswgnwsu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wqrtdcce.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rfudbuwd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yylkogtp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqxqixiv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfaxpdmf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2axxucrei.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zstyjyqz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytvchijv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvopnpem.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mnbmhjfy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfzkbzjl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hitdecks.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xoqkfyrv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lidltnfw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2busosrnn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ideggnkp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzvcwpvb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2erivckcf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tciuvqkd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ujktzjqr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yzeezkwq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zpasfsgq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lmzzatvp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hepbegzl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nqrgbvpj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mybttegt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xeqcnnqy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xpshbdme.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zvttxlkd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxffeyuf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hvcneedl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2osasfphx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bfjrpdyl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qnqaioce.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2dognniyf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bsmemgzp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vvzrfxcv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqzflpzm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vmegarbz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aawittyd.html


<!-- 参考信息 -->