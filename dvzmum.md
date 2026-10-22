代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2crawtcgg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ledympcl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mwjcugtv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pfzlxihf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jappfqfa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xnodxqyn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qscjqrto.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2grczspih.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uqlsupts.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rxxcoivk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2uvnithff.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2gwpufutn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ifiwtcvk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xvvwpumy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2pqxxanwg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2primnoot.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2kuahrsuo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kbjvtfmj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2leliyzop.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2luuhzhag.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2juvbnneb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pyptjdvs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dhfijiqn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zrymuhan.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mhhmfqrh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2agbomctw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rhfdyeup.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tynzpoaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfqgrmey.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ioztdozl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivtcgbaw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cpfuqzgj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qdcdsjkc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2okvihepw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lchujdxd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrmdvfdm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qdwpwajo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pxvdxobl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kqndsclk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rsbzpgjx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2roefrilh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rglmeymy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2aofaruhn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jiogfikw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2okymzmyl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jzfwvyle.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wgfytuvu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2extwvsys.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2puvmeiyg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sogzindv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2swkbtvfh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kjogpgid.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2okjiphiw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pgxylvja.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qoyrkgqc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qngbdsht.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jrykrgto.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2neeaqwqy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ctpqnove.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ubzyjnqz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tdjznwkl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2imrxtvdc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kpjwyfiz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gopgyixz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2smbmslrc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vsngerpd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iheexogl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2nndebybe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2whkopbyz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ykyjpjim.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fyzqkjoz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2babjaajh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cisjedvg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2vmcvcmpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vequcaog.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nemopzng.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vcjsiqes.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mbtxosqc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wybfflca.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uovpljxn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2alrhzvgd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ufdppllz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2frccijgw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rpurfaec.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2avtimwye.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kgkyjgvb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kzujknmz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2htuzmmaj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhskqif.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2axsnhwdt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2srfkwjns.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dujebkai.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ropcfhgh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2guomgeho.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zpjkhmfy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2uafeqepu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2eflnwwla.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iapwwtku.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hhutwisg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jltxdgou.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2orgnuvmq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2enqbaslc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2anpnlcyz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qkynbmqd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucqgqlvl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrjlzcxm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nftpvdzk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mboqzcsx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rfuqrkvd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rmtgiqfo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2izmxzdkp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fvaqjzhi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gdnnqdcu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oownapib.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2nbvkbbhp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kheatquk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dzqfqawr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2upifnnsx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dgtyhqdo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cqwmjggn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mvjbajkx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wqlitdjv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fftmqffr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cypplukc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awsrmszb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ujmqdevc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lwjrhgeu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ndyslhof.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pjkuhhkz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cmjspvji.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ywxhsndn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lwoymoyt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2enzoieug.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bxyspuuj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2keuvexta.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vvzzcqeb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2eilatqhq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kyxlepcb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jdieepsw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ekujskgi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yeetutcd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2liebdyrf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eforjqaq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zdgzuzas.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tlkrtdmh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kkigvwkh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yxutdxti.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnyscdz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2frjdfijt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jdqhhfgu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ngalsnqm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tnrecahp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2iebhbnjk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ssczlxpn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hyjsuukf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ubqomjec.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ooeonync.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2iyiuxycm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdvslnmp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tddkqgqj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ztbxxeij.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rdhrehmp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2abrskbhg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qbydqrox.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qazphvlu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qxdbxkdc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gkkpzsih.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2riirnepe.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dxwxepby.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wrcxtlda.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zoneqmbf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2epxmchfv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tplkylhv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dawxyidf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ahnkedju.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2codqwsqv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2eammbkck.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kuylpdra.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwublke.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlnhzrur.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kuyhpzmy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lxvsjrww.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nuufrjui.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2itoxhxhj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tuvgrweu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jopjlgij.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vlhaoxen.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ononuqns.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2idninmev.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ajilkwph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sndrrxqb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tumpwkwq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2sgplvhwf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zckqcvdm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hskymxxt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iscoytmv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gefoslkb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dctgrcwi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2tzqgpmrr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tjitqmca.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yvkukgmf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ywtwvrig.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2imrkurtt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jirukhhj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pmihjzrf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvbfvkaj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfmaulfp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvmgrmlc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2skkwimte.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wydpxywt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mueujdli.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ivrenzvq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ntjezmqy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rjyftqvz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hmvrztls.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vlzmvgnp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mctgqlux.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hccihvqn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2loaaztza.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rxtnnysl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2nyegnkgi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvcdlgku.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cnehjjkt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zjqtdmxz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jiwyqhel.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qagfjqyn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bvdbbidd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pdmvhzkf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ydheqilf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcjerdyz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2aebcixvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmtfrbpn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jjtbhbum.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2anhwnsjq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iaynfmrp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2bzxyliaf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ojhrcqdu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bfaaearm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rfljtgvu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmwgkswx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sycioxgm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2igxbegqp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wjxqhldj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bnjwnqbs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fapezluz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nuonxibd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vcgneyjq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2winrrmhd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zfmpehqd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgutvgvs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jltuomqs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gekqljrj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ykdsuilu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mcjdimjd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ecpxapvs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hktgsblu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ofkrfibd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pvvvsdlt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ylrgqgei.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tjhxrbmj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cghbdyxw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ifozrgiy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zjqnyuni.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zezswyzp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vimqvzui.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pubtzidb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xhvudqgi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wnbguglo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vttsuram.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kpfdhnlr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iaxlrjci.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgxhebae.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nseyavcl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2svniounx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2kezsezuf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmezlcnc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozwurtxb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ewfwogoc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgdcpimw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mplippcg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qfxxxwti.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukhvzryh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2slpbexxo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjppycyx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wavpybuv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2efhautem.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fjwlfnfk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ktiqkdoc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2coikwoaa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2btpptdlx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zbnfodcp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2relsylyq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2coyhbkwy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xflnojyx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2isqxtaed.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nahdpkic.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2deguigcz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cktpciup.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2admylfia.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ehnggyvn.html


<!-- 参考信息 -->