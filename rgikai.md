代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lqzjbjzi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2kldmjrot.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jxrgzyzt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hyjdmocj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2afszkfiw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2agnnsxcy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eswckcqq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2nbvvxzui.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tbsjeupy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fyswnbos.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tylvsvdj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ymxknijn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vvxgaeea.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zskijiho.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bdkrxmdd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fubxszam.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ziroldtr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fpzvvipg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmcynwi.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2uoissziy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ffrmwdzc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wutskrvk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yxdgccbq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lcomfrns.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qynjnptk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2osueuele.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jjkfukhu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dcbgahsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkvqqynm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qcgphqic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgvznget.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usjcongu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qejeoksi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fxdneszk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mavkfhnm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wxnxijor.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wefjliku.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xxinvscq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wpdkyika.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2loxpdgpf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uerdleml.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ifkwrshk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xbexjldo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cscsfilk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xgdncrri.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mfoarsyy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gjfwonnq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2clqhiujz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sqfnwkgu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tqnqijfd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bfixjoip.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nqucqhgs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vcwdoivq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tsvtwkwf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2raclttgi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jkszvgoh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mxcqsnnf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jqjglyrx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jfbmvdji.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2llwjhlxo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ybkcyzqc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sfdojjbh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2omzwfize.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2edczsklq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bwaxmlyu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hxpuzcfe.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tairgmce.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gadganpm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rgseryyv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zfezweck.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bctkueyd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nisrqxnm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uhembgvm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2oythdwwl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2egniodfs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xjbldizz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cgnekcnt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mwpjrxbh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfkdtyqn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2elymlbcw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ojycvpwk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2axhcwvbh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2koivkxdj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aldykgzt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jmmhvtmh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2slftikhv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jswzcbfe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mteiotyp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dgsbyoth.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tcivyiys.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gifaimeu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2lsjxhybn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kpjbqvon.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fkpztile.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ckxhginb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qokepuog.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vovbacgt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2brubkjbr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zrfgwhiv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jbankhie.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gzguhnxw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vbfuftoh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gyptxlzz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2pfkckgte.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dprockby.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2njjdvobi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gwyzunpb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zcshhose.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2odxjomkp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vfkmvadb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bsvzfhon.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dhjgokgv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ewmtiylf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bquqwbzi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ixvpevcb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aoamecyw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nmqgmelh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2smyqkpjc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dyeynmnj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ybssqvfw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2voukekvd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rcbuzqfe.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2elyfzpyy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yazvdywf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gbyxatsv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2saledcds.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2earcwpzm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kagyeyxo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jsmksman.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2aphrnotz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wbuqcoyh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ahiddbhn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2osvpsjec.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkcdzlyq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ceprkzvw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mobzuucx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2liuhkojr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xciksjlt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bukvsfyv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lonxtllg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tsmjmehb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2aebmclmc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfkksjun.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouwrtoog.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjvpejpb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2snlxsoxw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tuedgjhy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fmjovgcc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pmiycipe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nwqfluzf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cetupakb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bictsfzn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oomkihig.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zureqkcp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2shjhisbt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2smtsnnoe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jnuxqmgw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vuhtsgnu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jzajpurq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cvzgzxke.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqmlopdm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2stewwlqs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dvhhdnqs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2atxhbnpy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mthpggur.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rvqerxzf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fnugmgxi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijzmduic.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jxikfvwy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zfvmmtvb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2iladiabw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhupgjs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2asvajpem.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yqsdbffx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xkjvydmd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dwwzrjhd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bautzgqa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xygzdusr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wlxsqity.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2twpvusvj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjhwjade.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lfscimmb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bemnmffo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2npjgxrkh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qeiqjikq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jgvsuuhn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rwxvbdvq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ltzrkxxu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jekjqbwr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mkfjsidm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nvpqtewh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fbkigfuv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2eonxpkka.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hlinrekz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2osksdblh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqeovmqf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zxobgtph.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mdhgfrdg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zcdqtoke.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pplirumt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hnecmjhx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2znjgfvtw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tzqbggne.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zudkbnag.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pfcplccc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gexepsjt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2sygbvhtx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcahdubv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvvjjvmh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bpphspkx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2phikxtvp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zgkdlbkx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zoebikok.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ihtvghvk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tsfmngjh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2czcwhded.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ljbslkby.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bhktkcql.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vksmqbxf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lwdrltzn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2havzwdha.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2orbxbmra.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ejsifpba.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2irbxmnls.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ozgxabon.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eqsnpuil.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2jrlwvvsv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hyviepxt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wbwmxeha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clubcjth.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2umfvgiag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmaolxcz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2puyprgbe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pyuseuab.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2swaqogxb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ctmvgqya.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lvohawxq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ngpfavcr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vomvqmil.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfqmrrub.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iznranfi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2orxiotfu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2sjwsvuhn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tvhfpnyl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcudojft.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grvhmyms.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ohjzritw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dtrtknvd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gbupmipf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jjjutgil.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2weqqlnex.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lfhqpuyr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iyouyujy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vxttzyqq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2degzgwmg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kbfrkpgb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zxmfljcm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ehtfkbzl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rmvbjtyy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lhxxpxyr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2utpqxyuh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tiywxoum.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rrmdbzpm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bdvhyyjm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dwjucnrf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bxcgwidb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yatohrpg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2hvcigees.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ehfqzjko.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2oqzufxin.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qopscpfw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqugccvf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2crjxtfej.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vwipwkkw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wirgjrtl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2awuegvve.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgzognqi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpwnipxs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmtcxswn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2apezunpo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2areophqt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyjdhvyn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2huhydknp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnnfeesj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcvrxeuz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gixogfnl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pxgzstyp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gftmsepq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mnsknwzz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2anxrvhml.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2owmaezsk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2iyohbrbc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tlarnveq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pryoudec.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ugqrtkxe.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2eaygzumn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yayxbthi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dlqqhtua.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xrdharkl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jwgunjld.html


<!-- 参考信息 -->