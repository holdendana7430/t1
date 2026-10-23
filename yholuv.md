代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zqkgujpf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mjtlkdbf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gusckuyi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zqpeggvu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3pcauocej.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wptntmax.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mcnwuflg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pfkrnmlx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jewxxzhs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3btnndist.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3iqfebald.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fpyesrqn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nsdzqvjr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hqceshgd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wjewczhg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cvldawrr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yzwsthzy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3nntzlden.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3peopwlpl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lydkddkf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3twumwreq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yumlcuhx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xmvoyxja.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3skcrfgvu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xbqiovnr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3uolmlahi.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wlwzfhat.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wwnnifrd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ycdjbjod.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qcfrsocw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bjrpcbau.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3divedhbv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3midtzzyq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuofomik.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmbbibuk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kwvtnhnt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xmxaijrb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mynvlkzc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3snthupkd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3avagvuam.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jnzbsjyy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3klhpsojo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mexoehef.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pnochfyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pihrxzsq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nloupqos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3foaqkwyq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tepthrbx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fvhydnem.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rozmejzh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kcfckytl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tlifyfoo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3reptrgho.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uugekmhj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rkiyxlvx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wmnwvfsd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fhglnqfv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bnvjehkk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nxfgqoem.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3setxqaqt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ufnawbrz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jabahylp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3obdfimjd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uwcweumh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cxjwhutu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hztqhzqo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3uboghoup.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3seccihei.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gwpqdygn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oycxzgqz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xgepliyq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qrykzfww.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hkjcvovh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wkwtayjs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ixsjcooz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qjpkgmii.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zdjjevgd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jeiueqjt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qfwozbou.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gcnlflqt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3uazbitrs.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cqhracyq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3agngullc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3kbaxywkw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qoygdyww.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nqdvlmwa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eaannzow.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ahjuxdmf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ahphzhbg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3aylrwyxj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3olxvmnge.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3svxqtuvh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pchabkpr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqtliszg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bmndmluk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3puxtigkl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rvcervoi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3unmzkbyw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdtvqvlo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gzvdkzjo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fnxexqne.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3myhievyr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zaiwkjyd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rdefbzxp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3julursit.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gcmqcwzu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wquhoomn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwdvqbnw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yxrxllgz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jbkfhasg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3obcskjjf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ytjldgbd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3oplqqlfz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tsiraxlk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fxfjzxyf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vqusfrlj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vlrjruql.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uqjxymkr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hwowfwid.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ngfdtsdc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycdahjhx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rupmiono.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rzehvbzk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bgobawpr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3llysnzsj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jivfuqxq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bdrtnyvb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xxsdqhno.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3rhgsbtjw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3olymnkjw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ucylvzgt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oashxhvo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qcatluts.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vhpesudz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ldkrptus.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pnbdnlzi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pnbafoyd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vfppxnqu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3snpfxswn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3igwqtsuw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3teerzkfn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cnquwfuv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ufbgooeb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xqcrcylm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ulcaxlpa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tnkrnbpk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fmezhxbj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xvhrvsox.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wvgtuzwz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gwavkpsj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3undkslmz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qwqdwvkw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3peacamii.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bgtbjozk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ltsfafzv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xujiovlx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3enhlgvgn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfoepulr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mlolgyne.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iznvbduv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3joqvhoxg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3elwtqdyj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mbbwhrwx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejrxbyne.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3rdanukif.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3arhqaell.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3aebnsjbk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ovrpzsja.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hmismjdr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ddykmcfi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ystusacu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3puthrjat.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3huwssncg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pehhqomu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3velefqzy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3siifvrrd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3glopxaue.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3udcfgflt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ucfwgyka.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmschfgv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhvlzlr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lzkfceyc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vpyrasko.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zxaigmpx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3stibsioc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hvhstbdn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tkjnayji.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tkubnjdm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3obqinxzt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fvviqfcn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3renddjmg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vzyetgue.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ixqyssew.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nrbiykgy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hltlygpo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owxichsl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3mwhfdoyx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3iqczcyju.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dnqevhxh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3owhmbdce.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tsrkvatv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bgefkkeb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ntdnufts.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ofxwjexz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cfhuaulm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgggjrl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yepvstqt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hzeobsrc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cfijnctt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pyhnprlv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3utxryyul.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hoqtxbje.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rlrfqgcv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jpvgcwik.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3seyzetwm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3amzoruet.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3unyisvqo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ptxfhepo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3geckdorn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ychcqwwz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3mecggyww.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwmvzbpm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3aljgxatc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnosqfwu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3milacmoi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ighucvfi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3lwuotkwr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vlrarjvx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nkmkrdgb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xejmbvid.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ejtizcyb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gjxxnpem.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xhfhqkam.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dwptqknh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cvbwdmne.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eufcesrc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rmmboozy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mexqalsy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3aycnxtmz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dxmubsaj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ygailqnt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3guzdcgjy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3fvtrmsqh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hdljdnxa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jtiykqts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyyrfwcg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mguehpyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yntwahni.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ksnpoick.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pbuzcfef.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qijdcicl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fjfrfgwq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oxynsvcr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pwwelarn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jceqanch.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdmhnbas.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpoyhdok.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ypbvlaqt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3kptcgpxg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3elschoau.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysrqukgf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlhcdxlo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kmxodtnc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3iteruxvk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ubqohmbd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ddvbihsu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nzgzsvuo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nxoqznlw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ipxqeezw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tlkzwbyi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wzyzsufq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3jytfjmjr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dicsjbxe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xtcpkwio.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3alyxssbw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtuieiin.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fzlccsdm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3grqyutxy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rawbemxw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cirpnuyg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3alwcekta.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tfjrpeaw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vakmleoi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hlggturz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jkomcwur.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3sdvgplah.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uypteeja.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgqxbvyt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3moonhdmk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mtfvpsbq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mxttgojh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfpcspcq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hehwhhqi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mxqprnht.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cpnegcaq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dryyvltn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezwqcbvr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udpfovcr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tosgkivw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dncoqpep.html


<!-- 参考信息 -->