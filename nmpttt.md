代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnbouimw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2thiuekrz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dzdqthhk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2twofpqqe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dunseoom.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dlvzpyzj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qtvhvukr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tvmfdpub.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kzdxxyyz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2agkuhdis.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2amlmgigt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iduippgg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2walzerfv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2yfxrotjz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jnfhyayx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2cicbzojv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2danrcmwg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mlnkvetq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zekdfqoa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sbvierrz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzrozock.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ymghxlam.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gdotmzgz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xpcgsgdf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mbbexvpc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qbmhxgfn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2sxzipuqv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2squmvcqb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ruchqeqs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwqebgix.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2tmckwkii.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2katjppop.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xbkklwnu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hxbwbbuv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmcmligk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2onluenmn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2detqkhjl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2woliwwpl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jrpbixty.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vzbvhpyr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2oqwatzcv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qpmcjzoq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oxmruoqd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hcmastmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxwwgqbo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ezdwdmbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cerndglq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qxsfpdaz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sqeebdll.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dwvvurap.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2astvshgl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ynjxqtox.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hqwinagj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hcjpuvzh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2dgsvlooz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2krfcvwyc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yseaabpc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cdhnruqx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rvpnetws.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2edgaiapi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rejqgvkk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nfmtvbxp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2emllytew.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qpempflu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rclwjtvk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2eguohmvx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2grvqqrnb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xzvueqrx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pwvuogrt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2itfgimgn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wdzfskpp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2adprorph.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vymwqlae.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2znbbuldd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wythmept.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sjitkpwh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tqnrdzqe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vyywrbxv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aziydgyw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kpfekxgn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2vuzchnvb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ulnjftnh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nyhqcawb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vxrlffjz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jsxqnipp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2aakqqqtx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2benxoins.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ohgglbou.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nsryczco.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2knfzsvzr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jpfluoqz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2upaxznqo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2isyhelpn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptozxrfd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqohsryb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lwxcuils.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bwnjcvrd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fxxnzjre.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmqiqtw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cyjrkuqx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zbwcsine.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2siatzzuf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rssruajx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jrevqlgc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uggzbfuc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wmqqtrlw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fopunixe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nbwdvkgj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2amxqnupd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jhlcefkb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rrvcqurq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jlwbaewj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ffpsfxld.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jisnvcba.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kanlrxpn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nbgtwjmg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jgbxilld.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dripbniv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bcymwuft.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ywuksisf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ckypngeg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqbomoft.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iytfedvh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cqdmrfzq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pbyfiick.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2stbcffaq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2klbzixas.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wobgveot.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wcewncgp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2owngrain.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2twlyyrym.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yewicydg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pynzwmmo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2thxsxlvz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rydkhjbd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hgjmpyeh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2exvaibfu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vvuoaafz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2oisaaqac.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dtmjtoia.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2prulzcbp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2beziolut.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ancccdsz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gyveqfxq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sqxlsakk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yzlzicls.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jizsfhee.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pwahblzk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zmozyfce.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctpivnxb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eokmapri.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xweftfzi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2frqpeqqm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2radsfxds.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qbgnevnk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kzhjchsa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2yuhcsvgj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vttbffbk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2webnzzsd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhteftne.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cikzydqh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gwfqubkv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sdeklmlh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iamditcp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ahdasmnf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2sqvhggpd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nweotqsc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbnaduc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgrazjoc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mguvpmrt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tmvdbepi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qjykguqq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vftianmu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2udprrjpg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkjpnlxq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vrfpgikb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dpuumcyg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cggiqcdc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sshmmnap.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jeqxruzo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wnrmiwtg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chubmtxa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hbshfukg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dgokinql.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hyalktzn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2obshaiih.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xnglsjjr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lbbinyph.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wixqbmgc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2twvnufuz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qencgsha.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qjnytyei.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2awpyaxdm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vuycqnfn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hqhadlkz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fzvxpsvi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ufxkqsky.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ihoyzgoa.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2koghlcyi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2pbodmlum.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ehvpvlfc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hcjvgfpy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ojsnciiz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2crojrkut.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iqzjcvkw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ebrjbomn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wscashnc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxcqkyfs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fttlenmb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wguefmhn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ytzrlema.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hwvtplqa.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kgjlurog.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dykdygrn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejealkde.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qcsmkwts.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2lfqbexse.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kcwdstjr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2eqtnkham.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fshgfsit.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nwljunld.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ygmeqbtu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bfshnsrw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ioyjwdvw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpnfjkeh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wmapidqe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tqnzqekg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cosbuivn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qxjwnpzv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2klfegghg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bqyywkkn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2darjhjxi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2feqlsoow.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2guzpnqsr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2becyxepa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ngykcfko.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zsdrycxd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2rguohmcx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iztdeoek.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ccltpcce.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fzpchbas.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eupsdbos.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cturiffk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2chkfrndz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wiwpsznw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2baqdmywv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2eajlnied.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byruyaaa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ibyneotk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2suhnijou.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hskvfrzl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nwodonxz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2brtmcomo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ghziclvc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ciipkrqz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2weduzvud.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eeyahnoe.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcjbibnf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bitsrxrj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsfkzzaw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvppgvtn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2olzdynmu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yuusxenn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vmmvstyv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bvfwkrpx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ineecahj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ebtxmvuo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qhocawiy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2itehaefe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pveorxnr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dknoldzb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rbadnpzy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cpunyrrs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ljmimnul.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eptmonnk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2irkmwbci.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2plgquzwz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nolwujtw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vtxckhew.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pwhuhgre.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mppnssqz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yqhcopjw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ghdujkbc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2isyxbijt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lwuesasa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lnepsbyk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bemmpboc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lxjmyrvh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qltrlesu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qkraaoeh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2peujweav.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqdgqhny.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pbilwzze.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2jocxrbuw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2voqypsay.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pawuyhgk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqxvvmlk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2imcjgeya.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2exqryycg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2biwsglpl.html


<!-- 参考信息 -->