代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uspsucxp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hozygtqp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jrflbbwn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yasewbeo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2oubtwkqb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2uvflxxwt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zqhhmwxv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lxsdrxlx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xkxcmful.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bnajbuia.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2uwcjqxpt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pukflloi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hzfkwsld.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rmtctvrn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fseuuofb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rsbgqmeo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2subinjxs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rughufqo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2izlqhofk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hzuxburr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ymzxeqfq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czhdfocw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fodectkz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2awsvczpf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fqemggny.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qakhtajz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jhxzjkac.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ejvvnbid.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ekdoltpo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hsqaftoo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bqcrkuvi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wucjimar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmfjnywc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2sbuvcnlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhelpsam.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kcgpsrle.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zznvcgty.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2siakkfaa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vfpybnri.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kwuskeop.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fcnoyteh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2odifwzbu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cbqziags.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mixwwtvn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvegwucn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rymsyyvl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwjxqjwu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2crbahwjf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jawzkknb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hvyizgin.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2algdrxeg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ivqpqjim.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wmyuwcxk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cazrlscd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2adqvrxtc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mquhywex.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gqovscnk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2knrgudir.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hnsovsaq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zhopwclx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zsloiqfh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qijhslkk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rxaxylix.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cimcrfgh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2yjvihspc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rauvomkp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2csrmzxxx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yyicqdmr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2onauorka.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tquxvwuc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ztvqqhbg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lymgyyti.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bbtaytkn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2egkotbeg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2reomvtke.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lpaftevu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ossyukdy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nnsyvqoq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lxmzavqh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vkzidpwx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pcrdyryy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cfmqkxuf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cuisdpvc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2damvppsh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mhhhqdys.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fkibffji.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2blmfqasu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ewjqeusi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ptapnpko.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mzyyhspx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2aazrlkst.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zelzncvf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2osqhysyj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rervwsbz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dhysszmf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fxtsoqnf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2acfjludo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vhhjjyoo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gwxxacdn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2avbsmpnv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ybowryux.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hyzpiurb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xmekyoso.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pcpiuzla.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bqhlmmfa.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bdhcizgy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kgpaqgiv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fujdeuyl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ajjimznj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rwezzfex.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kbgowbis.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kmjqwnpa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ijwbnbuy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wdtzbudh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2quodtgyz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sondrzan.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yrwjzswe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fmyfexmv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2osdvxurc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iblhpbpa.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bdzbgvfo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cxscxukj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wrdezmcl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vikgntof.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lnqfsvwa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mweakfwb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rxtutdti.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2spyijotx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ahucdchs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2huzmjftf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yfzwopbs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pibhpynh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dychqgee.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cfhkguwj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2yqjagzyi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pxyegbuv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2odlzdtnf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pqkoxvus.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qfjhthrv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2kcicsrdx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2eogvqlzf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fbgoxgqu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2hcnroxmz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bigykgzn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zwlrlqvk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnlsnrga.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fuqlskmc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nqpvwckg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jochvvau.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iiufukrh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ppqypfcd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zvqgavhh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zrqqinvn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vbenwsgv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bsyefnhj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2owsfhxqe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdbxklff.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kybpbtsc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kgftyuzj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2iltxdlag.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fsamyojq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2dgcqqscl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tyhkoeom.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xlcjnxfv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2unppwmrm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xfhfbmuz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tdvptkhp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2faloyklv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrffcepr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rtfjptiq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mbizqnpt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nimpxbkp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tttivcfg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2laumddaw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pmkcdsnd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ozrovupw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jthcstet.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aenlvuhg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2euroojbq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2aifyetqz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rnlsekka.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2epaensrl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2frqcxcbr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jmiiojqz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2znlcrypm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zhbknxzu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2temscvxg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2txojjfvi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dlwkfobt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2scvmkafo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2opwiisyi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wpetetbx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jnlsziap.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vuaajvfj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dalsdcvb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mtpykqou.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gobgpqpn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xlpjcymg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ncczchej.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mlvjuhai.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbodttx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uyvxdovn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2spdzkjfw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yzsivjfw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2njurdoft.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2cahwenmv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ndibyvos.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2idzrczqd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pplnodcw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2liljvsgd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjzjtecv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qltryuxy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzdjluvz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2kkorhyfx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nmnhniib.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2favgusmp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2anbvfywz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pkczqpaz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yqxeodpd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iaepqedt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2surqmslu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2izlmdshx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dckrurxx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ndsnvfwv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2aflitqxt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2exuvagwz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wrnnzggn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hrakcfxh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2irwbbjtc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fakxuwft.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mllaquwt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qaxcrfxw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iqkeween.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwupzwtd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vrcwlimo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovuwltfr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2isxtonjy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yehmvwas.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwkherik.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qvyudmxr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gjtgnjas.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2psymhvyu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vovxehzo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qpqclahv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zrvjwlkt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vcrgdluz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ecoetbfp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tabcyugj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecbsyqao.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zzwgumjw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2phbbevdm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2otmablkx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xeujmdql.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrydryck.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nbwtggih.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mzojvder.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2undcypcu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qyogkhzr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2szecwxet.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rapgmlbt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rxacqvwd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dyazavbn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ratasqdn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjhzfgki.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tvlqxsmy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qwpkrugk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pmaqhkql.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eorkrqao.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ietyewue.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hufndtwp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dnkjzpfd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wwxfpxpv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ubquyige.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hzkkuzmm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nfblbwpc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsemjotr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwbkeuhi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jhtbivyz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2npsbuffq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nlvfwezd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2soykckfg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpcfuwga.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npszwpqp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zfpufxft.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eylwsung.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urlgkmyr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kmmionqv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yhipwoxa.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnjsjzcd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tykaajbq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gyrfgfaw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iykrvkbh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tcghxthg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hqbvqlgi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mutlaasg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2blvvalyk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2xnfrrsti.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2yiscvkyg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2nukxqnke.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kackuynz.html


<!-- 参考信息 -->