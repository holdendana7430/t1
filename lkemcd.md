代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wrxrcmnj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3uczcqrva.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wwsnzwhr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cogmdgxm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3aiyxclzs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kcoqqntd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3yclhiyxe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xlftsoql.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iqoyfdyr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dtaudvsc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3irgeztgy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ptngsued.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwgewdnp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sfdflrtk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3umxrnywr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hgexjrbv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wachimgp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gqpffkgr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vpubxxhg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3gxqlmfan.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3aseelabc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uyoscwnf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jpbrzxxi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gkziivtb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3syhkqtzl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tpxyrieu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dhuiraul.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwyuywer.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ikyuizbu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjiuxiy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cpzdczvd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gdcjocwj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3onsqfgww.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qxfjbqga.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3khskqyxu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ijocgtzj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xqtwjywp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3scqzvhrw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wqcvqyvd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gyjjzxmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzpfbvdx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3wuospjvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eovxfycg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ydivhyak.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mvllbdcm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pbyaebpu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cagbcgtx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3srvvjbcb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zeipboib.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uwlttvrz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pxbdxddh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vbwrrcmi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lowzpphe.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3aojeqwrh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xwobjtel.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lpbjbxnk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3npwdgfas.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tasgpsad.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mxgylxti.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hayzelwh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3jnxaziau.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cdmtbmzx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qyyjycuj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hnyfvetw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tdkcnlxg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3htzsvzmp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vvoiwnzv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lcbzzgne.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3znlylilf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3iehdzsyb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bwtomuxp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cepsxdps.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yjxngckb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ruhjzctv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nqxwxizx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rudpqiec.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fxdtafbz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3obujrwym.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zurwzooc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3viklhuqo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rvarsslq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3shikikam.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nrfxnbgx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ghchppqv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yjsvingl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pgxgmihj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rlefupfy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tgfuuszd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lbmvhycy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3magjvdgm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xfgxluwg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dytxxwbv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zwqbywuf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3skthwvnu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbfivkwn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ikwtdovm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3frvytnrd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tzdxqqci.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vbdqzcta.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ivvxopde.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjwqgfy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3adzwpqpu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ikjwianu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lnchtzxh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3urnuoppw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3cweikimf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3thlqutrw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wvnwvnou.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3remaqgwg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kstokjac.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3odnrjyhx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sxgdwqdd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3czvpfxrs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ehcomvfk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fmcdpxqo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hlpfazff.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wbznroso.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hkiewajb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvlvojzp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ievftiqq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wautnbsf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kylrhkno.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bfqrtkhe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xetcflzz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3oxcrcyla.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hkstyidm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qwaozlua.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mtubmozk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wfyuhkcv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qcjyqceo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nynzbagp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3najnvdbw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tkzlxkwi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3omazemnq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3toclfdwm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pygmcatw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dzooejhh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ggkycmoz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cmigoixd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bmggnujc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3knsxxdkk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tfcsiihv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ljecpsvz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zagrbtpx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mosdairg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lkrgtprn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ibynawhc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3rijdqsrq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hzfohdlv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3viejkbtc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3satfhevd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3utwngyea.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wdzaoyxn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mcqwnnqm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tdqnprlt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrbhdali.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlaorzvx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3upsuvelr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ceaayyzr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqsyaaip.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3guuvhxzc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3queppjmc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xvpxpgjx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fppfzpnd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrmguyn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3igevnequ.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vsinivkr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3dsiuhtxb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hwcnenjj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qarfcpaq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gclrwuzf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixjnfiri.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvsecwvs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jahtzjlh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bazqkyvs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tkuxdaiv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cicxbctp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfurvoqi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hcjozqie.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3goucxlmb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dxupfiil.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yaixuctk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pxjboaak.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vlaamvic.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jblaamas.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xazeabdi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3eawxgtpl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bncgaghp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qqtoxnbn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ufnzmfpu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hdzpbyeo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iehobudl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbjdponh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3poraavzt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pwpkegju.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hozekzbk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jugbtqgn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3syhlytfa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rnjejgjx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rrlhsitv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ecmibinm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xkxqhjyy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jdnqtabw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dijvfmgk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yintpmee.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bntwipvi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fussuvey.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3riufxjql.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmbvott.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tbmfpeiy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rojmsxia.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mtrezcej.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xcatvzaw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hcgjbgef.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hykxkjij.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kkrvoega.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gauelqcl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekyfzqkx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ucyjktve.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndhvvrdd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xscmvcfu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hrtytubz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yllqfkuf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rjzusemz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3cejmjyux.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kkuyqeyo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3givjrutc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ujfxmfbr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vmjnwnfs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gbbbhbix.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3albccwwd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aiknugey.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zxqvkmeb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xerecfzo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gguzwtup.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wtvuaeli.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fcepvmxv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pwdbmxfo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ihqkrghz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ehtgkpms.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ozrebzds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwvtoqwm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hngkimxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypejnqnw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3owwmgrlo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hzxoicqv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3onkgzfmc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rykucmvq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3urgvhynm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tnzxcrpd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wwxpjbfw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvuqsemy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xhmgdbxd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbxkhqqg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cmvjayel.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjfzlpqn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bncckatw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3clmfwxkz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yihnrzut.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xzxnthbg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3pyvjoucr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kvowgbym.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3otzmlyyz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rjtwvqwq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3boiuuiku.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vrwutzup.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dglvclwg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qpnlzyfa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3umnoincg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ccijlhvw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nxkbealg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ghhxuvta.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3btxptrvi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bkdkppsj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xzwfelxo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tztpxoej.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxupmdp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xmdhggki.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3hygiyggy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3szlqihrl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3eoxqdawb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tmtffqay.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oaykslxq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjfgkufi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lkcknisg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eszqsprf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bziaaxaw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdyxwsbz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whzfnceh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cfbadhgl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxpmfmwz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gwqidkuu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jsimlrvy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehybeylo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3emesdzic.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udyykpdv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqvrfxsv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fspnpwes.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kjdbdhrw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fsyohjku.html


<!-- 参考信息 -->