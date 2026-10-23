代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rkxbyrsq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zhlxhore.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bigxumzk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zjmhdwoa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3uhdqivec.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3masdlveq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3knoajosx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kkppxxqq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mzqmigif.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3xrnnorwh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bvyttcun.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3veetbqio.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ktbyaazh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftsxpqru.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3urynunyf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oinowjoo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3abkhtwwb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mufezmor.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqspwxii.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3laafxvev.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3agvyumgz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftemocmc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pjqahawq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aydzrzol.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wsequbkw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fqwvsrlo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jvnsehbf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3taoaeqdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zujodrpp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3mtpucued.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3giudzlqk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xxnrfovc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ahmeitdu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jeytedeg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rrawtmlw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fizikyil.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3scwkyuka.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3supcctqb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xonhbche.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ssepxute.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3efbwfczl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3plhnopgw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gqbjzzca.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rfanykdy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dohiohdc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wjejaoki.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ljrszeoa.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fbfiqstx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3glqszjhq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zdxqlzto.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3dzfexgxd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gunsookr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xajwveko.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gddpjopa.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pyqxtopn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qiigmdyo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qirfkiiy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3srzuhjbf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3rinyppcj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pxlgkguf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3glhfgbzj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vapwursq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pmemfmxw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ldsulgmi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3irtbycgs.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wmxvqqjt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jruonflx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jrtwqmyf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3yxvciiun.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3aqhnuyte.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ahejvwts.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3rlwuihkb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pyycuurq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kysqpiyu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yzftnssn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kqugzxac.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gdqzlopi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qnurnxrq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kecbzkqa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3srrkkymb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uzfxfjcx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pnhefoya.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vhkcchjb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vwlmwylt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tvkdkqov.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vpawkdsn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3gkoqjmow.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cgcrvgsb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3grawtktz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fcqodwdr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vgnfjeos.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wclxvcjh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qtrygdts.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mwknarcx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rlosvjkx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3gftwumfk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fzpwupcd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3usklqzsx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dqnxucbc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fljjbzij.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gagoohcy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ohnzwnic.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjztaya.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fafhvaso.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fppdypht.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3akeyegou.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ndwhcesp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jkndqaqu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3evqpqmwb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ikooszvh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3cidbgsxw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rndkqplf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zeddmfzr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xxajiwjh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tezdyzng.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xyjnjvms.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eeimnkmj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ssoooubq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lobsnxbp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjuhfol.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lxcuigsj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xehrrkhc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3roziarzp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3incnfplx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dvexxbww.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3encbyfgl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jcnpfmfj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ysoodzlg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dzstvwlc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qqxaakny.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ioksbeao.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ogzykhmu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3muobwvtv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yzciommq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ckidhqbe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jakwgpdt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3knjfuzyq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wgkuwxfc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xrduzbuk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bwqezjhq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tiesvsoc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcyvrjwx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmkynnnv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vaudvhpg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrvlktoh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lxxaylgh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cgzqkuto.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rroxoonf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jkunfdmb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dvvfdtzw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ltcaaeec.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mjkrzdrb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3noheabwk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dpzctadb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3noyyitrf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xlefyifd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uivokmid.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qiggyfpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhyzepzc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dqyifwur.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgidsdfu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hbvzilbq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lbfibjkd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfcvrdcb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3cbosrsob.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vktzuwwb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pjsodznb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rdokvfoh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ptzfhsik.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3patzplnr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mbrwdtvq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tolhusdd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xcbkhztq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wavajhwk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nfhbmqia.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kodcgafn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tgyeouny.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qhplrzue.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjyaplke.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oinybxeb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ptgmseqo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3amsfartb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nmmhaoch.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ygwxwgjd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3bulvdiuk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3uclaxxpy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3epaggstu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mlqtywqf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uzdbrcpx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3drbxipvb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3doqafqmp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zkwefpww.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3huzilzlr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3iuxsawtc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jgjtrkhy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rijchakf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3juitetek.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3anhmizho.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vwyojbff.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nkfhlkrz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kcwtadiv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jkwhkhwu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wadnjofu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ithtzjpc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qopvzlrj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3meicdvhm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sjmsosqy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yglzkezo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3eywecgrc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bsgvwfls.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3dhflnkoz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3kieoocyg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ocioxtry.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eeohmnye.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nukhnvef.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3znnqcbml.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qtgwuzol.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3kmhbsgmd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3puqizueo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3svhaovyw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vuuzawhp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jqxnkuta.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vjikrpmt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xejqgucl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fovjyfxq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cbzlxjno.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cnpouvwu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fjqmoohd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tdqhvpjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqmepsyl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3zoejomun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtvmmwzg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gzdfzesk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3faclgawn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qmougdik.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3rtngiryt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bwkjdjwe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qxacllyq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tdyqatcd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3youwdvgh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bltlgsuh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fuvqqiyh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3oynysuul.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhwgicgg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ehkpkerr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ikkjmlix.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jrxmhpvh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xqecnfzg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3extwyonz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3iewsekhe.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bmuwbdku.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kpxshbdd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ligshiwz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3agtjmpwl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pjoolrbu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sisjmakx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bnzxufbz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3juwxhszq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jptytser.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zubsvmqh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iixfpwor.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kzhpdwjk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rdrmetcd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3femcopkb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxdexik.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dxvzyufy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fcdldcqu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cnqwsmku.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vthqqtkc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vhyosjrr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kybstyeg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxjoqlvh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzyjjejh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gtvpczgy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3krffirrv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zywttglj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulxyjtnf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cotlsryt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jxsjvhrm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rozbavqy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zefgmymg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3byzavgcz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jpyidkyj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xximpacd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlwxvfky.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3taxkuyej.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kmhbsqww.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhcjlwb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aettlmke.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3unorcoet.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hstfewav.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vruxwdnb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3oqlmstxl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3knjrhwty.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gehecvdt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3aldyhjud.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bqiuyzxp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3pyemyfxc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3perbrlqj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sddhdvlt.html


<!-- 参考信息 -->