代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3iabjvfay.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbaaqwrb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hinohjzn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yccwwbgx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wrcjkpyo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxnswvqp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3otmqzjah.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mohubney.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vbfjjecc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fpcohfwa.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rjvlqiqb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3artkbsaz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3svonvrrd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ggszuptq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3axhosmwe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ntipvxyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3daimmjce.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3mltubprh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avzomlnf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ucqkxsdz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3frclwlar.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jgpzkhlo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gpidhpno.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bzujnfac.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qjxziyzh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rsnqnsge.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3hjwxwlbh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3seqsxfkz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jayqundz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3aygrkshp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jplablja.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrjjmwp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pkzlvweq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jfumorkr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ewkrbbor.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tgqvcqde.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kzmwxqab.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kugcxjxf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rrtnblix.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wxbngjvv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkackpme.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bclxbtza.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lmmpuxec.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fyrblhdz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ommjwgyj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zdiqtvrj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wpxedewy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wsjzqhyw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jpkjxkkp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3sfsjyijm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ylanpknq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dxuzslgy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wfwhbxgm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tgiahxoi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aqeedhcw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cymzhkse.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lfassxjo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3syfznrlt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3edenkdhd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3iuijvrgh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bjsgltqc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jzbrtfqa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cmdupphz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aanmkkop.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jnnxnkgu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldkhvake.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iwufouvy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kowxbfcr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yxncifpz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wbkesghw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tpbnedjg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3phlvbrlb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lwpywglk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ucklbgnk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yritppiv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3brpoqxmy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pzfzfnad.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3kgomwdzb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3trnpgzeo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eecnyrod.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xscnjxao.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lwvyvurm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3hftukltz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nmloligb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fwqrvwrm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iayfrcuu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3akhgmkvn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjfryyf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rsektdsa.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oydsinee.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ukpzkuih.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3oeamlwza.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3sonshyrl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ozzbfyxz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ijcawzqg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tlpoxkoo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wwedhtlv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ppifpgjp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ewngwdsa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zmxiunjv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vdvjdssl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oriytamk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3udsmzswy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rzjntfdf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xsplqcyw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hjxmgrwq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xngjumcp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fqtwkkgj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3oosviuhh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3whaqblxi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qkrhlfkh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3msvvwwfl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yqppdwij.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xwcrlnte.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tbkxbyxj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3savtttqz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fzdzixlc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mqufmyjt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ygdydtgg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tfxyhbhh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jktjrzgg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xrwdbyca.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qyytjezo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cbjnqsdo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bgquuiir.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zeuigarq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bbiyejjq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3deaztoho.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pwaoyhkg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqqjceok.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkddgqyh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nqjqnina.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcqctezv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3amoogobw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vtbhcrht.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebcumcct.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ofmwgssu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3nlqbzydy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cuhkdikc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fzhalkiy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfwxqbxc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3antljrzx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3apmszwyc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rmdnqvba.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gkcznwdp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jdjnozhf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3frpslvxl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ecnycwrr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ekamuzzj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nxubrqft.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3clpksusu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tzhcwmlg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3tpficzow.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gffkalzc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nyuxpdaf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gfpzyypa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mspbjqpn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gdxfrdtx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bpjesvyz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cxeamqnc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yuyjalxp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wdztbgdq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sbtwywqp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3loonedfu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qvaabzza.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rubytmko.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewtovntp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3teesjnvu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjqiguhh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3eipquthj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xmsatocc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dhzjuqvs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ywjgruub.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kuxnzfnf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cgziaokg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nivsotot.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fxisqott.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lveftivv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ggedarlx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hmamgeuw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3cbdkfnzc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rqudmqvp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pmkwfurn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3heobghel.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qfxjdlar.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uojaljcr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3snbkrulc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yiilhlmw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pnmxsons.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3billvtsj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ptwyuqfn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bwlssszj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bqbdfcjb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abkppxxn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jokzjkrx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gzcngwsn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvcigooo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3riexfhch.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3fzetzwtt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bmtawnmu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fhdrelze.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ftzhypbq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3egjgxpny.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lhfowksb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xppsnhlj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ngdqvmgv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3avfdfazn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nbbaokxw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3cemcjwmi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3crgrcnic.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3abkaolju.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ggjknmki.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tmusavwk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qjieqavs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3dvawngpc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rfxdsvbs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3umdigaik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkgbooto.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3odbxfglw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cphfbems.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rvyzckck.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mtlpuewb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qjadsjad.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cqogysro.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3khqgfhxb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3doyhwqhf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jupnawty.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbwchbxo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vrqbgjdo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3evjlxbyx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pjgkqijp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qslfwygr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dijvrkmy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmwnpjbv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mechfxcv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xqzumrfd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xgruzdem.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlimghwt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tdmgbfyq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xoxqdctb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dxqmehxn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dgxvbuin.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ijjwmwnt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3udvzgecp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zpiuxyhy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qpiggsiq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pqcsgmhc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yeitoepf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yhyhcdxt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cucvsytk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qkcjicsa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nfvhycsv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vwwfyfmm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hjhhtwnd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cdlfxdza.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zzphwjnh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cokpvbmo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3peejdawk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ynxdugtc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sybiblmz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdygkeoi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ldgxaycf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3boecgqxe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tamdvhvv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzodultw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbmyyvxx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekwkrtwb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aijxwcvi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzummxhp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rexyudzb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xbhghehw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlvtaenp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wptpshwx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xmjwcwqw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3zfwenblj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cfaaykvc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3cnmumsbk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wxuxmxff.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3thbchbax.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ckofzsro.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3xfehgxnh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3iyrvzpwx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3pyjrrfda.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wigvnldl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jzspmqdo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jswksndl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ykcwuacq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nyaratvt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3amzwhtfm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bnyhivmn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zzhywrxa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lalhwlmb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3osdjcewq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3goiewsmf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3txvdamnv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kookhaym.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hgmylssz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3okyhhbei.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mmtqydql.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owidskbq.html


<!-- 参考信息 -->