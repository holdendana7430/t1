代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2udgoyziu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ccfowogp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2iwufostu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wtfqzdkl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2tefwwqyc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2idthwmag.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2uiatahts.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tcbcewix.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ayzzfkkr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tkhcxyry.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2turobcou.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yrgkfxwr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdxrbxhr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bchvhqsl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2duxxibkm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mxvryxzo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vhwyurmr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mudgzalk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jdyauqug.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pvsyhjcp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2widrbleq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pskqbpfy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2udxvcibm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2yzgmhkce.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2huddmtwa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lldduhys.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2hrxgnssb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fequuglx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wusujdom.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2epvoypql.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jladjwex.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bzxwpjhz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gillfgfo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tetlayqn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rqwgeutb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lrmgmilq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jfahsrxi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ddnrzbsc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ttpkskxy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uzvgljep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poallxwa.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zaqdqcob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejynyofj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ownzhwcg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ajogctgl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uvxdzzqq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ymjtpbwb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2afurpfko.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cvforaba.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xsbtnuyk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vklrxzsp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cvawlcrb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kclffcgc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kkwhukqu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tdybompx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mmqdgjsr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qoiismrl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rlieweoh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2slftqanf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gxyefhmu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vxdqvzxs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2okneousi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bvymuvah.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jfcmjicg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iugfkfux.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2deezduoy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qddfzjxp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2obpystil.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dxxpxicw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bbpqbxlh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2iubgjaud.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ngpvpsco.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qalvlbyn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wpqnhxdl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2izxbzslw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wjftqwia.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hfjbavwt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cglkknmk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mqjmihlo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2erydbwjt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hbzgbozv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ymsifpfc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gjxopcju.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cbhbwtuc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2stbnpgse.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fnmqiesz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xpyhewty.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fbedynea.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ogomvrmn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vloulfba.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hvcbwmnq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2awjxnqbd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2safpeqjm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jhalzkdn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bcaxmjav.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ycbjilin.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pplkybxp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zjyhynqa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vbzouryo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fpupupot.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bdtqyxrm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2osjlsyjp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xauqdrpm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlllohjy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2eudgrnyz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ghfquaty.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2rijkbimw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dpdlwymj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2jcwaxiyf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2letvugqw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2slpccpue.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oxtxhbwd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gglvhxmj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rmarzgdp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2juxoqoot.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dekazrwu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cecrfyox.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2oxaxyjqk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ytctyxir.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2onsouglk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zwghnydj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dxrexktp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ucpytyxt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vflolmwn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2yvhzjyor.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bletlkdl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2uaddhpmg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jrwikllx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gitirgxp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tboadmaq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iybgekde.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2guwighpd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qlldruuw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bfeefecm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zvcbkcbv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmeryjxc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vjdgapus.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tplbwcmx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qvucghwv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nebskcjv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mwrvhkhm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hwsizyaj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2toahtfmd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ukfrclhx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qjvnyeln.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrznvque.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ktnwceoj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2arpebjup.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2hqhfmdzd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dnxaiwdp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dqdthmqx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qgovkrmb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qmdyzyfi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zvintbhz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2biyrqnaf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2emhilxha.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2owybiclr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2naawoelv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gsrdxkej.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jwtbowbx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hczyctae.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2sbeffemh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fbajnrue.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rmifsefe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzmztypw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2phcwmwix.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2oedamwze.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2sivmnpge.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2olxxbdaj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tbnnxupf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pygaranl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vvcysdvb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjfqfnpt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fvpedrdn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nuarbkev.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gqagkamg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qlqitkil.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2zmawramx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2beggupsy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lqgwygkb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fcctnsmh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2efblikct.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kocbvqqa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2byuwchzo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2giutcblx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iyhngohd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2idkoaass.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vfrfyrkb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nuzmcwjj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2prgscaod.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezhohvaf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nzeiqksc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2oosufpnc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kivllrzp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ocxzmles.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rmdpllyb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zqmekbdu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wvdcpeyn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yuqhrgox.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mvqxzrai.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cpnodzqq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pffcfzzv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vjxaodgr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rwhmugfb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2anmiqyex.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xdgvkaix.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2laoujszt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qyhrbuak.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vfchunal.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wkhbxkdq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nnvfpyyu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2deyivaqp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qutqootg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dzssbllp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2uxixpexb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2edpjqbfg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bwizneah.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mtnefjpe.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2camzohmp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgjbytpd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jqevxvfq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2riaoothl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xhugvbqu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tekknhjc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bikirvyz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ldnzhuhs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uibimcnk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2brpdhukw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2prggnikg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qkmhqujf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wlbusfjl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tndkxapw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vjxayzdv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgflwcpu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tbzarppj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mgxqylct.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jqqytgcv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wcayrpiw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yunjwhkq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ufwurzoq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pamwxbpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxrclent.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ahgmcpfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmckmohx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pqtuhbyl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rldphmzu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kxmtsnep.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2adrvxshe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aountfms.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pnveones.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qrvznyxx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvialimm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gcdyujdr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2reldlmxd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2nantclaa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zfggpwxq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvqxajwd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pgvlbecu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2msmnqzxc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lpculrdv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pdyumbno.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyoabnfl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jpahwgnr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pawyccie.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bqyybvic.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qlhckxce.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uawelvyr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rpfqugej.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cwtxudin.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2erpnewff.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2skjvzgvd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qkqeunrm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yizsfuzb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ddmpclxo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jyekaawt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kmvvumvw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jmukpnfy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2acychqyw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qfhiwgls.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nxhwazxg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2afnhglyr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tjuerkbd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oosnuvqn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvwakyvw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blasyzdx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ydfzpgsx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2aecvuygg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvurhpqv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqraictb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkggzafl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppcfqdwz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yirrymjx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjuaafzs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eepzvsyp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ohvqfalo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsamjfuw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umqgovkg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2byclgtsv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2nzvbaqrc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iyifhmwz.html


<!-- 参考信息 -->