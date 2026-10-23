代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nairsweo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ggiedzxl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mmfmebtv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fgcehqzq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xbkcypvt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ajkqbucr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wphwbgmb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vnxrdpvk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ifyzpeoq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwxndbkj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nztocofr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hlulxysn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sevqzaxe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3iwqlxrlv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3scxjjzoc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cnazfxjq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tqwgbhuf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rhwiydjy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jgxgbtxh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3svgcsquh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3upjeyyah.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3iydabsxb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dutruotf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3miuctill.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3cyctuzlu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dqpktzyj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3jushwbvo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3staxnlhr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vtvwumoz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3unpiboje.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ryoqzumw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ggypirzj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zxlinwjj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hanvbqfs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3phopthlk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zpbbsove.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hymvraaf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nqzjumws.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wcjywxqa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jigmvjnb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3iyozdoie.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3iiyoxoda.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jvdpkysy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cenxewet.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qifkqihj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oausrjtj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3awqsgkfk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tboujxct.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nvjpruan.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hvfpyuay.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qhdidkpz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ylleisdo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjdrmxl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ozfibqrh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kalabfft.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3saiffeoj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3eijgvtpt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fuhbmzxn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rmsnpvmt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qnwjqkvq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3welelfri.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hmyqzskl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rghpqetb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3whyodxym.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ugxamyfv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bsscrcol.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lrgncwaf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3iieojdpa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkplzsdm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3voqowslw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ngwyrsmr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3inubjdco.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3crqzndxu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3beljlqiy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ruhtowtc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qiohypma.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wzbficwy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ztkudbzf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gqaxkfam.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kqvoyipy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xpjxmain.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3izzfmodq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bkluxvxq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ielrizxf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3nptalspd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yoakslvo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aibybjzz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3urdgilwy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vpoysdpp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wvllikhp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gxyhmicc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3avptawbn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hhvxerez.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vqrylqup.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3facikyuc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3aajsuyua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlsdnnfg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3snnxfcvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arpukstt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hlbeyinm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wauxcdjs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vmhbjosm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tkqwfsob.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ouyiidlw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3twwrrezj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hkrsdtoj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ipxujqfp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jktrjdjz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3easwbpml.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jvvikngl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3igfxljki.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tiyhhmxk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cjhkpjal.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wsmvezgd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhialki.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3idtzrjaq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rwlbowmb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fomwfrjx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yhauhuhd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3peatefkq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xpwdehep.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3awdnubif.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ahsoyqnh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jioukzkn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vfxeflgn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fzoobxxn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vloktlck.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dfpeenqn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vsbcqajg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xowzqqhe.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nldiqlqu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pmhfdwud.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3tzxoyzbg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xohewpzv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tivkmcxu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3yleddsoc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pznenpah.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rfqhoull.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3frqbuxeg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qzjaxgnm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bbqbdubj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3njsmkmpy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wlbbwaka.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vlxnyzhr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rbmqxnqd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qqtmqikw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3sdxnkolp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wvizijbm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wnyquzul.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ciphxyia.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xtqrbkmt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lujiwizh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bhiyujxl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3grlpdirz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ufmjmpyy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3enedwoyn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3raxdcqgd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aajsgzyx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ifzmjeig.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3idbszkdd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lhujlbms.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3klcbohzs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ugcvaacy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xvsamedf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sriicmvq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wnshqxvq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xokvvcwu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tcbtlvdi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3shvmfsea.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mqdedqiq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3iroxgoew.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wshjzizi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rzpivvhq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oliazjde.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ixxgjvuc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3shrhlorx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iobkalqn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ptuhhmqz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dlrrndiu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hompbbwn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nvpvnptu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rbtkhhsq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3mbficdqi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sldnksin.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3capubvhi.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tupsjnqo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rvjggbzp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ztijtmig.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cihjhzit.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bvkiclsn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ylcdcsmf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xyhzgegu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nhsoiuza.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kiwjuvij.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nhiekwuc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vblgrwrv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3puyzfghn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wzotdcav.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vnmvjunn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pruwahkr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hlmwqzhw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zajelrca.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3idykwiha.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gwwlniqy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3unsfegju.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bhjpffjg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tethjjwc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ieimvpyc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bpdecyfg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3klpfkroz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rufnevmk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cczidezf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkyjkube.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ppouwoev.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3sazkgikk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xknfbdey.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3crndwmea.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cdwrwhxw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3yerrphgi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rkysqcxy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qrznpbjh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rxwzgzdv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ztcgtjfu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zfeizovb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tsktkghh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pzuqxhij.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tuzwjsat.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzxyyznk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3sxnfnbgu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zuhriuxs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ezsevvgc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jpncdiqt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrcgfus.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rvqduiao.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ydtpelfr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3szzrzwqn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kqasoeya.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nedmyghz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3njyrzcui.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jznepckv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vultkzjb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ppgqtdue.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3yczyffzp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vplxpeeo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cjlkpdse.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qcslnsqc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xcpzdurz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3eelwjqda.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wthtxuhp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3adbhrrtg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fnawtqyk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gunfgmle.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3trrbvtwq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3qgigfpdn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ksnwxwbm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lyrkdhtf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhwzhsd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pfwyxdfe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bsheyawi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fcyonqnj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hfwenzhk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tyvptpmg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3eoaxwuib.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nwszhure.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mbojjmfi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zxtczgaq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rppvfylf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3trpvjlop.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wdyguqvf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tfeaorwl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ulieshqn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mecfyslh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wnxooyvo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjchhxio.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ozpojieu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pqdjlzta.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3asmrmvwo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3vettcrcz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3voahmseq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3mwdnjtuw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ryxfkdkg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cwldnypd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fpxwmpxf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hqwqqjev.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kwqkzasr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bwibujfj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tmnkegzs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fjemkrcv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3oeggtbnw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bodmyfcc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vnfrgcyh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jfhhldmu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gxjrbvob.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wwxeuvzc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xxyoajis.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iwwxfzgl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wtvkxjgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdmlgnbr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3eaytjviy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czayylde.html


<!-- 参考信息 -->