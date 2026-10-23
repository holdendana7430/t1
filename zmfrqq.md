代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lcawihaw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jpfntytc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3amdvfkfz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ocaplhdp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3duxsahwx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iazqlwpn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ivghegqd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tcheezra.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lsqzoghh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nqqywpwx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3iacdazrc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3prpbuqzx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3inyqccvg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mwoeyhao.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3enohwvwq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oeewpxdt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zheygeja.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rzpwipdf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3megqdkms.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bpzliskt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iclxkkui.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qupqamcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pexkqbfh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3khftwoig.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vvujqfdz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jhowjssf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3isrlbriv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ydulpriw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zoevcxxq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sqizfnwm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3svvczxdy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nnoyyyrs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pjwgjpzz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tpajidfe.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rknwpgfs.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ggmsvuxc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hfkupmoj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbbtbovx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ivenrcbk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3erceilhu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fqxlgitk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tvqejlnt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3abaitllk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pldswdpi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jcirpkam.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ndpyqmfy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cunijvib.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uucklmxe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rnungtdo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ikkckcib.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nlkuzbpb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lbafwozb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nohuebmi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3imdbxjvf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wqdbbvkx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pvhgqqnl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3jnfeavhm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hvrhtpzf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hgcrkqgz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3obrvytge.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bcbyzlkt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qhqiuarw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jlkajfkz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zzmmgfzq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jyojrhfz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zngxpnvh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ngjbojvs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lfzkovsj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xwfokmyy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ddxusvxl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mluaqzzk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3splsoilo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3izmhnwcf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3namdskes.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tbgemtyf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xwhuhpyj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3shybybuk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ktmfkudy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3avgjfbce.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3worzkbex.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hniudrnt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ffgrkksh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fpwegadz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogowzyos.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3emmypean.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3cgaclyte.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ktittzsu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3iuuvyruk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3cxthqrfd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3glmcwqbj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3umembhar.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3urbscjhp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xyjqirtb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nlsirssb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nggtrdkk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hbwhjgiy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3imtoynon.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cqfjxkxq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3synsivek.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xjqhajix.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3icwiihvd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qeovlwbn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ilihatmg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bxhymlwl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ivualsdo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nfehvmmi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yqaeoizm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pmrjsrts.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jjdvxuss.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qsnpqrmx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dnvxogry.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qgvixzwa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ybtgmzwt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jxpfokgy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3csuxumuw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qakcsari.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sqkqovlg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bqfdftsz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pqinlcfq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tmdquees.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mxlkvfom.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nomrvswt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uodhlhfq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tieoibgm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mftpspyi.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nidxtmcv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jgskdywj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3yipmdnag.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3okmpksza.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lsyabwzf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3aizyvekq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hfsgmdyf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3buosnjub.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwampxnm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3opzsvmnf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qxbqvurr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pzqvqbwc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ugoonwzs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ruiyofql.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcsifgfy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3idwmteuu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zpvqigbm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jdhxhyii.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wmhfyjld.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvbkzidf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3idgxlboo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zmshltok.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zhpzzhei.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xtdxidyn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hpizqyya.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3msrmrlzb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xjgjfssd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3grgwonnd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fyaezcnx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pfawynvq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qnmjtuhv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3plwuhpuz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lxrlettn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nquflnlk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kcmardxk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mbbnnzhg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3asmvetke.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3eoosauev.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3etphhfek.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mcrrqdek.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3cespobvc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3iotfyqfq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3utqnvplx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ywguzfli.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxyheiec.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljerqyaa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iictfyid.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gfhgelaa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lausefjh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xutzevxp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jxbijltu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hfniryuf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3oglcuvnj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3oktaoubl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3axbjygfz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3htkjwedd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lqjaoync.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3myrxvyma.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ohyexcir.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlcfhfyd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dbgtjoio.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rrqlpyza.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3trchtvbr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rlrttkrl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3plybmahj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jkrlxxzz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xmyevzqn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kqndmfar.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3etfbhtpv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xvvcvnop.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3sdhnoque.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kjsgreci.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcrpsirt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3deichnlu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmncdpzx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cgipvaoa.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wmkqlyfd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3girmxkov.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gtyhfiww.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qesmjsxi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3plyedvzw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pjynrubp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3svihtgef.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cuwdzhqo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dwzblvjl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qqccetud.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rkugnjlj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dyjbyitj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3eelcrgyx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qjpcuynp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jrrokgmw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gvtmljrc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yeeuqrrc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ytxoqxly.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zlobmiry.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jtsfdfvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zephqgsa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3crmxbsdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iivdrojx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gvzrhwsz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hractyxk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3legcmkpy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ssmxuuug.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cnqdvgfs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hctcruao.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sbnhdlvq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdmnpozx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3flbjjlge.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmdleato.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hduqfbeg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hsbqpfwl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sadfjtzr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tqplfnpd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yivitwqh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3swbmwlnz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wxjlvigy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojvvoemu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3cxfpzwvm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3aowwhzip.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hebktzvx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3trjxxusy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jplhgcir.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ctbkyhhq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3suugpyfo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aridmywq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hsbpryng.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3sxxkhakd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mjpddsop.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3arcpafge.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fioljywt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hnmgpmll.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jmkxuiei.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qmwhydlb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qtlpjuft.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3almikahb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zxfiwowb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3otywhdfa.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lxhwzflf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvszoipx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mdeoebxt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ozmmvwdv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3owjzcbhl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqklttkb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3libsqujc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ejkkyanm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kuikkqqt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vhohsfcw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjwwqlsy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhtqrahh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwpoxukb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nepqytnw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dojzcntt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gbmtgeqd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3prfphltj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lykjnwop.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3buqpuvye.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3apmjaaoz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dmhrcbum.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wpcozsft.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ucamvayr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ikcdkyls.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3axtadhzz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ivznqnrl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3spgtgxof.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vkrekoww.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nfvanoca.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ztobdqoi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3motbrprz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fdzffbbh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kpqkvtny.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nrrrvapa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qgaiqozp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqnchmmp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xxjsypya.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hcilkove.html


<!-- 参考信息 -->