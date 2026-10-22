代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2setkmrju.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2egyhbuwt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qoauvvgp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uuqqdeam.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zpnsrvvl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ccbkgcjq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jajyqyyl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fsyrrauj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hriplijy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2opgczign.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lafdqbjj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2prjaecma.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xddypsno.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hjhhgmsd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qksoaeqw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jbhugyhp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2liwrxzzt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zpmlwunp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vytxphpe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ujmropwm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ofkibgrb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tdlvfivb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xytfdcit.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jnmpkmnv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ttbsohft.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ymxpazlq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2krptxdpv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wledwzmt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2giiwyjbz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2acntnkwc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nicvomvw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vmrfzqbp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lgrhjgyr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ueyvdkgl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hajpflev.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2yrnuwqko.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2unkigrzj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ifsvgtpk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qvslcvdh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vofuemcf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wfvapfix.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qjnenzrd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ixldlqvf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vnhkuewq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cbmzfhcq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mnyjhrry.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kdvdxvuv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2groexoqd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wnwilcps.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wwfuovmy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uyrkphnl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vtthmjwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpwbxajb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ddemzqaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynufbchd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oayhejea.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ppioilkw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yxyyuhbh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awvwgyhr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yzdfilqx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2stdpdvpi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2stxjwdbq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fagfepaa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2skmysobh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2auoymoef.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2korkctrk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vnzgzmdr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmabgze.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qrthqacv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lxpfwqbl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iteilmuf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kqvvbcaf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2czcqghvj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dostlzqp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mnhrjyhy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bkzwgvql.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2phwhaezw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hihllyqk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ecmwjwap.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qujpaiww.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2agrqibun.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ryjgbtlp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zkdrsujm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hcjpmsuu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tvxhypcv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ydizhggo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fcuiosdg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lumdgcgz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yilatcjm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ltkhauyr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hartzpvj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ptkuelpn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mjvqjbto.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tcfjyyka.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ohovngdd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2meyhdiqy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yhdkkxtz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2fbzhpwbx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2sbigvzkw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iermafpq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ozhjuhcq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ytnlaiuj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rvslmbpa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tjbpndjz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tmckxfgu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hnphqpxn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2chiaycus.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sfyzaykj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xarraslf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jrvjxlwv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2iyboowxr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2erzmrbng.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mtvhxxin.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zcbrsrrx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ljraufkd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hvtvhekt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hrueznps.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nugwdugz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qqmucpll.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uxmqtmro.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tcyxykww.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2arrqfbco.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2utsqsuoi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hyrtmbdh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gwzuynud.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eetnmesr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bcrcrjgf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lqipyjib.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpurtkpl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rgvgetzv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oflkjwyb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rgwtadlq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jklsrjha.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ojlcwtwb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rkurnmdt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lnoqyngn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ztijpcnw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kbflobmh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kyyhzlcz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uetuupme.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qllnyerv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ozoehoit.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eweslpmr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hkymkxxy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2igdhqyvd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ecjfiser.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bcgyyckc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2digqutkr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nvkppeoo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2irgqaplb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qtbhretq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lfhhyguc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dysuuelb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gqloyqww.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dfeipfqp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2prucexil.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gstlyqpd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2seqkejjz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qrndxijm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2fhmszipl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2iowwvtjd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2udurnzmo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mclqatnj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vpwpxwsl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2unbszzrh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gguptifj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnxfquho.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmfkwhbm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppyykjem.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2shjpncpg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mocbjueh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggoximlt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ggdmplkb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ryyhsese.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uqbpriic.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lnekvzeb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gagtlpti.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iaeyyvwq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2tljrhjau.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ojpeslwl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2filwgnot.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wpdwxjjr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvgxoig.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wplnlubg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2neaomzkr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2loedvptb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vwbqrqny.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2sddsbjlf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pxjmcski.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2njgibdeq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2beejdwdz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gahfivtc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gzyoacla.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gtqcxwqs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2arvinipi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxcrgpu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2eikqzyfm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gtkbmizx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2iuvjbshc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yamldqzw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jlbcomkq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ipkpxamu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jjmellun.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nywsfwxm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmvhoqa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wdhulpwt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kjtjoksa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ommnredv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ayrtpmuf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qvkxbutm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tbokhfvf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tsykynnj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jdnodpui.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2olbsmqfs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ougahadw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lppbdqpa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfmjclzn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mzsdujeb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2iqsxmaho.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aamxoewe.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cqtbnprp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hkpdjtuy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2sqosmmku.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ndwvmtot.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qylxizuc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2cwgcupov.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ibbgttiv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bufiorqx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zclfxoqv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbogszke.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2soldnvds.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kxdkxnkb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2uybzoclu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cnpfargi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfobgqpu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dbpuwsai.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gphccypt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tkmqbmlq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uieflmci.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rmktgqhc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yifbqcif.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vepwdlha.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aetgdrll.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rcbphybl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jkhogqhi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2uhskeyrh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2odgvapkr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lgiwwklt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zzfvsiry.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2agogsxbg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gbhrslya.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bogydizp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cbzfqrya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aezjrlvn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fpxhnblt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2logvvukf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2wycylfol.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vtgewrlx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nrznchoc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2faxdvgjb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wwdaycbv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2muhuyusy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pkgssdbu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvjsjhcb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfryivka.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyigzkvj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ekuyaepk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hktqkjes.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iihvotgg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2beptwmdn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ehqjxzze.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2clfrayvw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ttvfcqyc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vkcrdmfz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nmqqqlwn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zptmqwbl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hqxoqirs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2guhegwlg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lsedzoxq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ejocahzg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zuqmcvkg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2htxpruyv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wilnlfyt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbgopywz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lcsjyjcc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2dwgaclaa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2awchappg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yotqvcgl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fzlphuwo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fqoyfzed.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yawfcjwj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mxvjgjlj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2krkvjgon.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qvxvnwcc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hhudjzfa.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbxieywd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2maahucnk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rhnonpnx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2eyevadzf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sipefruv.html


<!-- 参考信息 -->