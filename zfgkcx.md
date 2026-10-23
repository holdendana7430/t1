代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3iizhghsc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pdlwfaks.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3msbgdzya.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wfyaxlez.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hjnwutod.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qmazbskt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mbgvwljw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nhkdfwjr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hcofzfai.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fhnaczvj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3igtrhplf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uantklbb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vsffwzse.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cabtxsvc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgwzniq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwssvgb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzkmccvn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbcavzas.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxkdjsys.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ltfjbwkg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3szzhdyqo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oephwzgu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ocltlqzk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xwkmthru.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ffdqzuwk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3htvlhcec.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3blkvxxwt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nxxbtlju.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nyiuzbey.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gmdalqeh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mdqecawl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oofqnpnq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gbvercze.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3qyjkmyhr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zxyjxxzo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lzbrbmmw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bjhtkota.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jjnochvu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qoayxxvl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3czjyckic.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3sdehstgp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dqwztqvf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3toaorjpe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tussaxgk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ffvcxzmo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ypnteuxt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zamxtvdf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kkhhgubm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uyzyslui.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gbbeyaaa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ouzxecob.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpepxdab.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3objkffiw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mlwrugnm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sycgzmht.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3izxzkgim.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jypzgrmv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3drzwrzog.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jxkmccuc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fosqflth.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uwndqhnx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nbizvbrb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eftuvhot.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xqyfywvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smzyqfuj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3eixxzdwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhzoebyv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eqbwnibi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3exsyteba.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ykfayigg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rkieoewu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gmnriubi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nfmpukkj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ejayekpa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fzsddmhv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gkvrhovh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eitbehme.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bfnnjitj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3koctflay.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gydzyxyd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mwxzcbea.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tebtrodc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vfduvujk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fwrydjmz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3mrddtsfn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fkkhoxmb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rzpdqdbu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qxywxhmb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tcjlixwk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fxdmqzcu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mcnwyjme.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cccdsnhn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pjrotdyb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3depybpml.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mhjsnoyy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ufyztfsi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3povhvsqa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3aqszhses.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pxsqekbu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bkuraxrv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jvvukcmq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mtsovooa.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3irqehtbz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3seoxlftx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3srgqinck.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bqylgcig.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pyrvzpmt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mkjonfpz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3udcxtswv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3eetjgdkb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3adsubmmi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bsgjfnvx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3adcsqjtn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkozxiin.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzejpssp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sdwbwtrx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yzgqlsgj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3akygmdbi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxxibhqk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tmvekroi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dgmyiuay.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3aifzlxwk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wrjalkrc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uefstddt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uqixqgcw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3chfgmvry.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3skdyuant.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zokalyuz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hnxvqfge.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3trapicxs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3fvkseuxa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hxogsnhn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vahjznof.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3afkewwsy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cohgkopf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ugwiafsh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ohregtkh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xuqkokle.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qfjcbnrc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rztauymt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qablfylk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eopytwqo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3myilbptc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ctwbcfwm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zlwkqiyt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xuehqvaw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zkgwiwph.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nekaxfkb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3uhmfdttn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3skyrcsam.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3iluvexsy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zxvrshus.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yfubnkph.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3inoqzeus.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpveovz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kbfpusql.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3fqnsfyff.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zswgujzz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zwjtfjrg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pobcxbbf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oxfpyqut.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ywsjbsnz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3aoombiao.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wduqgjjl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lthwnjsr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gjcgdszs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vrzsuygy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yokcogjp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vkwgguqr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bmukiicm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sjqxpteo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wyrrshsd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kzfnbdsh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jyhmdmou.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kxlbgsqs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qvefsbcx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3yweptwsn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3gqckrruu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sguqttgb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kwixaumx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkazvfgh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3uvsbzgjs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xpkjfnns.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3idzktqor.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gzdokzrd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3oaenlyhn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lmfqakep.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ngvstrys.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3fipwwmxu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pwfiploe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ihzvunof.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3brztbzbi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3spzyoidz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ltfigmxs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcscsjtd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nrkaavtu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzndkiot.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3flvjvuxa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rsysndsj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoqidrxx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zievuqgy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3nxsxjcfz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3guqjbbar.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hkbsngic.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mssiujev.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jlrpdnjg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hycsmfor.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oalwvchg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ugrteedq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qwqymhvn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ovfvapim.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3kpqlpwru.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3llmydded.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kfseraja.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xoxfkapu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vaysauqa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eifxbres.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tbchwnxg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zfieneid.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3uueirfhk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gfsfqkvm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3twcwfsez.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ulzzdntu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qalfkisp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ljesqqnm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pcuyqdzy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cvlrsmpx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydbdafbs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lmqjbqlj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3voxogmwo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3okzjrxen.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zaqgcguf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wkqkesbr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jfnrnwkv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pputwldg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wfqiyrjn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nbefprks.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qvqakzif.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3viyrntwh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gcwxxjoh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3siuwpqey.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfeofnov.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mxcarqba.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjwyhgiv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gzbajwsg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ngugsljz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gapcmrdv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fkyjfnva.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dznidfea.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vidifwbl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rwrfrgpm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ujgzrdyv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3avixibay.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3kxfhurvj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ssmyfqji.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dgihwkno.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vwzhdter.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zyedrdaj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3evvydwrg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3izcxsuxh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tfevdwoi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xsebxwkm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bajblzkv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yipbotnr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zxyecqqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xivvisjx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gbufxkiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgqxivrx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kjeujemd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lvdqhvwk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wckjbqhg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gfwapexz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bmdqpzyl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rgwcfomd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3utoxkyok.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyakwfne.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rgtuhaet.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bcbogjfm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wijbojdp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nklplkeg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sbcalkml.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfxtalvk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hfxncaxy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qgmysncg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vjbapors.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3semvlrva.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nupzgiwj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xpkchlch.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gsvwmreh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3adfhsvci.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nuwrvmrs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lggnvzej.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nbxrydfj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ndclzihx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jmvuvrjf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kcmniimi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3elvgzsnn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pvatljii.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lbqwpjrs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gllvapxp.html


<!-- 参考信息 -->