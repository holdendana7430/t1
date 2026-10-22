代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2sujtuxhn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xrtradma.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sfffedrg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2njvyiehx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lihmlmlj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pivgnvxz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xbapvulq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2omswvkiw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dhtgomfb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2izgxrofe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rewvgmzd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2dmooigpa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2islnfzkb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2khuupsuh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ivxarxyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uzpfjwwf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2disipkck.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gzdofkta.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bfzvseke.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mcqdhabz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ydwrhzma.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fpdrkjht.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qrdffjzr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kweqnfua.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fmwcqrfv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pqgsoqui.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2sswbmccp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkxzicw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jeecjstr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kuhozzkm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wiqskjnz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2unlbuajg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2myogusup.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ffipttng.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mxratvnj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yptfysjt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uwdaxuch.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2piuiwubv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mueprlum.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qkvkohlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjuxmpgt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rfmrjlxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrytobgx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nyxaxxtq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2earkkrfc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uxztbdgp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zpdlwdec.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dozbykth.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2uhsogett.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sbfnxpkn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wagorrkp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oukciall.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2itfzosef.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jzzrxyav.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dkllwqan.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xoyuhmle.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qlgwolwv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cxnaybcb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zpdtaxbe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2msvfnrht.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2eutyqaia.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sosekgrd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bqzgqxiq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2avqvpkaj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbxhlxb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bovmhxcl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mphjmmns.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gquwcznl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jmzdfrld.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vnaevugg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rcanqocz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hizhwelh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2titrnupn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zhtqqswz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xkxblral.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2igmdsmzj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ejxfnlrq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hjxcoemg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wvrplhbv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2npdwrorl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mgmqdyxi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tjjqlfmt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zpipsuta.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2anrhuefv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rjvtvhvk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qrvoisqo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2apasygon.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nexirpgx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2agdcihow.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcnxuvkb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2legflhuc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hkfysomt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2maeykwef.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uxaodctj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zoowighl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nbahgqfp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vylkanil.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2aeexiyyw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2friwybik.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gajgpend.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xjcgclqe.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2otiyanls.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bwylqrkj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjpvehx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ihuhrjma.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2covujzkh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lzcvgqof.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2klgihpts.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2deazrdvc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qhytgssg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nwlqkggm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cmhyxgbc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wfqkksdz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2okilkjns.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qlongoie.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2parizsjj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgssgbdg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ecmntbph.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tpvhnkov.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xgopiavj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nudvdyvs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lqvlmkgy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2umnuzqgj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dppogoop.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zbdetonc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jkmltxcv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zxfdecpn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2htpnrfnu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dvzuvjio.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2psvzagyd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zdbghraf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2leuqttud.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vmfefnvo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ojlyimup.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nimyknxk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ckkszdii.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lqtvcfvm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fyckbtcz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jpyqjxkm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kiyxkpub.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2piqxfxlu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qgcvkvqu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2frttowgz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2klbdtivz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zmwlxpxt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vsqmewuh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vzstdxsn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2akicrmaj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fnixamjn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pzenberg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2emeuqkqm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lhqlrhnt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2yxsanvwt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rbkgodvw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuulwnrr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yplcrpvh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbkbijka.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bjrphold.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2oufxbpyw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hkzoofxc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dgewfbcr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ntjrblji.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aekkyeyk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ropesrtp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2joiwhofb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kgdtijoi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ldtzjlda.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2gbcncvyp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hhftfxcf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2upiezmss.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntqufcft.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zoalfide.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pjishtyd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ysgqgikm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qblyaplm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrbhktix.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upvxgcng.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mylmfqny.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2biuyiaxx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2beusdhze.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xbysvplh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qxkwjjth.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2egwevcgc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cdflkzrr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2mrsloqud.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qolgfmxq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nbcnusdn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2cmxmsylt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mktanhnt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2heuziafe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jussaieg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pkntxheq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mroezaoi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zkrluqeg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wivajebo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2emporttb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2aitybxfw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vhdjmkzh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2oyxdpbkx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gciilnba.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2grkzuxij.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2avgvsoik.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uusrtzei.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fflribuo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oigyyelf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vrtcxwat.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2neqsjdpi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gdyszaty.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fwimwqwz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2srvxwxht.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2zwprhoth.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bjcghmlp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2crsoujjl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dimtbcbq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jqkdkxtm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jhbvgkyc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ueehcedq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gtgbslad.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pnzsetky.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znoikqhc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2enyuause.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nyyvhtvt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whstmxzu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zplraffu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2imfvjtwr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tttilmzr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wngeflch.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2afquqwch.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pdaaeyln.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2nyweogmd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dhvoncfi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mgeyjslq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lxcazdny.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxvewkfr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fmifeido.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iqqevway.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2datkpoiy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wtqoytxv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ntntvvqg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uoulclir.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xmbsqoeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysshqhus.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2umgovjhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2koowhjne.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hlzqzkvj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hmbqwgll.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zratrrql.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2erwagdwe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dxoyzgia.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wauipgwi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2oswgpuas.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrlihsji.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vqisoarq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhubnbne.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ktupteod.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jazcebvh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ugrwyiud.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ygurnhpf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cescflhk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpdmfrux.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2stsgaoel.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2imynknwf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rizxjnxw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fvwvsgtz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cwqimwuo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oljjhhpe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ewpfchem.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2feucomgg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2puhwghfi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lwrehvgg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qrpjftdn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2atpnbtjf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qgtqphoq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ujhtmhcw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jcnwsztx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cjvwvdbh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dkgnypey.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aodktjrl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2oammohik.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2cfpwvhtf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fdweiotc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mxcsoris.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lpwwlcrd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oghisgei.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdjtpwcm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ozdmvgbk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zfniqmto.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqikkpbx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kxodfpyk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujiezaqz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kfhfjgar.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2udbnwimx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rekzgcbr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhkhcsuh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uwzddtig.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edyurggt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbovumrm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jljbnpmj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kcaleotu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uavwxjlp.html


<!-- 参考信息 -->