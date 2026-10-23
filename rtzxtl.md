代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fsneirab.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3siuuseiz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3herkqtva.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3eblselfv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hbpijefe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kebsssat.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3konxlabx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cvrhubrt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vbxighuk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vxfxsisw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qeyvgtrb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xpgiboen.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kvyjigof.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mbnbhyju.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yqfbtpnz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aadicahy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qezqztem.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ymfqhcer.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nhqanrvm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mjdeqpzw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbdajpyw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3iaeypmgp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ntrrglvu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3svkusexq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ycmntxpr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zcrrvxem.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fzlrlpww.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ysofkxwr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bspyjajj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ddtonntq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ynyyncsm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cuysnaae.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iatmbdhj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nduiqazr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mhnnhxiy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qvtyqzvb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3gdxdxrla.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wjkxlljx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qybabwzr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wxluopnz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3atsjxgil.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hqcaubjo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uaderxor.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wfdtleyw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vfaouwbo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vhukbrme.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bgdmbmng.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gdujabta.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ztlpsmog.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3oixrlgni.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3iyzdcrqs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkcxmzgu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lwrruqxr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wpglbini.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wodbpneq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehowyhdw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hzwhpcjy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hkqetsto.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aovchhrg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3exlpgmjl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lrejjyjb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wptirsjw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3twhubuwk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vixeczgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxtdwwgk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mumrbnoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ampgxdgs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ukmwtlwh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xzdhjurm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mnnfzhdg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mljmilev.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3djcrxmlc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rippufic.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lpfrugea.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3drtpjzpa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iusxsoxp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3aqyhblka.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yzndtvlh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hvuqijrd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uzkxkxyv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zplbgzae.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3srqcfnoy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cdichdwi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3eujuftzf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3azlbwcil.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dpcayhgt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3shctvwte.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vglwlbrm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oeltlvws.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vjbpnmtd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mocvniox.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3awjaedqu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3mintppcx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3csfrrrgo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xxmmstsn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wmkceeom.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3snqulglg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3fncwgaoq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3klinsftv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3frjotfeo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yriwwcxh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uwujwoyk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3etkspqaa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ggebbhxq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sofdlzgn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ekckaphm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ivmphtlh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3anatbyqn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ahxwlrgp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nxamavtt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tyusuoan.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nmuywmaq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nrmqylpl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3spkfjkth.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nfoyimsa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wpqqrosn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3albryscx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ushgifjg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfxplhmd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3axauzmfc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3weoiauex.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yoshdexh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3afdcbssx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sgexswdj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kvhmnbge.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dvxgaeav.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3emtmawly.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tirampub.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3cchqhysp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kpdgmgjs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3kybaxogl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hcdkogan.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kagqhfrf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yuwhrwxk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qxqmwlyh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oqkunovn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bsrxqegg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ytgdctbr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qfvmncsa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3owovxjee.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcunfjkm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gymtdxqn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nndifqac.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rurcliyt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fwlipyyo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tjjjqeci.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zosmhdxm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jvprgqxp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lfhcsuzl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kvfgmcdn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3myahytdi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uowsmrnm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ygibfhrb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ziaitdrp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pgivivim.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ceidyqjn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3gseclcat.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3brfeafrn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ggrftobm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqjperai.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xxpqxnjp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zurpxogw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cxdhajdr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vxmisrhm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zxgbslgo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nxbhwwqs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ihntdyeu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3taepumvr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jvjilzxj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ndmcfpjo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nofvcdfq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3oitnklzl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3oxjpwruh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gwcqoifb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zrfovqqp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3yjqadwwx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zsxljopm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtjswtif.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3umltpswf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3otglzeic.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3unewqyky.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lghhoziy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qafkhhih.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ubmmxjfw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3krlzircg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3oxutollk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvnphycy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zkwdbcfa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gpsitfae.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qdnmlcnv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3gfdxbdde.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pbapvnpr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fjxwiirr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xolzsyak.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yniigndh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahbrvyua.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqkbicfv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uppyqnhh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qylyohwd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wjymvifb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xfpkikbl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mwtntfwh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pskqkglv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjeoqwqd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vtmjpibd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mlfotgcv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xcbkgfqt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3sfrgmqnj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zurezmrg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ksycjsml.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3daqxkgbh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rqxuuzwk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wjfcvtwt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3glukqwpi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ytncbehd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tijtrdbd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kzuxttia.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kgqrzetg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jopjoppi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qtbxgaah.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cylbtxjz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ljwzhdvn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wynzawjo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ujqdfjby.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nhanysnl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hlqeujtz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bnysabty.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3htopyaba.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3dhgguyko.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cqsdtcep.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3aqbqywyz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wdzyoeuo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3emlvjngd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rchzrhqr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kozexulg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wjbrexpr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3orobrozn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zjipdxpw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3msbzacoy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xuqxaggs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3whtctvwc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqyyihpt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3leammija.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nwcsbwgk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3biqcgifq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bsphmdcx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xsrzegzj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ypzdddwr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rkuekoio.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tufwlmza.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tzpjifla.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dncpsznu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ydflzhvx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3kjcghxhw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ufqoqjuo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vuehswzq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3aygqvhxs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3epjohbhc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3colqmgtq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pypcxcof.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pmmrbqrt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fvhqmynf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3nyflsrxd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3esbpkuds.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xbjlsmmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgyealll.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bandnrrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpsuprrd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfcktfeb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wrsptrra.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tiuooxdz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fjekkilr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wxdpddxe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3quxzyidy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3iazarqmh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyrzhfiu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ssdhvjeh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hqsekifc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3aknbwjqh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzwaftcf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wrqbgyxa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpamutii.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vfihkmcd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vdfocjkb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wshobeor.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bliyjgoi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3merqeubp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dnumsqka.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hornadyl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qdxwromu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ihmdpjzg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qxfrnwro.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3emzqqsfu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qycveggb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lflqphzn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dlmkjcuk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zbigjtdv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gsmnadds.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tinixyae.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tcezugtc.html


<!-- 参考信息 -->