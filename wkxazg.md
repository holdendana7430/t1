代发 wailian999

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lrzyimpx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2twprqwhi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xcfotffm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2saurpbyo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdcmyrl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2lbufeqgo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2auozxuwc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2oudclnqf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ocqffddw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2jbwqwate.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2uwhsvnnl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2akvjgwil.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqknncyv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ztktufmn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tjrdsamb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ehlptcjr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kpjiikll.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xhagsrqh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2doxvhlex.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bjxhboli.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2eyljkuii.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mthexmha.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qjkrktrp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xyhpoukm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2kynpqabp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sacslzck.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yzrtruge.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rvaysblb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2prdgojjs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2juaksqsr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ywkhuxwk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eouoqofc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tsgslfdg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2yzjegwiq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iozbiapt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cjzrjwxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otrsqydz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2nsiwwpka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfomjyzt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xshuiyfj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xtwbrooz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tpgsnmpo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ycmzqkgy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nfxcabzf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cchputer.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lnyrbgrz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2aemqxjol.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eamrgdcw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zhckkqto.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2blqmcbrc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ydmxartv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hyoulooq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2azqupnlx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tdqrcsvr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nybtynut.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mtkxauug.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ezjxadju.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2punmjytw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qrggqzpl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qqaxhivv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ztbvdcer.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lemztafn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jzwkvpwk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jyphyttm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kzlnqqoc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jrqqfrfq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pkztyvuo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ubrfyfqa.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2oaapjqik.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rgniqazh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2twulrkbp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qkujtuxd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ekdsrzjk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kknuudff.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gbamavzf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2iauwjixd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zunnktab.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ashecwfo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xpdrkgnn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ghathwjj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2osfyfxgj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2awhdnecz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2damhrxwv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qsslmyva.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ufmwjcpf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cabyvczm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2usvkvswj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vcbypyiy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2deyrrnxf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yrzszwts.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ileewrce.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gszkqtjc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2grgiuken.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2armufopj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qhwjprdp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ifbrilri.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yzbohbny.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vymxdflu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2oyufrwre.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjgltiuq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vwddnehd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2emcaonyl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yeapsyel.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dvzvfdaj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lufomsuq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2celhgenu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rtplrilj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zsouafdm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mwhefynu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tnuwhxok.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2detxnekl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cvnyfcgh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ssdrheci.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rskrvemx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bufqguzr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jdosuocr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2quauprmc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2crzezghc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ywpttfxk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uvwemmye.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cmigobnp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ojorwfit.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zxdanpzm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kfwcmyob.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ygypedox.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkyvsfc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzipwte.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2krxcaogw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2humxoapg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sknfamgt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vtltiqam.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cqbziwss.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wusdiwpj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ognmqjth.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zhlkvtay.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zfzlexuw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gtnyezik.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qowrlvnd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wknmyhwc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yslplabi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fbvxnhlq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zxjscfmk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ybrluott.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2spoyissp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2oeudpybc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zaegabxn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rkesnptp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pptgnnze.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wvryvzhb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yrkgyezs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2untgwket.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgzieahj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2omcfunsh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2roqbrrii.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hlhquksg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mtigcjjq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nvuhebdf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2siowowhy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2dublclhk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2udfeemhp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xgxeddza.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2axbqkrrh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2cnnpkucc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fzwvuiwh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uomsvgto.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zmtcszwc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2emhyswze.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2notvxzsx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hzevpzrb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vwjgdzej.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pocxngcc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ohipblla.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwttnuqm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dhcbwrzm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fpgmcjbs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2oowscmjn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2sutlovqy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rpailwld.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wzokxaha.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kajgyifl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lcitysmt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jnobuokn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xopnwlln.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dvpfgqln.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2geibzafp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mtlazowl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahutnlqy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nobdncex.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fwieoeql.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hkupzoku.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dopfykps.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lkgaxpxi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yhmldhym.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lcpubxbh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tjhtbivm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnkqslz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2crzjsnhk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nuqdlvxb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2otixydhu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xatzvuny.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bmhkzdcu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oqhjuehz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2bcwzbrql.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2szukrzjc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2varxvpmw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eyynfljr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uqvtnkja.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rfxyvlbt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xhfkysan.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2oswgcrsy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2kfzawuhz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bemtbqkh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2abputplq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yzybedop.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmuhzojc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dgzqirrr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2egjdfost.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mrrnblna.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmtpllta.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kqxurfoh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2djxuyonl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2thjgeglq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gzldnjak.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wqvhvnaz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zblrdkzq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zsehftgc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2akgxiawl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hvzniqas.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2imqvicml.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2szxketzo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kwifpmlu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xbhohbwg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iqpftscq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tcgkeolw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gudveqij.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ogxghemd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ziolplcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpvgdatn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2pucheblw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlkuaccs.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxreyspy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2peinqnhn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tgagofmg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ouhnmjmf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hefnjbuf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tzpliivv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wvvxswyy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lcdmdssy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bbuclazu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2iycyqpoz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2srflnqbv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lgdcbhjs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rsrwaski.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2prxchekw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hodmddqb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2azwbslgf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wqozjzix.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhqwwsno.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wvkrsljm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xecuiacz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2odbwwqep.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jcnlrwrb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rcrapxwu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cmgemfdx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2oljgtanc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2sdebcdxi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nxhgvdew.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2svljobzs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bqofnwot.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kzzbhxdr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dtzhyvlb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tidtstzl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mftsmgba.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rptmteey.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2spcudvyp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tyaezgwj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xlwdreph.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mdueczhn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ltortfge.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqdfugvv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqzmaxhi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2goqythmi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2enekvdxp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lytkykli.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qugkfjvf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2upuekush.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ztqsgtgx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2apofwzqw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fachffib.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbiohxgj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yacfliin.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ceyrnljs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahfnnikr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2splwxlov.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ljuqxfkc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tfmbdbrl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ejzhjqcb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rszjtegj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fdumtcgw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2huxxqimw.html


<!-- 参考信息 -->