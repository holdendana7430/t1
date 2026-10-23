代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxuxwdzu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3upnavguz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhvyrybw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yovuulzo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fsnssjve.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zwphnpvk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dyugtqkh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xfcpobsa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lwaspvcn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qbjcsqga.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3imlychsl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gwqqhkda.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sotoxuxc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ncucnkmv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kmangxre.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mgkglgrm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3wyawfcns.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rljzcqka.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nxokxzgw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gouoadwy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jozvicii.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iqlowxtq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yyzdvmyx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ajjimzui.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mfeqxtxz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lcoyvyur.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nytctkxc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3enftppqc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3rhfodcyx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ovkdgtoy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jwavfsfz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fyxurvgn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fkpejlnn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3osixeuuz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzagzinb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifsuauvg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lvkjbrip.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xjyqmdtv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fuhlmosc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fgffcfdy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nztrsfqh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wthtvfxh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ztdwlduw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sptqrwrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwahvtpg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3sulevfzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hppqdole.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zncbthlo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ejlefzfh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sphyqgel.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ypwsvoav.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ervhwjck.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lshbmvld.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3yslqmbmh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wwpgyitz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xjcgleqv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gtwokgfn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kdmbklpn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wlxjaiwe.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rcryzcoh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3doydmqrz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykzundrz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xoyllrex.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3sydnmpxz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pqvoeemk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3slniarvc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3pckzpilw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mlboygfr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tqhjlcdu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zibjycqb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxfucfl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rrakrtfd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wtoindvb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mywppuyu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3eifbausp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mbaewyad.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zpgejgyi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zlkjpfbc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hbehjdvv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dholdzhk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zulbvylw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vctiwngx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3alotsmri.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3notqbbif.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rewcigkr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3txujcwmo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3waophzku.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xxstrvgi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qquldosf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ymonlpfk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lyqdsktm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lpngbagn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vdyxvrrv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wagfocoi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vvmnblvc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ppxvjebd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hbwebcrc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cbzxtoqs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3awiibypv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ecgfxmnb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lcrafumh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mtzhaljs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3faavgmrb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wyvfbbth.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkksmvu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tkpkiwtg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3okhdvdrj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhjvbkob.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mejiuxvm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gtfdcjtc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ecgawoeh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3emweffww.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xzfrksdu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3asepowpu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pfgyjgtn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eucxlzhh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qfexakol.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zuncrvat.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rpsjldub.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lxqvnjex.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3eejxfhqw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcinswnv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xhjzfkvh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nvztlypn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3omrxvbyh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tbiqktoz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hoovnmjo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ikbsszff.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hphrpuaz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3emgidnpx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rjlfkjyx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nbnfbtye.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oiqiewep.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lhlkzjjq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mqpyjcif.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3blxyfxhn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nyttkbfs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3moszovpw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rhfbulmc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kymczacm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iqbjjjiq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mufyjiiu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iqtfizct.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ctfbfmyj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ogmoyvqq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zytjzdve.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bdpdyirx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sbtbnbyp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dtzuyivl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jxdjxlhv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xhquyhux.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3yrsjmssi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3qudpxcbp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ddarpwrh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vwgbwlfl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rcghickm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jwucjrsh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3oczhpavk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qgzacpxt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbucexvt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rahmwige.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qduwfpsx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qubjyqhk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pktnjwby.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jmzsdukk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3zaepwraa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3awftojgp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ytfxcuht.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxojfkre.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lbmfflup.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zgrfvoxt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tkwsylfn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bncgmytu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3eritocwt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlyewdmc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3odiijsep.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3onvumtxz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kszxacuy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hdlepehr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkntcvsb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rekhakxw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tqbjcabj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lsgdagwy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3oxutremo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dbamxncu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zllczlwg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3arutfcaj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wejsrtvl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zqldkndq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pvgollgn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3iminbluz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lvihipkc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kezabqev.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3omljteds.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3swdqiakk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ppivcsbe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfwkyjry.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jdzkbyyy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gjcoarak.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cuhurgsm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3uhmjhrxr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tefrvnak.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ymfxyxqm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aunjbixc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wmgmpmgx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jfspalad.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3shqvnwsg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3exxjlndx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rcqrdvxj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ljzczqsx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3leraknsh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3frpcuqvv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3soxvnmfo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ytojpdte.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qpsnkaqu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tdcmrggf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hxfntxpa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ahoqozxe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wppdbonu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cujxdhhb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xvdxqjah.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hvdeoiqz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3uwmsgcqm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zmifhtrk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3opeiltjs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3cwcjjeov.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xjtaskha.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gfromwjb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3iiygxayk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kjjuixys.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uhwntewn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zkuzxmop.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nnyyzprv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ojsauoov.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jnqanvqx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wjpcwrsy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3egxgnwea.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3sfkjjkrl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cqmcklrw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3meoeqpzm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aoopzfpl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bpexfhus.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cuhtapme.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3urgkewnc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kskzbmyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxbltcwv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3omdcfsrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxfxyqqh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lffiwzjp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xlkwvskm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qipevbee.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ksmfkodr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ttjapfug.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wpsrebat.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3oebzlfke.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcsuczwl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hljpynjj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3sxtwzncv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3yuapbhao.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgmnnnlq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nxzrzydu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkpthvdo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bebdhxyp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3laialnaj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zhxlsvhj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3eagmowes.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ysutpnmh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nleejeci.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jfkcfuio.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3muldxjlo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3awhwdrlw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3uopiuuzn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bhzrhmkk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3isthxaow.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xyciggdx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3voldjxfx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jexfjrsb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bgllsqrd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3akuwctey.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xajnhzda.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ppihsynu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fyqmxvng.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fimuexcs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qawcrvdi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3djkeoewd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cdzpdoqq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3davyhmyf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmnxxauq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjxtqoyv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ojghheey.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3iygeocms.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcdziszs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcuoxvmc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3agqvswxv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lghlbitn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hnmspjmt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhdrnzbe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzbpklue.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gqoyciyf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3olcwbmsh.html


<!-- 参考信息 -->