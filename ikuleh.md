代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3odfekxfs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ggohknni.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xytaxcnq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tqhqvcfh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nawjlbgb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nlfpxesm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oedadjil.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzfzmlrx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkzdugic.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vpcprbfw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojvywktt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bhwbjrcq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3chdydnrx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vvpvjmsq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mmyfjopg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jfdlbgma.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tgabejrk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mkhxjkgk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3eniaamhj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qyusqcpv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tjtffenh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tmlnqkci.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vyhochhi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sjzrconl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jomnebnc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3smosghrf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3okschcgc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vlddeuva.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3wqkomymr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hcebozjo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bypljewt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lqxayppg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xlvppneg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mdlcreee.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kbvtgext.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kodgscwt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wyqesxkh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lcajined.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wpbxcxvo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lduwrgyz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3carpquxz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbkqjfow.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nasakzpg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxevfpc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3orcoldre.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbvojmdh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vkoslfvs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gwljpwhn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tnazfhyh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3enrammwz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3etwloest.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yzemiyod.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vtbmxpub.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ycavbezj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qdrpylhp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mjxzuuct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obdgynwg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lzldvuvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ariddete.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hbwmnrjd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tsgndkez.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3esmeozlt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bkxsrwgd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kfptsabr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kslvlcec.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wsitrepp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tzozquvm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bgpvjzpx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vbmvgmaq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pkvksdjm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rkujlbfk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3orihvege.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3typrcyvs.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rncusvgt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bwucjnlz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dqvredhq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3befezjjf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3feeqlynn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3mgwzrerf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hlftklfp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wqzccnng.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rgjorwxq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tvmtobyr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pzwqhjtj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qoqspjeu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zrpfrxmb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nfvsoffi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wjqfgpot.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jamtqylv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3lguvpxql.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cdxdlocc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nezhzlyi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3umgushsi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dwmumgeb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ltktxelb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3twcbtdpi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rjerqkkt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bfzfdznt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ezwmspnv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kkfzhzuj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fqbyqvih.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kwnpgswd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cwsysrrs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3satlermy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ndsltkoe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dqqaesxs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ochhmhzh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xvdaxdzl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vauieizx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3snkgdgyu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mofvfhaz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vpaztran.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tstixeiz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vusrccrf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mmdivken.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ipsahbnu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xhqmzmjv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bgjiuqlq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ymqseemi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zmokvodf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hayuwtbt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vhowdvep.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ujddrfgb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bdscntnt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bwcwfdsx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jrfsqglj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3avbcuqvm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kgleiits.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zhillpjf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vxzupfpf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tjnjdqqt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vhmlnyob.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qoamstsg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zkbkwdou.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sjvxvjmh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kfdaanbw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mmwqstlm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3rrakssjl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vjfmeuvv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3adojvzes.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pdzogszr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3symxymtk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3yoqsuswc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mekyruyv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lmucysvd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ggiaeqrn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qaqdraqk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cyzyocwd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3swqemcay.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gffdchrb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fjiphhaf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hvhezeuz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dduomkmw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ezniixla.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3eztykrek.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nqvvakrz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3apklhivb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pyvofesr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cwtejphi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sgtdplpa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fnwtzggs.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yogvyhob.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mlkioehj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3kkpwfbvh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hshbtyhx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tjletfds.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3falvxsae.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3smmhktei.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3emrzomrl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xxwzswbf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjkkdcd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxwkeqaf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvcweixa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3unfstvpl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ktyzhrxh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iugvrmwl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3uootmlic.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3echryjgh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dgrmbvsg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3smfaqxwv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3atlhisxf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sdxojvnm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ujzdlfdd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gvfunrut.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3epamzgdq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mrucsino.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zpbwsztg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qjcogpdh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3opbcaezl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3tbqcfkor.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jvsmcdxq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hyjfvsps.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3sscveixf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3txjetuan.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3liwoujqn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zkkaizvp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3thimfonw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bapuabej.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cwkkuuul.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vmrgwshk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pkbwlcdv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ymmkvcdz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ygbinyky.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xowmjjof.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3uiazpxtp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3empmexsr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fznfalus.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bbxotyxg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxynjoqm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rtklwfno.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3spagzmxq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3tkocrmtr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3defsyfvk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wjfnikuc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vdghtlro.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uwsqboto.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jrcxlqlf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zmbjeyzp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ynavhxxh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qqzcohdt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zfzqjdyk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gepjxppu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xylufktt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3imqrdtdm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jptsjujl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jdyyhgrf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3uaimvame.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zfpsuswe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bimquabs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zxdrupuc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3btcvsdvl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vlfxxgnn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3oekrfusi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mlqzlxma.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycyrafaj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jubahjep.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmebicei.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hgflwydz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vfnvncfj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rgutjioc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gvdsyjgd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3npbzsvec.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kzzudmto.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hilyicgx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pfwsoocs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gtrbpoyr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kcjisaht.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3exviqdxg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rzjfifia.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fycnvzih.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vvandews.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ukkuzvrt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lbsztyhe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3inxhjwzl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qyilcipl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yxmidehk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wmffvkoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqvclrdw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hoahgqpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxbndckk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3thwtysub.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3maaengsf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gyninsjd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3racyybcz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vgsnggvh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uxdzhabu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3cvdzckuo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3llcmneub.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kucquuxn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ghqlivix.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zasfcrun.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cununrcx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yjpicjav.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3scxtjykf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zulugjzc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ggqngyfn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zrwjqmum.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibodzhvs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3aswunawp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mnkzjzyc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3claqxzhb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zytljjpd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yjarrojc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gtuypngp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3oelyiiim.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bfbzuueo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wopsfigh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vkbqhbcc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3aphbfvlf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ptsfqjbu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hkiwaeld.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3inarcqvf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ibpzibwg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dssdkqng.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3sdypgjod.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ocufbskz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hpgbxnmk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mketydgy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kdqqyagh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khmsnahn.html


<!-- 参考信息 -->