代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ilzqqcyd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qpugmxpl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmjezmjx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bhgdjeqz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xwhcldno.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3tbflpvfg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pmirnpff.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3asadyuyb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3icyubgco.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cyztnnbv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gykuvcdi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jlcelejr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bzqhdfko.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tlowcdni.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gawdzmyg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3chketrlc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jovsaxtn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rppzfrrz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wgsgknqc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tqazkfws.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3pibraqer.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ugozukxj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uaswpwtv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xyiwjbrx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gidibtic.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lyiuzroa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fhnelgya.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lirwbwpg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lyqxvjku.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzyzrbfe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xlzvuunh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3awximrut.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nzbiecnt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3huxqhgzl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvvxfkww.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rjidzcap.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zbvxrluk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hbgktqzp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sbrzqext.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yaqtkwba.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rnzkesnb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bosfdgsq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gdltfact.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sfkbbytq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agccpmln.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hemopnit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iottlrop.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aoblgtwa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3psrorjlg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tzohomnj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zamblpww.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rdqjqzel.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjdhrezw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3eecaguki.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3lcmveyxl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3awzomscf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ztwtbxwh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oldacoau.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vmhdvapc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzbzbzn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tcbtxmmy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gqklazit.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kcbssyxi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dzpeleky.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hdypbdea.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bshxwhvs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3evbrscma.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mymbwrwc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3brhgdrvo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3skqquilp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pyyhbsoh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ilbwfrcx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zamuubuu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bsimmudw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jjzyghyy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ctebjlgi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3zdxsztmw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nqicaldf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tdtkcujk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ebmgikjh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3neuubvol.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jqolvvkj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3roglclsq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3oflkbtei.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ptcowuch.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jmtocvfg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jzlvakdf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wcpmmfxs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rkomwgcr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gstzlxdh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yqoaxvww.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rdiagaho.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3usurojga.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ueczgpzf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnceylkn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ktgnjtpg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nxykoroa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ehmyxnkm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3blifqksf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dcwzlprf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dadpxqes.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jojzlgoj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3iadkuujh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zavgvepb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3eikbjsdw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3rsrmvqyf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3rifcwgyq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oimbrpbd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3kbskkswb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rntdyfqb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3tgpjzzbg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ujoaicjm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qwxotwja.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3otmkuotm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xladhztb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xqjjkchu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mumsmqfo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nxccazfg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3perwnavg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tryebxvv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3iaxagjba.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3piurynbr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bewwhsij.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uggmepvh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3buoqpmty.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vcgojnjc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xovravif.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ktymzyax.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vgtenmzx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tzxxskit.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jjwlwbvx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yrsxojcm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qiibkkgw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3htxtuqub.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3alatpopo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lilowqob.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wcdoxrff.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3glseuxdx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3scirmdwk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sugxycrx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nydgwlme.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ujrecimz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3esgostay.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vhktpnif.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fgdhkxca.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kabcmsvt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wrrxnfjv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qwildwfn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3spzdwyzd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lwsiczqv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ragvrfjy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gxdzoasf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nzdngkfd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jhibreqw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ricxejav.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nygxnfif.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pspnozpu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3znatprse.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sayvmimg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxrfshop.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzwjydzk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pomeexjr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dkhaubwd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdnttbri.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3idexrncv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kgumluhl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vbthzfaj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gvsdwxkh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajkdyfpy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ptyhhsjq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jnchuxwy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jxxtfgmk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gchejyba.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3afyhqtpg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndkcuexo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jatzoyuz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3agsyiezn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bvgpwslg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3aimjwnof.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjyehzop.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yphyrtud.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyhxvjyk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fzwpnrsx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zoktcnvx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3yaaofwrj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3eltpqsez.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3detbrfrd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lcubzmdk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3yemescii.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vtmgutkq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ldyrqhjq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3uwrovrax.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yqtcjuyl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3sbokeeyc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lchiwnol.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwolxoe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3koxwukmq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wzhyhnfy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xrwoucxo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gesvujaa.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3sdazvrrg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3uymoxfqe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qetnbmtv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3giratujc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3votphfmj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hkjjkopn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3thgyqrpn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hgvwvemy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jnocgsqk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3clzwuryn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3yhgskjjk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ayvrvbph.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3svuoigqs.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3btuggqcs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vmgztfmo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mxduiyzn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mgmkwmyc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xjdifoax.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3lwysodzc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ochgdces.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3eysojpfk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdtoxkxa.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3eiobokms.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfpqfcbc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jfvggcxs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lxbcsqce.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyvrsokq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3imwdqyop.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3awfnslrr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3crcmwiqx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pldnozcp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hudjtdsu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qlnljnwu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qnzcrfrv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3akfkklpo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nxggqllk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xagrgweg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjagsdmf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pczvgkve.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gfqpeeua.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ynelkssu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cjtrojqd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3pzlofqrj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vqxahdso.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pjgwspco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yavtwboo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gdcuflsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmqydqod.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3igojfevs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pjndqsmg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kxrbiqbx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dsxmrbpa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bnfspamc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hqolnngp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3fgxerako.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3izyicgvo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3slfwmidv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pzhipqcj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ophgnpql.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vixxsugk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3brnieiza.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tngaoqob.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mjwzocuu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3rkvhuquv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3uzcfwerz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lrqfomum.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vcrvooed.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wzhfbkuk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ptqrzldv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3plcoplcf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kagywzzy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jzfahuct.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3invfzjis.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3oonxcoxb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uorcaiyy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3towvtjyz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eciuckce.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wfyvjpbv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nxpxcmje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3coesluuc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mjzwskvl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uyrbcwfr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bdptujdi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zlqrzgxz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3eklxssik.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xxvqsiwc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnioowng.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljpvuhna.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ycljqfbv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwwxjleh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ypclpcrf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ofqtlhcj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwflxqdy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lktwumlm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbrloohe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mbnyfxbn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twtkwdum.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ekssugdf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cikymdwj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okanptms.html


<!-- 参考信息 -->