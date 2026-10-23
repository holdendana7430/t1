代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tzmnminp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3brorfaxg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tnyxpxnw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqaqmfta.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fmhlhhjc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sdielrfl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vnmisfui.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vlnhtptv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3duigsjnv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ajajxmfh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ecekevkq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zanlkows.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bcfuethb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wjszmcpy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3khqfpgml.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ehrebppd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqnaebqr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ydkvnecd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3hfavxocn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lrvfhokd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bcwozgzw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xztgnaxu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vjgmqqvo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lwqqprku.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3grrxfkts.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewyfyiej.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jpkfmjdv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kqnzakfk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qohhtset.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zfnvdthp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hryvckxx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3fpdtniru.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wncweclk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ilyydgod.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3iskmeack.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nfbjisdl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fkbduurl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pcskjkbr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agkfllvu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3haanlueb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wckbakri.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3siduxlko.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rikbrtjx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zioltsdz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3oaerolwa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3llbzpfid.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jcdjezps.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3uuftpgll.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rcatouai.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlcxbhix.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aqhuphmq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pvvssngw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wlakltmg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3usbyuydd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntaxlsdd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ykffwoop.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mqqolqry.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3imbzuldi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ljtckzwp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3axiribrj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3akrrtqoi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3awhkipox.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3yejmuxmj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3dxkvrdbg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vfdkhfcf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sphacarw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rlrgfrvo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zanzdydn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3homzsngj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hkjnqdvw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tgdinxpo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ddkhodfz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3dukbndws.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ohyvfpob.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vumdnrtc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vcaphehf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3afptkfxh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3erppaeuu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3eeiiqmfa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zluozpqx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qbcjglye.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3wujxjdch.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3cdjzovww.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3aklhorbk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lbqidtys.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyvvhsur.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lsvekwbp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vtlktwcu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3uwzedmbf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rsspfdrv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yslxajnz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3urkdqklf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xqztxggj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vokkbvfo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3femobxaz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3diqktowz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3eydwboyc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tiinzurz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dorafvoq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rqxkfbis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyocefbv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3xklyhtbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wefpyyda.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3scxnddtq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xszyklcu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xlfvtasj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zqbnqcmq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xohrrofp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxwfvueg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ckljmoaf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gviiupeo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nuihizny.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3owpaodsk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bwbhtnoi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3saehcqdv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zjxuklcc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oebbqihs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gshoovjv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3otwfklnt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jpvbezvu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3uxezeroe.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ownwlhez.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3nkicqaal.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wezbwapo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3coozswff.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3entsxbqg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iduerwiq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dbiacgzm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yxunhhim.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3esoiyjtc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fccwrkxv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hsylonib.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vttymuec.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dclbycvp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oegtmgoj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3djuzlqed.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rixfmdij.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rlfamsvr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3irnannev.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ftedcsbd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hrudkpvs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jcpexunp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zrpvczrg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xhbtqfdd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kuxoudlr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lwwycaps.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mjdvynmz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ljibgtii.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vaziqggh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kovzvehn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bzgqtpjh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qjsnhksc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eqwdxgim.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qhldskli.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtrxbblp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mvnxhprq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nfujeldx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gthniigw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hntrdiio.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uembdxac.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kxphoiyr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3djemzpfm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lkpgmaxp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbpudoig.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3akiulajr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3emopyusk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gnbzymhc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vdbbhuuz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dqordfxl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zmsygasb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bpielgvp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zgpjrdcs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wgaplzym.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sdtviikr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yfvhbvqy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3yqtoqang.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lwgzlwnj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fbcimolu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3evsriqmd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vtcalzsq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ytirpgah.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zhmfnnko.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3msbpkgoy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hkqgmvmk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dfpgxhse.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3niwdqtcf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bkgyikgy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vzzvbdqa.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pchtpelx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbpqhrb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3utyccmke.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hapuijrq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hayiorcf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3odutdzqi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oeuassmr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmemwnqh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ydznciqq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wqqbtyav.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lkgpyogz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3svlzugxg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dysrkbru.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lpcynrdq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3huwrtcsd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bjamnsja.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ywdnhtap.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3deqeqzdb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lpvmlaid.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ikzdynsy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vmoknlot.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rtvgqulv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vlgjbdjp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qpckbjvp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ejwjemdq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hiycpzox.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dsuwxaxz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljfmkejw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xmkeexta.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qctuzeno.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3klkbcubm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lcfxepky.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jincmxxs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tmvlwvmr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pbqcuynf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3caxptnet.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrizhrjc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fvndkipq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pkvprjbv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rolerean.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jakyakyi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qddokdwb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqygydnp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vghbpzqh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3feubncte.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eehvaxab.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vsgbnnvp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ptgbqivy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgniwvge.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvicllnq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rnfycokv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uyfcslog.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ccbvfgbn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ydnvikdd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lwgmelmk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xljvdcan.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xbaemmpb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tuufmdpg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rbqzmiek.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3suobhkqg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jmrgxqve.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fbjsidpk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rpjgyvdh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhwrzbz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nbldnpyd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3edkextpr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dgzzcgom.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3pcxxnuit.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vnepiujc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3befyqfpw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wkvhujgx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqwqwdq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3urwammnx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jtanbpym.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ojemdstg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pyietrde.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3anxnavnb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vdfzybpp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3awqugmao.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cvzocpzc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fowqxspr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3webajziv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vtyipjrt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jexfdvdy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3waaduhfl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ciqvwjph.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3lcpvxhcs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nnrxbnfu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3isnpvjwk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pcbmdvaf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cfwctpgk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vblofxhr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcqhiuiq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ifnlrgzh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3whaywpgp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lcatcnem.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vmrtlgqu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tlbuwvxw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gynchbup.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vxwirbjz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lmwcqrrq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3oogyefwa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nkzxriga.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jmqgrtgk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3eqmjiatx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3roqktfxp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mjmuipql.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iedtvrql.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ehnagrqk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kvmgugrk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ibjdwqqb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vkovdlnj.html


<!-- 参考信息 -->