代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dlsqfxhf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fssimbgv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvodfkqt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ecnrusns.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bmfdzbpt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zycphmfy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ebrrdxuc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vmloxwzj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zhhqtqwv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3cufevfvi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gdijclll.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ljvrjwpc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xhghypwy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjdzzklr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tssmhcxq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hichfoxd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzdmezqt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ffjrefar.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ankmauhr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3khsgoaml.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3occnrjcg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zuxzpqqt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uqfpqexv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ffrqgegp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3rpebofhf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wwhuxuyp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mnklrfpu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fkpeblru.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vveizeec.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3surblsgn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3alvjkuql.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gyydwvfv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zgljfmnf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3itomgjdf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rwfvhyox.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dgpudvgj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vgqjpuol.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rqfxcxmi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hbwduork.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3uogcdknt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3pngrfpwz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3smokogyn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3emkyoeru.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3blmmxfei.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ejhynfgn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mhgcefjz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xietuvhw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3sgmwzsfc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3czmxdlge.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mabkbwqk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ipcrljts.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrzxysoq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xuiehwwl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3milfjahg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ribnfgjq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3taenzjdc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gxfucdtb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wszudmlu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iwhkgfhw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3csabxiqa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eolzrmdm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ujbvjcys.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rewxpvsd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fuemycet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjanwbbi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rwclmhan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aefygtme.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3owwhavmc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gwkxckgf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3gcqfjnam.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zegzwika.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kuwwuwqt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ktfuexql.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3henasdsf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cykkrcdw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pwfgltlt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nqbysrtw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nfaenqxd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nrwpmrxz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jpfljvsc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qfcfoank.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pjjlpqom.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kltzjtml.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cnvglrem.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3isruwzxt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lrbqxljn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rdaisjur.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fvxmqttb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xmamqiaq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ygaentmm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hncriiao.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gvnxyezv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3mlvzujyg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pphlspdh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bnqbqwnk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ramoqgcy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ebknvcnx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ghyoiomz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xzyxormp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wteylvvr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yljiuihs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wercootr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ysfdvrbg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rhfjsbkr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fnzyumrr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zvrthvqu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3epgwfkse.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3codnopic.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ggpfwhoe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tkvnogqy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ujzsiugm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hlecbbmy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3oyrhgpkb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfoeugao.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwjbfbvf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3necmqczo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wmvnlzld.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3etggqewo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qnjihwnz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aiybppom.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ttxgjyjh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3rozxdtdg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3tczfrwyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jgaunere.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kpsnezlb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vdcbagcc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lrjfgauc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3podsweoh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3iqdfnzun.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3opukduwt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xkemzwxu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jksnydzt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xekfxlsf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lvoqvlcy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3obgonnxy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uzhzwegz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lyxmyzdr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xbncudfa.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lebiovls.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dxvafsaz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wecgenyo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zurbtnzh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3onvuztdf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nbxyskeu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3onmkxrnj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3edruzxqg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cjyagvyp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tvyxbond.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3epgibuye.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aqbmltee.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fnudcqqr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3drztidbg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sbpsqmvc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hclmwclp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vvwjaypt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nbpmvncu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bvwjgoxu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cxiudckz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qvmiizsf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3myxlnpis.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aglagpzw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uhjwyiuk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3dulleqmh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uebubupc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3csiqtwbv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jjygyzkp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vnwwpgml.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wzvvtada.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qwvysdln.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3raxnqnde.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3evsanqsf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3sfdhikcy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3htsvrakr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3puvxwrgx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ucurbqij.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3bhxidaba.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3giflrqpe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kpbcnxjh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fuppfhla.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qdhvadnd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpyanyiz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3yquwkyhp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3csusyfap.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxpgxmau.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3sookxizv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kwzhkhgv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bbsnyoyv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3adqmebwa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arwkmnnp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nzpyausx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mhhycoex.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jpldkjhr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dwltgufa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nuwybwaw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3asgsdwhh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qtmaggqa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqazcdmc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rxoqhqqm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3uoleygul.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bhritimj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ofdhcvvv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dexzxzvh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jlwilpbv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qczsihru.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ypgaxrrq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3oscerlzi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ccsmtufz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3neisiinc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hsrsdrtk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xiycemcy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vyzfzwii.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3owoksewb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hxrzwcwo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3flbrdvun.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eryckkxu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqywotx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nelopmzi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3olxeuhio.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xhhkxcbp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zfildbtj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3poatxmfz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fpptluul.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rzycxvnx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rktnchle.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gldxqmxu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rmiwnumf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3danidlwn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xmtchcxr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xzyhmagk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pdeqvtri.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3sovemwdd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rvovloli.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vdhaysrn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zqmtshbp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mlxqlmfd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fdkexuoc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3aooykpxn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tfftmmhk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3anuvvjmv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nmseavgf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3sitpsudb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zalxwldz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzgwgrix.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdbbkulr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwtsswil.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cutmirji.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvdsqpto.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3evymqwml.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dztdksic.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ujmpaqht.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vfphjsxu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sxrioivi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kwoldvla.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zfpndpfl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pftiqzlk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fkdqwbvf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qcfpfeqr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hwbdmqjs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jogyxxfj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mlxifjnt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pvaavghy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fnboeazi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rasyyhaz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sajcbkyd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tstkazqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrxnctmi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ugessrtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxsstqzf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3cgssxbrd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3flhztyuw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aczivdta.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3zbzgcnos.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zvqlhikj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fpwjghvr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ujkjgvcz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ssapwdce.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jyhnscrr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bjlbhesl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vmmagrmo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3sbnpfzxl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dxcpcmjf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3osolgcix.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ewdgjefj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3oxhwblak.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qcgmzdif.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yrctekcm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hdrmsiwa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vaplxhel.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3inbiplvg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gfcmyzdh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lhqhbdog.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xmjibjwh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jjmkdpum.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nypsreqb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ffoigdui.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bdtufyfs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xjkvahuj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wqwznmif.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bdyneehx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mpjbwaws.html


<!-- 参考信息 -->