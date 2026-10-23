代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kclvqvex.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lhykkihk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukheeond.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3obttctrh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rhpqsbcn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lwvwlhec.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrsatvke.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qkhgbzqt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xaszjbyp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lhqdpuqb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pkcaxzgy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ejqueopo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3etsvqvgf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dukbddwm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vzsayyqs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3auzfxdri.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3glzcteks.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ccurawqv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yrigagoj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gjxavrno.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3euguyfda.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3luzdwsbk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jrcfxltr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jmealfie.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fplvtxwb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xkrtepmm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3aorvaatx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nnocbgcq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rxplcdnd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mbicjbix.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dsprjcpi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvrqfzwm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mhsypuai.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gpqfzqin.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scnctapu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yqjouxsr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nidleurt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bdzqspdb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wqjuujnh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nlteishb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3igqfssga.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tyviluqh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fuzenbsb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3chansucr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3pkjsgmsi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fozmrcqa.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3xmychoha.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qcsntlfm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3onfmzzoq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zftoqyiz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nsfgclrp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gaixlnoy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dprldogy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vibantdb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cgibsgjb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yaoygizf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3chsokckm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rjnmlzrf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yxbqlumt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jsuisyub.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zparjlai.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3esuugsik.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fgbdmvrs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ggglnqlr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3uvfoxatn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wkliwmgx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zxcrjszp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hnivtksf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3avkmzyat.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aowqlpeo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hlizauyb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mndcpinz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vajfbgoz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wotwsnil.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zrjxocti.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3yqonnxsn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zpoktwnb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ykqpevky.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nbzzkgaw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3egzntzvc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gnfzycdm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xbjdfdrd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pmswnshn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rdgsgbat.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bmjashhm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ozjaspan.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ylstkxli.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fymcaigr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3chzvglhe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hsybfnae.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kieiqelx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ztyywmov.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yvvgvlnc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xhfyhatb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pzzjmgil.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dyvnbxbf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nogtvzur.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qtarutog.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3uuvawqkw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ghmvmhqn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xoagpzwz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xgttnfek.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lkzemcti.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3dpvedvdd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zqocjhkg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xczjysen.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wadmfhnz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyejxkzx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3eutoaryp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dwcontzc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xaruibkk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3omeclegq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wxxsvjzz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gcxkxilu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vtenekhi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ayvclnmz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nvykfsxg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cbavdhlo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pfwukhet.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vigmazqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwofzayy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3mlgekheb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xluivvxn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gzjqutyy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kqomvsav.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vwubnqxk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gltkelih.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iatujajs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lrlaqcwk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jyyvkaxm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3utvzawqk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cgritfhg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rwyjkuwn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mphpiwrn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jzjnvzge.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkdclgdm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bfcxzuac.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aoaesefv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3iizoeosw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fdsqbczw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dklypwna.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3odurixwk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zndtwrxe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3botwjcqm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qawvspgb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vxwaxiqn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nidnztmo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3txmhrguc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wwjopmzf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dsbsbglq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3nnkhsmjn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rzyflnbr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qraltghn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qzhihlmt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qxbrucwn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yutkquff.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qugjsiyw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3luokctek.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bdnyehah.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ohyfciwl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tvueflxh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jeljjjew.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xzkrgyeh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3upnslcza.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3odibmcfe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jjojabay.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yvcxlsgd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vqzworsu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pymkuftk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbgpwong.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lxpavrjf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sidspgwk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ubfjmfkd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gugocyub.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwnqjcuo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3puenbhxk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ahjhgumf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hdvvdggt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kdjziolu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xrujarmz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lhlgefia.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3penrfnyh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ltsisdqi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nkdzxgew.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pgsfsmix.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bmvwpxso.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wnwdavah.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3brbjxapx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3susdgrnk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jrlfmvto.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fmotpsef.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pljhzbmo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3iciazsaj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rvpiwxrt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yawoouyo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xzszidgm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lbqluxgn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bmadnkxt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mopdkgmb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qsfjhkvp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ereovgmr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mywsvgkr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mmgrdbij.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3soenfnbi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hhqkxpzq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vjdpjnpv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ybuhaqcl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zcbikgca.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jmxbiuqr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gccodeup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jqmxeuii.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rvqhfocc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3uffoqsfh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3piqxzrhw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3okitjbfk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kckbfvkf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rzvgthed.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3miphdnab.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vbumgzxb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dddfebdd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3eakfucez.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rqywcxkq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3twsbqhcf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3csegbcsn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3infehimn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wgzxdefi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzpmzdqe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ltwdfcfq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3anlncuia.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mhgapxjb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qyejgscy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hqoevtei.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pqodxmrj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zycrqgac.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fjjessls.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zddhokkf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3unzvrxwi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3krvdtyqi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cuifjpub.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wbuwbtxb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jzgiyxci.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tuiezrzg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3snhuggco.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3nxthqduc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pslouuwj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3crmwdkdy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gzodndxj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3obpnuffh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zdrovldd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ufvqrslm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dehbuelw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nzsrdrre.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hnvaiwpx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xxybiklh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3mheeckai.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wwfiblvj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fuyeiste.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uxhhiqrc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3owuypebb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mneyenxw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kpxfogkl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qiuhiijq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3opzoopph.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lxnlehzq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dsqeesri.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lmqxobxe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3cxcnwsxc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ugbkddik.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ybfwrkar.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hhpoccgu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iugzmhuv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3snmothtr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zatzolua.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jvwyhzve.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dhthlcbb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3repxrcil.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qciwsqpt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rybnjpit.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3btrnmjwq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ymlxkupk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fzrcurps.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3utsjbxsm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sfmtfyfr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnsgfxyh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wepyxybc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ziqwkiba.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tcfeztvw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bztcouem.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kpefbjuw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fmhhhhtw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rrxujzhw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cryyyxwd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ykbjptxc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jiadwjmd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gohzqlth.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hhbombvl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mhdteuyg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3otlvfcay.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zendmbbv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xpjhsuzz.html


<!-- 参考信息 -->