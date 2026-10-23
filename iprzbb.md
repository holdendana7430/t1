代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wnqaqrfj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ssbygqxt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3urmecisa.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cmknzewm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wrfzezmv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3glaxaxbt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ruzfzydw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bjmraagn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3elugpvly.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yamcavyl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3afyylski.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yxnkpmuv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3owninzuw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rnlrzpnv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kpujolww.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fkcezgyd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3shvikgee.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xenvaemk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wpjavuel.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qunaldss.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zgdotxrh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtopqflf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3embhcmdn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ciikvkto.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kpydcitr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dhkszdkr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3bjzotrkc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xtausuha.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dhexqmwx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3taledwnz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rgccxlcv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yzuxwmbg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3irluhkhg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dgbijlgu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3cgwkksto.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kuyngffg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vyswzmdv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mremixcu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uscmufpq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jwqtdnlz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3adtrmwzs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3auwysogp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zlllgwmr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vccpaicn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hqiyxjtm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lpgiqtsn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tpybkvak.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aqucjglg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3czzuzgmf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lbzpvbck.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lqykdzrh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lahqmgfn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3inepcnsx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3easctspu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3rnvtgety.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xvvxlvof.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tnwxgsfy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3amhasjes.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzforiut.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hdkopokv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwivftxq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yigoigkd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rhfvclui.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3htlrdzbf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3upvftoxs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3glfioxyk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nbijyvjh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vpgqtotm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ncxqabit.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dhrjmqgy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xkyjvqja.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ybdldkdd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bnwhderk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ddoujpen.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pcqcdcdi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rnwxjnqi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rpzmkpws.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3thgmvxqc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fvlmgyau.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jrvbbgix.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tlyzbsxc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gqdjhvel.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wkmlmqxy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lbrbmpyw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlaytgq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wjkfekak.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zdxfaqmz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3twcdmmdl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cqxnsehn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3knnkaftb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bhjhmsli.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3selxjoen.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ymmgjtit.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mmgekcvp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mipxsqyr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lbdnaqec.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qonmegat.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgdntpb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ggktnhuc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3djnoeszx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gvnvvquj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qfuvcctv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nwkysfpd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fpysenaz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ijpensqg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ptupcqdf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lrcuydxc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pssscigt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aiplxpze.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3aprpjyiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbfhoade.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gojqjurw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3emgxdxum.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wumucegw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xcakfcuc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3actblhih.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3filkkxez.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rfonjcji.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mbjqzumj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mjlnkxtd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lezvddct.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ijomrpfz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qzdilaos.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uaqluqzz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3axhxvnhu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zahkvmwv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ddymmmns.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3laqoihbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mavmpvcv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aodwxtpv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xitihoha.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wyodgbjl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3essxzwwu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bxucrlbq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tarehrgo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yfwolrqh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hxdmnkul.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ojfqfiju.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kqwcitev.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3agihqgoe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3akznetes.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rqoplilb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cbiylqii.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dcdkpvmr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nhupezdi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lqpumprk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gayjlilx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fwvugedp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kuuegbav.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fmjqsxha.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rikdxroz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hftnpepd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rpcdcqnt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ldnxovnl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dhyrpypw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kpazmsbk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wekwptqa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rpganlps.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3opauivjn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ensbhcap.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cgtkgteu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tnaitrlo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wpmkfonp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vydunegx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qlzpztld.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tjljidbz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pjlmicbn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mfvnddtr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhqtuyz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hkebmpsl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lbvmpsjb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mkwfydef.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3byhxykqk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vgbsolec.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3uwkyqtko.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jlvvtzvy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3alaaifae.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3idtezmbl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bllweuqs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lzwwbuqo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ebtndnno.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mgrszttn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kfwxvmeo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3glfjlypp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3twpcecvq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bswvkdxf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzrmstyx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lnjzjoyw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3koxnfcvx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cnriccep.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hpfsakbe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3slhxufvr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ifhkqgye.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nltudocc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lvaddaib.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qdnssewi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jgbbarth.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpnopia.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tbkgjpzf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pcxfrzfy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dwnpmrpi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rsgnxhmn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zwcyunxm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xmawtclg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3radvcspm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kuhigjxg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vqskfjhs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fdwxcrkm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3riaopjcc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lyhlivyn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jgvodnlp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3abtrcopw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3eejzfogo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kbvdvuzp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xykfntrs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hizwxsdy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gjmuahwu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3buivfnib.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vvhjbvmq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tryrjygm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3jegvswvh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlzuhjkr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jvevbznf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ittwgmjg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dalbtjyr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wvutuoul.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pbgbhxsp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vidqlalt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3odhzbtnf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ghqiksmg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhzqynxg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zkjzkbad.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jibescdd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nfkohluv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3oadxipec.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xmrptwbx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3izelgsbk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3uluhocrk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jvxrvkuz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mjbzcfqn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yertkeoc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3addxjeso.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3hcuspjbr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3synoppwz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bhqljtdf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eajyhzbp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mhryltnw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jtyhcjqa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wpkqucds.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fjpzaywb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lzrukhwl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gjjgtezl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3anhhddkk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3louqxnbz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hohrxzxb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3uxtittbm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dcztsvhs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vpvevvjz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3phaipjpk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rjycickm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzvjovjx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xeivnlgx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ehbmlyum.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3bodnylci.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3nwqepvpn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hijxpmbd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3foygdjdj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ktoqfuch.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3idmjtrny.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gbwmmesh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nuosmbdg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uoxdmvtr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ixvqbjhm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cumvssxz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vxtsqild.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihjdrint.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pzpetgao.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ovdndsgp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tfxaywwj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bjtxbwbb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3rodjazdg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3uxnirnux.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3knodomow.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3phuelgcy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qhxzyius.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ymizdsql.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3obrabjny.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ozhbcwap.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wvbngxnv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xgxiqjjv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3knsilgbm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3elgihdoq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xbtdibzu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mqlzrafr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3phrhgfge.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dmjnfuos.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3joqzajak.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kbtsqflc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lkgjfzmp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pmzusung.html


<!-- 参考信息 -->