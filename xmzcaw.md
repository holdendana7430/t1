代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zuapedwr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqdalxuz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3aoccrqqt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wiykedxi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jzdajpih.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnortto.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbureorw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hcfyakmd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uhyagimc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ourqavhr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yybxymdi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hpjuetfe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ghvgnpmp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kgumabgg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mdmhtgky.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qpcpoptt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdzvowgz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vmysjidc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbilebax.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pyzlfecd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dcztgrsd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xnctlwcq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3crlkidiw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dpskjscb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kstyxltp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3almupmgn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3hbtcwuus.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ahcalydg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vkegxeat.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rjaukitr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ettlkdqs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rsfhvatp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uigylmpb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lpedhbjk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yshrgytv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kvjqnleg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qsuuuqxq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ojuvhcds.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wznkspoc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lvxnpkgc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ezicnfiq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aqnqvkbx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3roampzbv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wlycddnw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3znjbrjtt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxsqfnmu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hgzzhelk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kecjqqxg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hhqgkstb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3adtoomsd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ybpfitgo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rdizvyye.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3jcpsmjoe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3iauzxetw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3baujmdhn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3eglgphyf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gwladesq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nomvqtho.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjscblq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ztakdjrg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3osekvwwb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3yocrphua.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hvstvild.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pokzzgzr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3avebppro.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3itufnodb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3occfimvk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3htbjkdrg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rgewuzrc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hibrwptw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mteqhpzw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cvblcktz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3efgpekbl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3neiktrxu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ukpmsrrx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pznfiyos.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3umehnkso.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dmcyebzp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3tjwecuqf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tdjmousa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jxjuxnyz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bhitpiex.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3iyhowcjz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3slqeabse.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3onubmsfh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qolsxsvc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mplvgyrm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gfbhhxyp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ebmartcy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rsdhisqn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ijkepads.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wbitixya.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qyvhttli.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xvxrjevp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ejqovdfl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3boudllvu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ztvpfmvu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ietkkkhh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pwswkgvc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kysrdokr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fiakhgdu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ijrzkepl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ewxkmekb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fchohhop.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kxlbavgh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wpyvnakn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ovbzbjbp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nyvufxsa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3miwxytrg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bdfqpork.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jarklqwd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cejkqbjw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uqpcptli.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mcbxuxfm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3siifrcvl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rxczbjdn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mmzqgmvx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mejnqlpq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3reuljpga.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dnnmfzds.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3euxelmmy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3itsiewxm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wveuuaxp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xvvpwtdj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jmylleuk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cfxhzxpb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ixwetqvp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tkydtiyl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3odwqpked.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjmccbxg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlikxkzs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jajycblo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwsypkjj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qonruush.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3izshynrh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3knpjxwva.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wvujtfld.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tdajychm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tucoddug.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vklkkaat.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ysehhrcq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mosxvkvx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mpyulout.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3tpdjnhue.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wxnxmvmt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qrjcedvj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yahdjtsq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rqovuruh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dotodcvl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nppejbiy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3imwgyirl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xzazjxrb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pdtnebro.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwhbfzuu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ppvsgsyc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ehwlxqqf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3pyzqlvpn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ujlyemob.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hdwykvfz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dmjdumzn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hpxrqtpr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ckwqqjks.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ewbitvuq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vaokqltn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dnfobupb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xyahgsxt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3etcmrbqf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pimuqtlk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nxhtfqyk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3phsequcw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dqgzpfiw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hmlabgyc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bunvdfcb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3nmiqvjpf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3adpgcthf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zlgwtdpm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3canaamsd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ziavafbz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3spxilslp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tfjmvemt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqrzpkii.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ubcusfds.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3nywopytp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qldtrdew.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qfgpwlwq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fgcvqkdt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3bkifyvfc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mhouwoyy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tkhrclvn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3yzgcujcb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3haavwnsy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kzldlzgv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jxxfhone.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zrdftorl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3buksxbbg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obqpkdcg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kurmzajq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qkgqiooz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3lelzanhi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ovhibjcj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jtojqmob.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nqtimepu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cbrsgmrj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3epjaqnlb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bfsqcuhe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ibhokopm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jsqxbqdr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3baweogkq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wewrjkws.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3brgsyfuh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jvghuupd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zfomvjrx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3trmdemxd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ythkceto.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fyolluos.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fcfsywml.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rmwmazst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuybwfno.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vqixldwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvrlhtsn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gjcbdkdk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hdpcwwxx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dhvgyphv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qrgtdbyd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pnerlruf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lbpidavd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gxyoaymr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdqrvqgr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cflkhepv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjnzbhnj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hyjergwy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ccbegsqu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxwpydld.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3djbejgem.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hllzgyyr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jcilwgex.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ivvrdboi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3uoxhyfky.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3utdduaba.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3npwxxykz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3utgcdeag.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3llfmebtm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qljueibe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3prdhamzp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fojzoqpc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3kvhgijsw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hghhryin.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzuzhxjd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yjndmdwh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3knglretp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rrvuhlsg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jxfqqljf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3uteibbqb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tadkhqgd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3guygrual.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uumrkkfu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3etprwdia.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fuinqbgd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jkexmiri.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abcmwraj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhujdpan.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dlsowpio.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hzuxvwev.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxzsepky.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uutmtcfb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3auvasmzf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjsfsagm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ugxzdtsj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqxcwugo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3byvaqpzp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kqykzcby.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vspeqvxs.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3imjjqyvg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lmoqymzp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3crowjrdr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kjzmdzzp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ycohxrsk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fjmcscjx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fmnctgbu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rmvbcmxi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ucaptvoi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fcugcnnu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gxhrhvvd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3sjceymbg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lblgzvra.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzjnuyaw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3paonihhf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3szcjzdxr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lvbnavtp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3frvqtvvp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oyhuxshz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ygsrfrpa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yxmqokmq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkimzzze.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nvvakknz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3oivgggej.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bnlutmmy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cxwferhg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3uaxklcwg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmtkendx.html


<!-- 参考信息 -->