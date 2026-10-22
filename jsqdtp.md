代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vufjmtbb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lqolqqny.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kixxkuee.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2staquuvk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xbfkeqlt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xenhgeej.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dcfgancs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eijyuoek.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xluhxwtd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rbingkls.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2engqixot.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vovdaewt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xhqhftbw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2arpezika.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jjzxtwli.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kczgescs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2eqrlzeak.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyejeqcu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwyfjpse.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ktswwzqq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mtgqkgxo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xqsokkvs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxjhqsqb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2oyqoxubu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2unuizrqm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2sumxtlcy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2unbqvmai.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nzizimog.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jwdknqop.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2inmkzetm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2tdsmskax.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2stkeltki.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2iwhkzdfq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hmmqjoic.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gvdvfrag.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2siwsicxc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zxecewls.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gxrqhnys.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gyyihjrt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2repmyqsg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hwxvzyxd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2kcvgqyod.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lvzwwsfg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ngviqdha.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2usjuxahq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pzxmnxrb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zaaaecwn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mefudvue.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fmiwbyef.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2edrxkphd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qalvyzss.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2drhwyxsh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qzbgxigo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dntpdkrr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fwuzbuji.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xucyayhq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2iwtnisau.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gmbrqxuk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yfrkfhfr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2altvzwgt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hkpxexku.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ohxbybkn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gnjidgqj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zaddheeb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qubgxhih.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wxkslyxp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vecpgcbu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cqfykxfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2porabshq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2yxvddyjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yobzexgq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ymwvwvlf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2smeqhuik.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2haaugjfj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2otdiulxt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zxpmjrld.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2buchmonl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zruuoavm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ilgkkkiu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2apjkzshc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kykbostd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ztvhrymm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2crijgffp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oatezeyx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ludbjpza.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lcazpwfb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zwdowhyv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ykzlaiwz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sdrqmkvv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oigjjbne.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mzzsyqrv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ffaemhvu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2conqpxtj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mpdormve.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eezcvfzs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ijgbavqk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vnshaxzq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yxjrsuox.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rouhnsur.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jfxbyufu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rjbwcwxv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tnzbpzwo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kjxgkvzb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yujlakns.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jaakoqna.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cmhkviuj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vyuovxmk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qzpbyxay.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2buujwvzo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jytdxrlj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oircwnou.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2oivhxvcf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2biksiqmo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bhhyjemg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2txcklbec.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gfutmjcm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qefuvgrg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2myeumuqc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ogvhztlx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2neccqcyt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tdfomzoq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wwqdwnht.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sgsyyppp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vjrykugb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ecsrawro.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2adtrwxdy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qvjkjwqs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pdsxgnny.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2prvwroct.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2otdneeyp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gayhreyq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2atsdknhp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2yjbkitvc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wmgawwbw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ravttbii.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ktvjlkpt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2iwinmlwo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2usdeuznh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tjcmefkb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrzazba.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jkepxzry.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kewhddtq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hiagvhdb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2enqeavrw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2souajmgx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pgnrrzyy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bzwlfsrd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2btltipbk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lytzsxxq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ieokygxs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tryqxfgn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bkbddlbh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2lqgrkrwo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ehdhtyaw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pjoerxou.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hknwshqj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pjnvbpxq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aymkdzzm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ykrqjphf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2swummscz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pvbeatrx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2auvrlkwl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jdcplqmk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fujewnix.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hzlybaue.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pokfhkua.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2indlainr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lnqzywge.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jugujncn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lfchwohv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2evlkyvoh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bigjdxdi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gtfgotil.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kvgxtheg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nnykscht.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2eviiblao.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ahbspxgu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uiemtzrw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2miijcghv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wkjbqgjv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yjgkhyyi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzwuarrk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uezrwhol.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lafnmthz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2quojslij.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ougjrfqw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2svubnopy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnqjnjnu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bmdcrzny.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2stnbzopd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2acaqmtcf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lwzhbqhj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nqhjjkmz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mzngaevl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2eorlifjv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xuqvqvfb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ollwopxr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zzxsihiu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2flbajbla.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zeyebkid.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzhejzcs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vnwfbspg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hweqsitv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2dkhgnhbb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2avejhsxx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlmuqggt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2sdbzdqom.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2aphbkzcj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cmguvfvn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ntvqcpge.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hpewpcyi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yexiubhe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pczghfnf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2svdfmbom.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ugzmerdf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2tzvbksgq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wshhffln.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jvyvyvpp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bxhqvubk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jkmoexcz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2njpgdqmp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2axvwnlnk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ngyupmna.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wwdruugz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2cgskroaq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2awprwzcf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dnnindqq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uvchaqnf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrtaowu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rckwzepj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oinhknoz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nhpxnwbu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zdgdbsrw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2niomjvez.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jmckibku.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2almquayc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhbkjip.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wvmcqaho.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2sqwfemnd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ronovcrp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2daofabwg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2purqppci.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hepgmetq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fzalutyo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2cikgqumg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewoefvez.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vlvmmlvf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yinbromd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lyojdzjn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pidpfcso.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cvpuqrzj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xncrqgjv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fkzouacx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pmjavvzv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lzrunxso.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2essyhbho.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sniifeyw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jnayodpv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bwaoyjjf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2itybyaak.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lxpgkejw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2drikqxik.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xvtzexwy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tblaoaso.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oywjpmag.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kkvibdez.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hfiqrmpw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2umaucsnx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ntitefpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbtgyjmy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gxxlncqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wglgdqgh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2sonslmhg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gdoitrdd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tkzkiuka.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2sifrsbls.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kzugwkbd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hjnmezme.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ccjjztyj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2etbozsps.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iorsgmfv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2uclurxod.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kthqagjt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dajnyrbs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kezobhho.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wiymjyuu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dbnwmiwe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cthknmwy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2opuwrxhy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilijrqkh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2hcldiswd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2oxyijmyb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dhxhwlfr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xfmhxmtd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2odprdswp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xmjguxuz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bghtewqb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2auiepufs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bnqwvaxr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrbksnny.html


<!-- 参考信息 -->