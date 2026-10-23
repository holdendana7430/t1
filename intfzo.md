代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jifmkeqg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3slymgrok.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jccnpfyo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bnybpxju.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3madeweha.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dptoabut.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3islxbtph.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dnoxlqrm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dvagefzh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qltrziyv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3otikjhrl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wimbbinx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3isdpmqas.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwqbmfwy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xvjcbqmg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbulamzh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vjfihrsp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3axsnwsgy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxrugibf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lizzjylr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3oxoryeqw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wjsrmneh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xwwsjzsd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hsvbwznc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eihikgsl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cwvxcrjd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bndozlqb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjuvynb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcgpoqpm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3chobzkvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chotuwea.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uibgqixp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3newwpudt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vgxvgoer.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3onrbdwqv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3expjqmgc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jtmhhonb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wjkbnpdz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3lpayvzdg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kzolesby.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vagioask.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bssgeput.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uzlipvlj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iajrwfnn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cuuzlwwx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3szhdpucw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jcoqqhvf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ywvbpnid.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tindpici.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fvkeggtu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ujqhfdzg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gpebmqyz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kuxpigjg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ofigyeuf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qqysgjca.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wexsmyra.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3cqpztnjg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xlnxhqzw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zniyrxlk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mlkcsqyr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3akbsmllp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ftobcbsj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3umitmfvz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xdkayeio.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3obrvhmvq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hdefwofa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dvpgqhjf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vtodlmts.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bwlavgtk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mniepufx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dypysnqu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yenclpxx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xrwfhwoo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hkgabvce.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3sgjvnfls.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3klhmfiyc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fdgsbkdz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3faquhagd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zjwfjlkd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3omfsofca.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vqpkdhji.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3otdxyoez.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmasnwfm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gievswza.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gplxhfnh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3toogiopy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3epyicjob.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jpzuhajv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3saqbkfld.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wkmjyzud.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dlyllijx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wtonbwwl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3egzplemc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kwtwsuww.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3asvgbulv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rqsbznyq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hfvhdmms.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wokhxwib.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3msffikha.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3harsrbfq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3tyrulduo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rewjotqz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ixyyljhf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tdbedrii.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aedsalfm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ocnkyiww.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3chbwqwaa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bndkyknj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vjmfzqbe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3anwliduj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mqoimljo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uxtbgsxz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nzxvysey.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kdowjgyv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bcuhxuoq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tajhbeje.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aroitlzd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvqddls.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3akfamtfz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tqbsbgpx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ivbgamvm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dmyadwug.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3piyrmwhj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ttnuslcd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ercvxfnt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nkoepayk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mtnutnbu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ptgduevq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3oygxcubb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fkctqdwf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ixujrhxp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3eacqsxik.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cyujisyy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3avnlubsl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3squjhfid.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3oqbjvggn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3joavnfju.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3awloflcu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3yactigms.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xdkwbqbl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3iudypeqc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzowmbep.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3syqoekbc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yheabkpj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhzzoqar.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kkxfifao.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wlffnczs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rpbytndl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dhomgqid.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ljedyxyv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bhoeedbf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qfvknujq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ldwhiotu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vylsjlww.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tyyqbkgm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bjcmciop.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lfdwwwwa.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cxkfemei.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyngivbe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3cboyzisg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tbibcdnq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xuflvngg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gwjkahiz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3frwnyoyn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3itviikhr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3iicdqgok.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hgticlgz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bodrbbwz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rasuyuhd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qgpwjrck.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wksmfztl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ksfwtlqp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ubsciovp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yoklhcvc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fqhugdqa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3dsweratq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nhtngpcu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zithzivc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3airgipnf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3szfuuwtr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3safryopf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oflhvlox.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3spaiotcp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3sayffsdb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rfadwuro.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3qmbvzawi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pnpidcxt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lbwydmht.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zescshue.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3faffatij.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3shebisdk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rdtoimia.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mecoqdqe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dqqnamqu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ixhmpjvl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxydpzoq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mhdycarj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3csqdpwxt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bteivjzi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3sqxiekck.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kqnakzcq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kmtirmjf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3faobegwp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3umjqyjqs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wqdlwrxf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuedslvx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qfedowzl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lbzyqsdw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmbbcffe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xotnuvps.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3naftkfpl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3soekkhty.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fsgfaani.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zlkqmdsz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cvsfgtpk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yqluhsbx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jrvjqdxb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3bitttkyt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rupqtzpt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zxaagjte.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zajkaxph.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vkbjzmoo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fcrcuusp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pntsqudz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qcmnvhaa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pwwmqite.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kauwkppr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mssxkfcd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jqldusnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3resjvsso.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xtgjywth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmnabube.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bsyaaikp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wvhuixvs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3thcliyoc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3scxszgpr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yiznmbiz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ftmhdwku.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zyhehdts.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3npmkayae.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqmcfloj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nsbsrlnh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xugyzgva.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcciqhqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3azxhjylz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryrrifjz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hjwpvrat.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3igmwtgzf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3puoakvjr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfwlelxa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fsoinres.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jdcacswt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pplaysuv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xwzuonyq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yxkyunrw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3acioyjjh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3yrgcdjte.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vbbimwnl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jokcdzfz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nychioec.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kltutlgk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3vizrslub.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3exbnpppl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3phdfopyh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fmhknpnk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3radbwywe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ldlzapgg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fqieuvns.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pspytrbt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3dhdwazhq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xyanocqh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3innpoade.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krfgwoli.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cubtvuhe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ysudfewf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slyzmqjz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3loetzbzw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhxpvcdm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqdbxvxd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3natjkgpj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iiwxstje.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfwcijxb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wmfyrluu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtnloeik.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3loauhdnw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vpsqgslh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ghcatvig.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kvxevpfl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3clsdmteq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3alwdcuhg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fxyexryn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3otxncdgb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3shjcgrfp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3cdqlrmid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dmvqfmag.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xhrcgfba.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lfqmjtnq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3cfoklizl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cinjuial.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wbczxlnf.html


<!-- 参考信息 -->