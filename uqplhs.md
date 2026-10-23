代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wpvutihu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nrknfrkm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3fpgvefqw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3exjvgtpp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3khidmxgx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mcxhpgur.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rkycdlap.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eipkrlof.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3prpjsbcf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ihuvdooe.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zyxmfpeg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zmccaygp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ksvxzzzz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yhlxembk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wkaypxax.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3stiudczs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3paffloun.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmpqbql.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pvpfkkrr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eqyvmuxz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3lctmetdl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jszoonjy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mzxsteqq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3qfnzciwb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lpbnsznl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3enysedzn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wdxvaayb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3huvgfrtw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sjfbgjcb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3bpnrpucc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xjdiieco.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pvhgbbpf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3qihoxtrv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xjbggaov.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iviwvcns.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zzkuprqe.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3htvmfjwe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3agwinqxs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqcqilt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sjgdxylv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3teqxbudz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sqezqntj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mezsqwcw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sszwtozk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3slbvfsbx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jvxrweol.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kvxqtvvv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rxsfzlpk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fimipram.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3enrxktjg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3vtrjyapr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3agrcumvy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ddqbnpvs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hlkzpacj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sxgpivzk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ostinplh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3cdqgxzwp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cwotrnfc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vcoyxopc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zgqsbnxb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wvwigezk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qpvhmupx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mernairm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xkjzhoxx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3leqakldt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3saceozft.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wtwigdxw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fyunvsus.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3busteoir.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ytuvknnn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wzypgjct.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bfmnhdip.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oqrroylq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3teqbxhhy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nmyzodoi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pxvvbiyd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xygcnfvr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rwyihknl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oyhvrygp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xopxfnui.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zybuuaoh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yanxvjyv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jbswtdfs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3osbfaxso.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wkmzgjvt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yaqgpqca.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3spvgyzns.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bispvdue.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gxooamfv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uqlrlvdr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eyhzbgab.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yvxhnwat.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3cwzhiqam.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ndhiakxj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jpjcmaof.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ckkrkfff.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3btklcnld.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3oduybhak.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3coiohpvh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjzyghcc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gqioqbmm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3chhyuris.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3tbjixigp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxsdrlog.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3dpvgaebt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jrowdmko.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3iqlivsfo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3kfnrvlbi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3umfsrfcm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3anqtlhos.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hkaenbkx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jtykvkhp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3womubtmi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zdtfozqy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkumkane.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sboykdxy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3auxurweu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3fhoitwns.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3weueyxwn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3zbshgkkd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3okesjedy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tuhlgaxf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wadwpjlt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3kucpmqfv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bjftzgpi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3caswqeql.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zbsqlepa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3abesbaqd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3iuajeuoj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zzokzrvo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hfbrxrbd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zgtiirgz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bruqubgq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ijcaiiky.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rbzjjucz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtjgjoz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3yqetfiwa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3atezqbkj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ehbppghm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3azushhol.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rsuwdpjq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3exfbzguc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3euaawhsf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oqmqbuqd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fziozwns.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aaaszbst.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dnfifjnq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfsodzoz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xclawkbd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vbyhbwkw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ojzuxtvg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zlqhvulm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dzhdelgh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cbdnmixi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rwzikxrq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gexcxmju.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3bltcjwod.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gtdtjaql.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fmubrobh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vysogreo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3yinlkbta.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bgwppzah.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewnhtpui.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oewrgojd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3efyrbiag.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yrzqgvzp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tiqyfupk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gvqmsheb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vscxkkfb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3npskzlql.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nknrnnmk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qfsdpmez.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mvzlbvbh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3oiamhefo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lbfgiugh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lobdfitf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nuyogtip.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3olmfamya.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uqkaakgb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ymjoipku.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ttzqprxg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qqiwujig.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vrpzoisc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kvidqesg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3axcnhkkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdczlsht.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ydruiiws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sidslnpe.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zcgnrpix.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ayixvhbd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kbpauydc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jdohgpvf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cudaulth.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fjjypaly.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vruebgua.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbohvghz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lducinbb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3sdsrhdtl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gwsznnhp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqcmcbix.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3szhmhnkb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bguhcxha.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bwgksfhi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jhxtlzgr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zrsemyaa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rhsmlfys.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rpcovdqu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3sdctmriw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pgeoqlhu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pfrlthfd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uoorihed.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3axnkzhdr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wlhndcie.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qgkhszok.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hwukhgnf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3eraqrmoa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yutfpntv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ygrbhhfa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tfjqtjzt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hfrprvcb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3tqmjolwp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vnmifgto.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3yoeklwzk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hgqsvcpw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3lnrokwkf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zhspldtl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xmlampus.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjxjoihg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ccsxzirq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3izadllip.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3swkefahb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3asqyzzla.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eazcljvi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqshddqo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxgrabrk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yerieybr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqrhqjkl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqfadzyw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lieoopga.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3airghjfm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3spcjbnbn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vqmynkgt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gawhiihu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3massjnfi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ydbneoai.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xwkymkbq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nhosajje.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ejecjyzm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3swunmqng.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3okqrhvns.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qpsmukot.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lcyppaku.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3unjkzzwj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ewdohccf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3frafjwbe.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qglokdio.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qsjuqdgr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pgngaxmk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3byrnxuze.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mbafwtrz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bplblqlu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imsnkteh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xurajfzp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fpwqlwxt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3flgpbded.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jcmccruq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3uljakvkg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vehwusxa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3yyqaxumq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3otlkmdvu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hglvrjkm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bagvrenm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ifbctamt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qovzgyno.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gwqcpzlx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfxhhwrg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hfpueyun.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjhtmtel.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gtlbklhr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwdxjqlr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3slzbzftp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mblggsjd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlphvpkw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pkzhycmr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hyxzanly.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3djhlisls.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xgcvlbup.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3batmoypw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gowuluaa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gkfrkxal.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3whbuszlh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lunrrmkc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3pqntolyp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3qgbejhcv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3spsutnkz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3hsnvfswm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eumcvxmv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ldzbsmri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrbohiek.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jiimvabd.html


<!-- 参考信息 -->