代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ghkyxjmc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hbrjgytz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3aqnhokfg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rgzfxsjr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qjdnglic.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dmaiiial.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cmfwneex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3crbzxwyp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sehfjrcy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3qgczizkl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jhjzyspx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gobpfdnt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fcgcqgyo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ijyrqrlt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rqdbyprt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uhxultrl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lrrdqast.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mmvrwipl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mqipcqbl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3gftyhule.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zjwzyand.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3iuosgmls.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kuomwgmt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pgvmjvmg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3exibfdjb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ydzywcpk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ljplmcoe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lxrzpkyc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3niposdik.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3swygsouv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytbiwicq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pkjglczg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fszslilr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hthpiyxo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dlzppupa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3djcxqpmw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qiduhaqt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3avxlocpo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ufdoqqqw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hyjbwxoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbvlyexp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3aqokytfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jorxtadr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sjrvbixv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fgotvusz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pzntsbvf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lfluwnmj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fstrfaxr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3pifvubrp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mtyuynqh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qvkxthda.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lrhyrodc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3loijlhte.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ghjzvoyk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xfqdobgz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3laqcqnag.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pslforih.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzbjkqed.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jgrstswo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dijfwyjd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ecueihbo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3aircvuli.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3dlpxnshk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eaofydcs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ymwnlxuv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ukzozoet.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yfrbnlgw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3okshpwdd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yixfzlen.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkvnjpeu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wvpmnswn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3toqwfiaf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xxbrftem.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wauohpsr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ifltjxcl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rlclridv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xxrprsez.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qqepxktx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mibxymvo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ujtdldwi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ryipooqh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wckwwovb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rjyluijz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3srolopzz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uvtycspp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fnrumzbx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mjelgwrx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xuyxqaju.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xpqeibgl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3skhnwssj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3znoknyeq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mamaldno.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdhfzyos.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fpbkvson.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jivcoacg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zobdadxb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3okabznvl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dzakvwny.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ekemglvr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cnvibjcb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ipeafsbr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gevhmvbs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3djnwdouj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tbzipgqs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3iihnwzqs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3snuitxsm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ugsuxiqx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tmmkpdnr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qvglrrhu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gqggnyfv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3plmhgztp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3iypunken.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3yskqqgok.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cqozjnhr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gageerdn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vttopulv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ilopkecd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ydsvnprc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3psqkzept.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yuuzjjtt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qzmjmqzw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uxyxrniw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pdyurooh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wzbtbakm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3magjrwbn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bytqpdpa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vfwxlqml.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ompweqzu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xbntfpqd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rxknfjib.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3refegwgq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ahljryzs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qpowired.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ycwzmssf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3doagtvbn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iomijduw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uaylvhhc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3maqewqxy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ljzhlfqc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3diowhibl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vqzwjrfe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qjdriath.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yddozuhu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ktevkuer.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qeteudis.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3axldwjtg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kmwmnqbz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nucmdgcn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zlsjyfba.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qyceaigd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3obdibdcz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gilmarmt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3dpnunxsv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3trbiuejj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkjmtrod.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3suaanxqx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dxxnyjqy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kgvtebpm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3sgkejhkw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kbdzoasq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3zslzdjlu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hetoeogn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxjqjzpe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3rylvlssi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzzihmsj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eyvuscqq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ytitejrs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jjwzosut.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nvrcuunf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3knyyrajv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ustkntyu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qtihycov.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hbyjmrgt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aldivpsp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3riqdyrcc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3aontzluy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lckawwyz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mxyowcys.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zsxwdqpg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3klsxknzm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xmguawkr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3snvzlebz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jcqlarnv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kjnqgoqt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qywamobi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bthhzfpe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gztteenm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3emwatqcw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zfhhoqos.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fzcvffzl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lsmkkmpb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3aesrznjw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jwosnpqm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3khkbnfqn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3eovnugxt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yjjnfcvs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dpwvdser.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kaaxdcfb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rwcuytnz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rieysoyb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gdfhmjic.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hxcufbhf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jsajqflt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bdhiffay.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vecznxio.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yzrqedzj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3flzzqmkg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mkybarpr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hskoifet.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aicmuzvu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3mwpbggws.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vdyoxpsu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ubdlbndo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gzhrubda.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xhfputaz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3exxxkptk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xuyzqfyy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wfgxqlpm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqkdsewq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vsgcdcsp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wfxmgjzu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3yrdajkkb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzevpkpm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3pufildkq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3iwkrddqy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mnxrgbtv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ejpfjkcn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ckbilnji.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dqrtvwob.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kyccwpwj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gbvekkvb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rntlaplw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fmgcmijf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fdirygjk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iycesocs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kdnweyhd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wslsonpv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hezyfiso.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3svlfalhf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tffjyjew.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zqvztxrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhoyqjot.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ozyyghdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sekwpqxy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3oilrccqk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3tsdasncy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3okqwlozg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ymhhchmm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pvjhnjdh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uwbbndtj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ozlazoqv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dpudpxan.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3akrtwhlp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3auqyhvsf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jarweqgp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xwzppbob.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndcrckgq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijvymezw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pheakiej.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3oxtqybcw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3eoarwtci.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqobdgsm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wxrjzzob.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bmpbdekz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ezlhprwh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yzdojnxt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iskraxar.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wlvtsilt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3btoyrkbc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bqcuilfp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3neojjjns.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvbrpyre.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qyhryvwz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xiwmsbag.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bktlhlbf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mjvmnkmm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hsxdjeoc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3estxhegw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3xffjmmoj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nkosgvhz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pvwderol.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vhhsrifs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rnhmzjnh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfuwnckp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndgvaxin.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gdyinxlp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kiqlynom.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgcnruls.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihdpninb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3aobapyrc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhbnuhcq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wjpudqzn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfdsqrjk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3skqlsnxh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3utnfahpa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sugxywvd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ueqquvgc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cqaadrje.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jhhcwsiq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lrahrbmu.html


<!-- 参考信息 -->