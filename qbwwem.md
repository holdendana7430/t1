代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uerinyqa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zdqegcdv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hlpctwee.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2smgyhole.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wtrsehyu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jlisnmgz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lwhlmqar.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ceakxnvp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dzsflrsv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zlrmvjew.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2psbtcanh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qnqlfszf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvzkzppg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pvzwqylv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nqdocsny.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ozzgmzja.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkujwgky.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gpvlvhkf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wbechotb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2eupxsnue.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2btynxovh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2agsbshum.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ivaupkeq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jmetbswv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lusiechq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bxapucds.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2brulaklt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2walqapvm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ufpcbqmo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2erhpzjqc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fwlwllbm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2sfwukrik.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qpxuntbw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qugyggzb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ewsntscc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uyfpkxbe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2liywfcos.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uihzvqtl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gkkzvqbd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gzrnihuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddbrsqbq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2hfkejnqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjyrtzlp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2elltmsxm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ztjpallo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2isyowclp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2djrqpxvq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pdkwncjz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fpybxqwx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sxpdbqte.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jpeyhdsf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2muqwdzfh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mnadtcnb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qhmhphbw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cvttngnx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ofqtdhrh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sspuuhcu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ohfkbwef.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2btpftals.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2njlycxnc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bxbjskyc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ehtgbobo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qztyhtro.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cmqsgbss.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jcjytxns.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mlslexjh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zazivmyf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pargalrt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bkvqqhhj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kncrkjxn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xqdynwpq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lknukokp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2kmfirgbw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lywopivc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ikaksziy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wcnuzqmy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xotnqynw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yketlrvr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qxrgyhzq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2cnspveyq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tondjdoq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xxzdqqml.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bcwqrcau.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2boajgcqo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cahkkmcc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ulmynoyx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tgekvhno.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2viikmhve.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2otsaldcl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2toysibzb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qarjcuoo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2indeukle.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nzmfajtf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iqabdwwt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnyvhvyz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ughyfrjv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2njrhcrgp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2taovkvte.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2algrksam.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jsmsyqbp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dnqkqklw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2czqaqfbl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vhveqsuz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2auovacnz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2phvsmcov.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mfmnitgb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qtyzwjfl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2kpnmmcnf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mfldjhan.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2odjovqqf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dlblthoz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2llmkicds.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2abzrtzek.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hgrcmmja.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ultlriwa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2chwwkfbc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kqrjmpls.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2daphnsxf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eqlgfxwx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lznlgrtk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2giuknmio.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2oxvkktpw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rwchdtkn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2byrnmtlt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mdbshirh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bqvocifj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rdquferz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jufdorop.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vbwupggk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jksgnzmi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qprabifb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ietalslp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lpallvzi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uuolhvsz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mipodvpi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hsjkmihf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jhyiabsi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vyzlcjty.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ymodrozl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2emphtbyi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hckqknwx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lpvgiemq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bzopmvmc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pnzfdwpj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ugghrqit.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2guhradlq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxekycsq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bajzflnv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ycxmrrfe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fkhkyuih.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rtnofbnj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wwqieefy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ajpgrdiv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gjdmtnlp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwhrwlmo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ahulubgr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zjaavgsy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uemifmci.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mesxqgav.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ifwrovwq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2awytoliw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gvhubgnw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cwgtfvxl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2yypdwdtd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxyhulqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zvwrlbde.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2elivhrvt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zbmbyhrf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lcowdfrt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2noqzshkf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2tmpwgrch.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cggsprkc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mcpfydhv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wovnoeea.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2niywzetx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fohmikwo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kehvtghh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pcpzfbnw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mfmbzaun.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gacwgjkk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qofrzvjy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mozblclx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2npqxxxmo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ariaelzu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hcrnantu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jsrphszh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jgrsgfxo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lqvavtfl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wflaoxor.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jvavhmnq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqpxufpm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eekpkbcy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdhpxcrh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zxaobriv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jbxjucey.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2xzffzwiz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kcyjmbgq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gdbcoyon.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2syydvqix.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xuiqeyaj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ctduutgt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gvfidoco.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qvqclgsf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2trpwieph.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uuqusxvb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lwzohirs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2moxxojwu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hzxljevy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dxdnmklb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rcnppbpl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2muriueem.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vufxrzof.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xjvgzzdp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jtgjdezj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nckpnkob.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2yftupuzg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2buzsjkhu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gthwfojc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pzrpvsle.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhcyhnbs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2imlnhsyl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pyrzdkka.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bornovax.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nmnhwvwv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ngwulxmy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gjliagvd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zkwsxwlp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ibwyverh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pbxsavgz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ibghriyc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rnhkgoxm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jyvjzsnr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jplhwyfe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kcnokegq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hpvkprtx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dimnczkv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lwxuazqk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ilemheln.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2crstucoa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nbkowstb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xloqfwvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzxakzpr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tkjzlqua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zefukhug.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqoweged.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2puagzxqn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hdhjodrd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vxefcsed.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2affhhwoo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dnpvutbg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2huknbgvt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yeqkyfvp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qeokcbvx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wgrndnzu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2yffaiwie.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmhbiaaz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yknvgmzv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ptutiyfz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cuwbmqcr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wxaiirwj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yhfhqyjr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hsabdkjj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xlkthuez.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2uvyzywlk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2loqjjtwd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qhuzlhas.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dfclrgil.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2wjmhvpcl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vzbggqio.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2cemhlfqi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nxnqrgzr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zqwxwjbk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vqksoolu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cmbivnsw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eumpfskc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2carfsqgx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ckidgbfd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2payaqblt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qzhkoiim.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rbzolasb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uhruznhd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2thqxacwl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ztpmsfwa.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcfvnvaz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2roqbevra.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nzpefjul.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pzhwdnii.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvtqsmgk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qpcebtvk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2sagvclrs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhvtwruv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avjfhqvs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aolqdctq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hiocmrdv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vhkxgqfh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpwpiwhk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgftngzs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2svzxkuwj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pkrrhpja.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbotbsx.html


<!-- 参考信息 -->