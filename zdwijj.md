代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3syrvescq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qmequnea.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nyadzomk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3smtpgivy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gtejjhsj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dfgeplpy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3klypqoep.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mrkxdmxy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pbnbdcdr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nwpyiswy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ihnkitwl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fpjkfycb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3alndijym.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rjnkeacy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hxiphkdj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgsnhckc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3phovobwe.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umhqapek.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3piyuehoe.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3stgntezd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqrkqvuk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rzckejph.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3auzuwtnv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3dprlozun.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3chmdrfiw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhcjlak.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ylunpoik.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wkamizyc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3hoxrospa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rrskormm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tlewosml.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gcmtnekn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3exqnwezy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrqqzel.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jeajnxkk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gsxevfje.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kojpcwlm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fefrnuhq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qwmdrzdk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gxoitjgr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ctawbyoh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hgukfxvw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3avdyjydu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pfipckoc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vuihkppa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gbgjkyfg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qaelkeyw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3byffmicc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wertlfsk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxojapjj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zggavivj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cuyvmgzd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3chshtcdw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjgayxvh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fwovoqie.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3sftrjhps.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jjpbhled.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jqujajri.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cyckvmxa.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yoprravm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cqkospwv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3sthkpzfl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3igtqtgfu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3whyfnjjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egjxcwed.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wllwcozb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hupberfz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hurxplhy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3roescrpd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zzgjukug.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rzfhmgai.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ihruzlhm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3djegpeqy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bwniwewr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nfbxaazf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gvvtklqx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lulpajqk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qmqfjupn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qyzxlwzm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vvkqexbg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mfmpoluy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hyqtkesp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzxgtva.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vsvghiws.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jshwycqy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xbuhxqqj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hllftoxo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jiuxunsv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3npblzszo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ccqivcoe.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3etvhntig.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wdywuaoq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xtglnhse.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3lazcmlqo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gaseymyn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nnjrdlez.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qwwzozbm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vdqvziyx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qfgbmgnf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hphuklll.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ibcekggb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3micmocmr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qlpzzhna.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3maaiyrza.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gerrnkrd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fpaikopl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3utbcxmrg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vvzrksqf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wrugygeu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3foltmelm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3brwnznto.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jwuiythp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3injdtmit.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qwjhksmz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhtjtxcx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3msocwmzb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sllkvvoe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fxjzjegk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jxfvknms.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wlfotczi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nlrlcubw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3gjspdugn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hnumwbqa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ulkfrhnk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eoazrwzh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gdcejmwe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xjmqhpyd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rizodsdp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3owozmapi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ttuzbqmz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qhoekcwf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dfsekmhn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mrbbtqgr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qgkibzod.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kjswxjxc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yzvsonpn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bgehgmzc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3msodajfg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oqudisaa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nheimuke.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kzllsnrc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3audhmnvb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3neegwhbx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3crhdtijg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pwisrgkc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ycjrxwti.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lqleyoaa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tfskpffx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3waggibct.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yljeqvum.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rycjevob.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3blipdtbt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fdjcocym.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aigvhflv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xtdoghon.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmvaklp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xstavtjy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fndkgbzo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gqdiyaqx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pjefqqid.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vmqmpuzi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xbpvqhag.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kxxpbjhk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rxutbfty.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kuzayakn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3omntssoq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tgfbonvc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lhhmediw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3eusmjtgw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3frcwolda.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3eulawpqh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bhoybczj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gjctmahd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fdchsgeh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3elianhlt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zyblixbn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xvuylrtf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qpecvdfa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3roqoymtm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3myfzlfvu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fjjqsnxt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3biifikxt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3cvzibovk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xwihgvnd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cbjvblwv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hemcjzyz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lapmxpuz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3yrhburvj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3isrmryfp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ydrcfzxe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lofbtkue.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hxrxuxfz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pydupqgm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lyadkaan.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgszlcg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgqjxduk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijcqgdrz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3egfuxbep.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qqpsqcwe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rnftyymf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kijdfxuy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dszhjrtt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wpwrzhlj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jbschoen.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rhvjpgwh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ufjytbcp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ynpnszkn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bvybcpwp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xavseify.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ruzthoyc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3pkvnxfma.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cxcurrxj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yiqfowiy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cgmgzsbr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zwqxgwxz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3osvpxuuh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3difilxfp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ygxhwlte.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yhlvzhwy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3voucoqml.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yydqotaf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pmaaanpb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qovtmwsi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3scddjdal.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3avlaznoc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tkqpyiya.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3opuwvulh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3egluuynj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3msytuugk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zkessalm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pbyrabzp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sazpnrqw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nmaqdwxm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3otymblkd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3srsgxdsu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kfptfwcx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3uyelhscn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xymfqxiv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gpgafebp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3dqmufyvt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3nxshydpg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymduymdk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3rbdjgunf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pdcxrwyw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jeynjhra.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3weyfodpi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyxlwflr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3epoolkzs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ihxcpcvq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dbvuqtok.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mpfjaixq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gsvzvyoq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bliwwwme.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3clndjdve.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gvccaqwh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pdxlfzdi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3xzsxhamk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nibcyjhc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jxteevhn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3plpijtdg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3htexllvd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xmcnekjj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xgvtnhlo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jqzwdbxs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uiltheag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbdhxsek.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3zwhwsfzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfybkalx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mosancal.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ppjbtgng.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ljmobdiv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wddzgrlw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zcjpewgd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yzmjbqmc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3cevovavj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ricmuubp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3utnpkvyj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qurxnhlk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yrxxjrzg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uetylsax.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnanbami.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqurvkfo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sjfpylnp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ivtyhfar.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hqjawnqo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3bycdbzun.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qqjsdsty.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jtrdiltk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xxirauqe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ppvfoiqw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3spwqfwvi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ybozndae.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3svyrhqfp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3azgwqwhp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3egbzujax.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkmftpxi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ukwltltc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hmdlsyrn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rsfeonhs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hmpwjymc.html


<!-- 参考信息 -->