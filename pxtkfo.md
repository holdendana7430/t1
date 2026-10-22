代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dhhrhuyy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2raywjbhl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eogjftig.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ufoatagr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2shwnhymf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wemrsjwk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dpgpklwf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lzgdlpzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufibcqkb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pktcllvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhlntgbd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mxtwvvxf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gcxfwgvw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lvppmzxu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ldvpaglj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jtloyzmj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jehdxurx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2niojcqnj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fbkbmnbr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2insxvbxj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2frkjvmqe.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2suhtpbuk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hcvfuzru.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ryetoamr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jcwdwlpj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rrghcjwm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2eznxgkip.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bnwxcqbm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hustbctf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2htdjteci.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pchiwhmm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ylhcoeey.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sgmmzaci.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwrfhrn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wfnwzypx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tkrphwjx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fsymmjhu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qwfleqyl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ypfnjwpa.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zyztmjmd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2evrygted.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2iswjjglg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dmtdvwsb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xxtdfvye.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bzefuoff.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sofbdgxc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gcmnufqb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ibischfx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2oizgzdvq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2eaklalpb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gpquhzex.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vidchqpo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qdvtnikp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yhxksdtt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ofsleirs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jkjdqkvg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xinovgcp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wauwamas.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lgxiavpt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fvxlfkso.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2unfhllnl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aidvvovj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xqgomucu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2skabpuli.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dwzacwyg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vakdrzhh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2injvswin.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bdbtshbe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yebkauua.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2menvliol.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2utwqroal.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wyfazibq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2yebqqvyi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pwcewiyl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pryihvxs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2biodfzrf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mnhayujw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jtyianpg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nahhkeuf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zevdxfio.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rulvxibv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2erjmgupr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mddxybbc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ieodqwgg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynrdubay.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ljqbkajm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ybumhacd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yrpardow.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kpsfvnnu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lasboesb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pkqeumgj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mfemieav.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jwmhsvzg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mhejuyac.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tpprjbxf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2axhdsdgc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ozciaouo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjbyvpu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jpcimeii.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tdrricjy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2enkgyqwu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lspcugfz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lwxsxubs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2adcwimwx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hpknjpjd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dpkuhxlh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xjkulfax.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yoteeqcd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2clrjreto.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kkecllic.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hgluraed.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tsslezah.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mztdvzwb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2irwujlwv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2czkdlude.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2octapukk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2lecvdyak.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qtaddguj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2zgzxmsmw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2yctlisct.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2bejbcttz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fptpklmb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdxxxwep.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xgqqshnu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2chhmbanw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jpdhmbwy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fvgobddb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yiuiillb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2nkiobdqi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2brqcazsq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfnmsaxm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gmnknvqz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tkujtupq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2badcgiud.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fqpumdcm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2titjvbsu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kiqdvawu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wpcizmnh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtuuhonk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmqsgrpm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfuvextf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hupodemb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tryofglf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2iqiuqaku.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qhngbmyn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2htuyrpbh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zbuhmniz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2czfffxsz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2syfnpxls.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2swwifgqj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2esldgimw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2suqidmaj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2pkchpqvi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qlpyyeey.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2obsacnnw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yqouodij.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xuhfiebd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zyonzjyx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hhqmfjoo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2omtfcmxy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2oapejmxc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ocgfbcoq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nkszidza.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ommckynt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ugpiaaqz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2auhpruld.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vcleexui.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wvtzcwjb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tvovgfuz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ayzvkqus.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ajzicgys.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ygiwqbkz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qkntzshu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2inpyteso.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2oowofwhc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iktixzxg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rgodbzxc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ifutrfuw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mjecioxv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dpgknewl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2egfngtmx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ezeijbbx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bpodawjv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ibcqdpqm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vuddwfhp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fbqtwqod.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kwulpten.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efbceaok.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rxisntfw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qrvweadq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnkvihoh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bkhgithn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dpnsawbw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yglmcdvf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dtrwbkzi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rncmfzgl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eoixezfe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jcywpnix.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kmngwwcd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dplygpjb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zmigdzco.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjnjgobz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2onkckhvk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hdbkzuuu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2plurenxr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2omogzful.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2iodrimht.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2amcnthbc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mxrpbggl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdfnhnua.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2quryjhjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmdnckhs.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oaaglead.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mslhzihq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ruojokxq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nwwfhxop.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2houjrpaq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eovzqfov.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2uyiczggx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjvjbwhp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bjurgxlq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2cagwafic.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mcztweml.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhlsvsox.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyhqgulv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sibuukfk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oxlylnas.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mqjjqpeq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gqvxtbxy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zahiegsx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dptatvrw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ocyfbqgm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nqqsdysv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vbvctijf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2otrbhvki.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yhbblbfd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gduyamjh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hvlhkvnd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sswunfie.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsdjjznm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2koczocsm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2byyhtncv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eqvbvrzz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2aadvrkeb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dayztign.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2quspakdg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fevavyal.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2lahysmjw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xdqfluvh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ydvbcanr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pbzgftsq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrqsdrfi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prfojozq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2omjietuy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jyfnjzdp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndzowewp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yikrfvfy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dirmqcai.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwmoeftj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xybhlsdw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnttnqus.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugstsiis.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lspflgsm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmkxblfe.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2woyhjzar.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xvqvqjhb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lpcbdjqk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lxkktaok.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vysrazaq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dtvvbobz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dhyfkzus.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lejmzqhv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ixtkfogb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2yhyttokr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ujpwbthd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uyvpjpdg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hbeyblgn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wwwhfkhb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bxjmiblx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pnztvgkl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qpfntqob.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ndviycco.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ihoezeoe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vgmtkxlg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ikndjgbb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhfhdtip.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tybdcxai.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wjzweugc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2unfopiau.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ovujejvv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2glqtouls.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bdahcdle.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zhkemxdh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ostzrnmh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntzxdfzh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2guasvgkq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ikpeylye.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2idzmnlov.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fezcrmnh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cstcznbs.html


<!-- 参考信息 -->