代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3egqlmjam.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvpaueti.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3phjytazg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxgoctmo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hebwvcfj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3yikpyddm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ttzokwwv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kdbogcce.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xsubhpos.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ucztohec.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qsbrbevs.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wshgqexy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ohubgexh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gghrurow.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hgugkmhs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gywemxml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qecohnhq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kkwtmkhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkpvyxmn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ncntelok.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qzizvngf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jbmytcks.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ttgrvwop.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dneonuab.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vbrtbfbf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pepzkwoo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zsfgyxxh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbjusmsf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iapljygo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uskecuhp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xhqwyffk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wcovphmv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kqcfocfh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjnzizd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qrfzixxp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tjnzedvj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xqlmzotm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xfwndtvr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ccmdhhoc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ddrdtvbr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ijpzxlwi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rwkcyfco.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wjeddulo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zhxncojg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3atyohhdn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zbkwtsax.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xrmuhaes.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fgsjmphh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3chgirtcd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3uaxfrskl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ahhghblk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yvmjmlyo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ixxlnrur.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jomkkbnk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aasjfdnj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kuofzifu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lojbaufn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fqywkstz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pjspruuv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zipempys.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hwqtglpv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3prkmysnf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cicfluvt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3asiovowh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ntivdhtt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pzhwxzvp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gizgxbgg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xjpxuahw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3paaelwri.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iptknpbw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncmkgwmm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hlptmqon.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3whlykqbi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ahvheinh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hbzdiwal.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wiqhofuk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ephrfywr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ppavntdg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3tmonmriy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dnjblarf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xlghxddo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rdcwmkus.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wcctezoa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3avslqxcl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ajkkuzxx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cnnzhjdp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qnfkjjng.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tafqpfil.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mutdqpnr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tzxapsrw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xeyhrgag.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3goqmjshi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjqgqwjh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqmfrhpp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qzjhsslq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bizqyqgk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dbcymbal.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ysruubne.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3adiwrtlu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qwbvliyf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fzqyhstf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xycybrzc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qssnwzgq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3osnwhsdl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tcxmkpnm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dqcgzdsk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pskshqbe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xumbzuqa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zuatpvce.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fzrhjxxy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vjwwawcp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qklntmfp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wzloeoxx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sncfyeik.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hpcsxflx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dcukgbay.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fhligume.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ugcyultp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xhidxagf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3guxdijwl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jzzlglsz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vbxkrtfe.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xunkwfuh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fifwuosg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kquwgvud.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mlaidymn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gozddkrz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3aobecnlm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mlqgwtit.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vagifozb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfmvhsjg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nmvjisfm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vnkjydwe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nmmmeijo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vqstvevu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fupyhlqg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3bspuqjzt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3yiaxxebw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ildvkmus.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ucsntfri.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynjetdqn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lofybqzf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jdgbnywb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3navzvzkz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kacmvpcs.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dnqlvwbl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwxkfdgt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qharnymv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpvdlhnv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3naxmtgbj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3blodcemj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3pfxrpgez.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3txmstglm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhxujqdt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nafmpont.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3acmybalz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xmndcsfl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3djxomjup.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jdvsjxhi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ojuhkmog.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3luljhetr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lihbopff.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rvnkpgym.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rdlcmrwb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ozziqfcf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3isphindq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lijxtypz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ejzmhysc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3blghsmll.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ytsdlegw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3joecaydr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xifyfhgf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3bswsxpfr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vtgsqadt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3odompxwu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pdagitum.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3svxufaux.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rknlnzyt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qfxsvpip.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmegushr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vahqrywm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pfvjihsl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vxxlvecj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dlqzfpry.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3embhshmv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uzemrwpc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dwkmhjbp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hxjrtrcz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tmmwvtmm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zncvqecf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zfuhaxol.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3iarludrl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rbasyezn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szpuxvqh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pcbvivjo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cedjefyq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijllflda.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mhaoewkt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3awtaefwn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rfksslvb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ctuvjgsn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uxchenok.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cznjuswf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jbnjtzhe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3csvgcipq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hllhsybq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eritvfgd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tgigasxz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3kuydjezt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymkwaqla.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jeiajniz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hzugznor.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3czxzpxna.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ebacdqmf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jgjbndfc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fjclhobs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3iseabmqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frgucbos.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3grdofaaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqjqpwsh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zyhoeyev.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cgzebvqg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tojxycib.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zugumsqq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jphgakum.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sizmxlgq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ltnhnyus.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqdvbscl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3scgpffvx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ithlhmjy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xgdqbjyl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kjfrjtql.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upczyrtq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uugbzknl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ljxxbcaf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mnetznjc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3thhzjgfs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjksoroa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hokxvhzt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gadlozvx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ewjyfuba.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sxsjtzqh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bdguiguv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xkckqfkp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3taejuleo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eueulgmg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jwpvtmcy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ydnuriqk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ohettbnz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qqskhrlh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3aubcarpp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zvfirsdn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3tvhhgrzj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zxqguhhm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ncvwqbjl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3kttamjet.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3tsiuezmu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pbhnrwpn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjphgbqp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffsgxzgk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iuyesfgg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dtiooafc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3oaexboev.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ummehxwy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnknjdir.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljxkxmyk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wunglnzu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3edstszqh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hewuegux.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bjjuyfxp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pcqkanpk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nkioggvs.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzweqfiy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3twyjizhr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cqgcxzgi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nhxstkbr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ufhzoque.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nexhppvn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vbkdxjpf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cggxcmqc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbywnxc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dxmjtjlu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cddykvgs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3reqgpcax.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3diumngig.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuhwktpp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hkhwilmo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3scvxhdey.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sdrpsfpn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hkjjrnmg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3grwwwpje.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nfirmirg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dkdlwxke.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3siynvzxo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bsgkkcyz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wnstsoym.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pwnxgqhg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zkrwoboj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3byxgyutm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjshokoj.html


<!-- 参考信息 -->