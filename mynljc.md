代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tehsgxol.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ehnxhbqj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2aszapqpg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qccluitm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2korslgnn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kkijoesm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2iqfpxvjh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lajcopyd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2frnxdwdm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjsesbpa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ncvtbzqk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2erjxqxxi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fcvfmlng.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pmymdqqk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wydvpcta.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jzrpkjqb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yjlqbiim.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vfiondsv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vjqevmwq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2muefigys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spchcdaq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2sgaiowhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuckwjbx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qgwgzykp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2maluqqfk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2aqejwmaj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fmdqdrjs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ctuuzpar.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2frfgwwfm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mspdiubb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zjuyjaoc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2txhwpvjo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2tpqydmho.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tgwczpqh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fkjpbqat.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ulkmftkm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hkxempjx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2atmhriaw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2aclccksb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wheiuxkf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hpuryzpz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uieiaudb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2tjaaparr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rmjgkbwg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pyveqmtz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ptffqzjv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ziozydns.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vfhxhyos.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ytrveekr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dymrnhtw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2owuveufn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sptruvxu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xqoonaoh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yolutbrh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2avlgvmjk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2smaxvwwl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wytxdfqt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jbylfnps.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zaugzbvl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fidxyxbh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tqudjzwm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yafowrge.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mnyuvmca.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yeipwvzp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uvqccjht.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2uollcihn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2czadsqut.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rpzphyqo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tvvrmkru.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rqqxuegx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mpxegkgg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ldvidoes.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xqmpsmom.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zzutxgds.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nnigeqxf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ofblryva.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rprgwjnv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ejbpmtzf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2mtnrhddh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fxldijwo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fvlscnmo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2cyzflmzr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2asmbyiph.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2znzgwlab.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2odfkcawv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kxnyltrb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qtrgzysh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rivumgth.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qyexrefu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hhafysji.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2adawuakf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qkuhzphv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2gdjavofa.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kxhlsyzt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2acrlmjbw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2uvgpycio.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxxsfmqe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2usmmlisq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ndlqprdj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yrulkqro.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2apvxsskh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lrczqnpo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zgwsrqha.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eazlsfyt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zbhmxpvp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mndaxjhj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wlhrnipe.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kjtkrnzb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2osxnfgvt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2szcvrpok.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hoohkawv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ymyswbrm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bfddqpdc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2espkxhji.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rzqmgmgf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sfwnmpmp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2czjocsui.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wsvaawie.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2twbdkseo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qdffcbte.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bflkatlt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ubpkhvps.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2sappkzer.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pxexxqof.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tjrfymjd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxtcubwi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qcnknaor.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vpxqtcqj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pjyfgeyk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rlqfhlxe.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nccehfih.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mjgnwdwj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2admpnosx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlpfvreg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjdocxpw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cxxbkjci.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ckpgqzhg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rlpjrrnm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2oucfhuip.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmrdneeg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gvbirrvw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fmwncsca.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rmeldeeo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gfjyqzsg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqiaher.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2scfsjwio.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2vifezele.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vajzsqhq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xurqrbga.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tcaprugf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oeuseugl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ezjhgatk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sspaohin.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dawkhizq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gdjhexft.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chrbeomy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jnngwkvz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lxsmjqpj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2huuzibux.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mjqcpdeq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rozuceuz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2codpwqwz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2khdiwuxa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2axctemop.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bavzxfyv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ecrayttg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nfzdpvac.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2epcmopok.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ezjvwnhq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ehebsoau.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipnuujuo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2azcopvyl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zwpptize.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zpkxeowk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2azabmrey.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2pjbetgzd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nauewfev.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hmapybsw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vulipliq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ptyjjrtr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lmkprtch.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlsgzsw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zgijplwd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lclhakbl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tinwjjdt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ozhofykv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pztjwgva.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2esmfdges.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2afsnyeaw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lcgceuod.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rbbofhsd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2uoqcwuww.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2juczbmkx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ijxnicbl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xmyrykug.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kdzatkrh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zbdhdsri.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nqchtsta.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkvaqqvt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfnaceux.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yzodosfk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zcbtnwzi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2eajgjpbc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qzapmooy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ucfaxqzk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2npyqzkpo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iaiogzzi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qhohtact.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qaekfjqq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2dtzqconi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fvvrosdv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sfquvjac.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2paovgmsx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2rzyinbmj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zvhtfcgr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cfvtbbmu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wgqnzugw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uuzpzaef.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2csrngupe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wqmrqvmc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hxkhdmib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxkzkyrb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ywjsxnvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dghzdncz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oyzctqac.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2etafhkiv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oycjlvfj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mqncgekr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sggzqrtp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2euuhpmke.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2expxjhce.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzlwvncd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqpygrzn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mnslsfuh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2vvowarce.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkjwxbux.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jxctypih.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stzvhdtj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ojfggqds.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rfxuwhfw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rumtgvog.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tgvwdnyj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2amojhqbd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2tychbmdf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eobbcugs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wzikqxew.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kjzvobue.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kmjottsk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2opmjncoo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lhimruyd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ygqotejp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2isjrlyig.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uzxeiimj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jhstoedm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yvgqcdia.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uljbnzat.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pnabywbb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ojvubdxl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zhohlitb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2itmfclra.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2falowjsb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2davffatu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czfqhphd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wymebapj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2liqfvimf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2envhdwjz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2cpeiwzvy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khxkvhqu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqbpgggf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vfcuwpeo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uosrruoa.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vojmgxyl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkrmgene.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnrwsqff.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2grrektzx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgherken.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqyizfqh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yagbgvmi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jztzksiw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ouonocyz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nwylgphi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pndkpymd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vidkjjbp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lftmpmfe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dcypwktg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jlwkxxwp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sexbmlhl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2spxroppe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vqqtifpb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylqqhfog.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2axozawvr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oksphytn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ijvgzmby.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tomyjkwu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bnvthujm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bxgzvazd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2aesvpcch.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqjfgadh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2njdcktdd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gkypireb.html


<!-- 参考信息 -->