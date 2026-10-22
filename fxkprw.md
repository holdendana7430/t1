代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwuqrngw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnwsmzau.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhbxsauv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kesmcvnu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqnojgk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ekzkkfti.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xzbjijax.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qdzoaixn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zidlghqr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mdeyeaov.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vycseizh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kywrfyvn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2olnydlsq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dhhrcajc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qwwpnqfi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdtulky.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yqphcsoh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2yxhvsvvb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qpytndlg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rrrikehq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdsbjsio.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nnrhppxv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pnbyechf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rauknhft.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pddyotqu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zqhmixaf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uprxdaes.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qzhgluit.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ldeiiphm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dacwwomr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fphtuhef.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2udgnxebj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mcwcjamx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vlcjzpvj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2pmfapsyw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yxarfwpb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fzjjrakw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2scatxors.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqfhbqaj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2sztbwpbb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tozyiuvx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dtwsomxs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ebdopgyh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vdxmyigk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zhisfbmd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ovxhazip.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2psoawxqr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wepcieto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdudzmbp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dxsqmoqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbnyglsb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2odbgnupp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2uoccacxn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yaifpgmq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aewfwhhv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rksnmsaw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gmlnngxa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hyeyrcoq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2aobkdjxn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wbkdlzez.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2geucqpbj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rjwebteo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jzdzncpx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wuaimehk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnfdlccp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zovhwlff.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lbdzmrnt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yovbuqck.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2prlxdfyw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kbtdmcwa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2huesucds.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xcnelxel.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzluutx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wllgelpy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rgeralzw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vgiaumdt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2omxeygmh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mjkoxxrs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2eihwpdnz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ohswzqfk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rqpardec.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hecieiwf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qlezevza.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gftoljof.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dspajnjp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qdyftays.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ijtjtzbq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dgjibwab.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2meyfkuib.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fqavazwn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mgqkkyjd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jkahtjcl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ezpiyibr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2epvbjcej.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2iyvbazzb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zpjojjbh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rwzqsdjz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qclinfxt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tpkeffkb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qpoavgwy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yzqjuxzh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dxohqpwm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dmumqizt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2butnmfkq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2csklndyw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2okvuqqdt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2eurrrxhj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zknozffm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rbeurreh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2oifgkzvj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2cqeedhsq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rwyrrbpt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ppoozfrf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zadiraen.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jmlewldg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vffmfjzo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xjsyygtn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cbysokse.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vhosbqzw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wnvccjrq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mrrrlwrm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lkaurkqe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2szsyynvi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dpmhvtmq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgezldwc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jccguxek.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ezmzwcgi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gviqrrhd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ekcjtjfl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rkxoghjs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wyzxeqpk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cblfeywt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ltoznbxd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tgoyqyxc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2lzkcxqez.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wodtztyv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qtzztoda.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2whcnqkur.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hxmvjima.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rngokenl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tjfmihgs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dpoagdhx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nxdepslp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sjujlepl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uinwaslz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uveccayx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lsxkgouc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rzeentfb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cmceylhy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ioaermma.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eoaabkjr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sagncepg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2lclmgddt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvuqminx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pswmoquv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pxemmuni.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vqggwlrr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cyhssaqf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2abqdfkyc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2intjgxnm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2exhipjgi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhiumnez.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwpwpggg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zenequfb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gwwnutho.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2lwjukmpo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hvbkltyn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lgvgrihw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vigvfjdh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2smugkbld.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2covekojf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tpibawpw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2efdvyrfk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jzwtblnb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ymgekexq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2alocotnc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tgxyotea.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yvnslctb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxlqtom.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2boebqbpd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oyzgzvze.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2uvmpvoar.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ankfbtyd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gnqlhtqw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vviksvsx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdymzmz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kryzxcbv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dcexpgsb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ryumuhsc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rogxkagb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xenehvva.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mlejwzxs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2plcyisxb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kollxwjq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zmilmmuw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ydebssjg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zfkefdxx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nzyepukp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dyrwcavk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qydptlcj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zibgiljf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uxldxdxq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2juftbmms.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wumsaqev.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2fchxjaiy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lpcjzfxr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2icawdhfb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2azfljtsv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ldxftixj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uodgozcy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gcwqekjn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zacldzcx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iqimigil.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nxmazcuf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gmguptiw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uhaibvha.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tcbmxrgp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qgsgxopq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2npvpjifl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2swymhmbc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fewjfmtc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2nnpmqesj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vpmzeueu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xxkzgmaf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2irupjbxt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqhbfcqo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ravjwuqq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xrnyehhk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2flobqgfe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wjelmnam.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvfagwfz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mmegwwhh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mjzwirmo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gxtmyjlj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2enjfjkfv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aqwstbzp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fjodarfi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2iyjopwoe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2afvycbnj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fizmjhxu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2egsjicfu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxaceidk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2chvnwyal.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2itfylcml.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2liiladdo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mnxupcbg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jkslfnhf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lioabcwc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qmadnwug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndypeexc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2unijkehg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2coeowhng.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hynofphd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vtvphzqf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ajrmycbt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mpxigdeb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qqwnxgot.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vtjgfisv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ojztlyij.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fypaculu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqglhvmq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohhdwaxu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xvrpswqh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tngyxlan.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jiwrefyg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phrytbxm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jcwesasb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mvoiyfiz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uotksrae.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttokksfr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2suvczrnq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rmzgslyp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2efdvxawz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zborbsto.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xpfdpcwy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cznhreun.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hzucjcdv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2yfjbjale.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gkhwqjge.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wqbvscfq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vkkefzoh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nwjvbiwh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tqkaeadn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fhuphlak.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ccufgoaz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cilrzkqo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hwwbftnx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ajqkpwet.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2noufalqs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zctcazrq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xujuruce.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjjfvhoz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jfkhaysy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bmulzvpp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xmbrzxcm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uypycpyr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcmfakac.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsoyotwh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mprinazu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kufsckti.html


<!-- 参考信息 -->