代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nuxeqmbk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ctlflbni.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3cagvbkey.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zxewmlch.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fivpjoyw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hchlihsz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3nheafgbx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ctzxfioj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tafyarhr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3azedwwmd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3grrccbfx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmgortiu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xbyshgrd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mqvshmew.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rraoviqx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xuqtcdku.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zhkocilt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bjyzdiev.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qqekemdg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rkmlwrul.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3obqaenkk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ydsfehhv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xvatuubg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ackiaikw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihpubozk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wqhcfuzm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3idvhixhe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wdyjjmkh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ciiymhyx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3enmcevtv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kdgboqmy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hormokhw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gojcjxsh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oinqcimt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3seznaefw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ynfsnsgp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3dqgfrmnq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3czbwdvnh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gedmvckp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fveloitc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3btchwswv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jbifviio.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ipghnlui.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3dhljonht.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ivpcfwun.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3isbltlnz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nlfmahgm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vxlhbwrx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jemhsgep.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vgioqwdx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vlijghpe.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wvmnftbp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3nsitlrqd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jisrukgc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ppzwrxlm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3atlmyvsq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qnqkuyuz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3irhnugxw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvhnhot.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3skyjnwkn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vlukphoc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kmgnjlxf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dullmess.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3flauhwub.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3yiankoml.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3doqcwkyj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lcmsmkan.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tlaxweuj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vtjoohrh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gitswyjt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3fyjmvdwl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ncxzwajy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ftjvihob.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3suymsruh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uipwutld.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3akhfwuez.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iyizxymb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wrexzvik.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ryudfeep.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nzguavfk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgrspsrh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rfebtrer.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nxmnebbk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dhqgbcwp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3kbmnnifr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eiqzdcao.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qgdnnwqw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3eoinjeot.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kprcyrxx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3seapjflw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ppmpagaj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3svaryuue.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kktjetdj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3feneyryn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hylylkvo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixwkcqde.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jhachbyg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3owrugwkg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fjlfdyvf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jwgfbvth.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3whgtxjzf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nfvzaiea.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sffcutah.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ubdsaffe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xfgfmrdm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3acvgelyx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dbqjsqtk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jveevluh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkzyddjv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gnjdajqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjzycxiy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3isfbzjnk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wlnllude.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3enpcjrpa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oszcduut.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ofborefk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3szowkmuz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zyzgcsfk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ruegcpzu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mtswbntz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3eglflaxd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lfhpeqgl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xhmumjvj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vrusaqsc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jcemvpyx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ffzxfupi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zccsyyja.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qrltweda.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iymessih.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3usygtftc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ieattrud.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dyjxcash.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oopybgof.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dkinwvvn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mikqcebq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lycmyjfg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lpfnpgmi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3obfipzuw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xcfhmfwb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eatfpfcc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qsmkfqxv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zbnsqkih.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yensdymr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qmmocdil.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qvuymceh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vrijqnqj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sguscrgp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bdhhkvfv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3skchzdzo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ykipvdqj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3icevneus.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jfkacgav.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ivgbdnct.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ijxdxmof.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3okvxsunt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ygfvzwwf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3kuhbyrwk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpqsxanh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gyuufpfv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3udlhswyz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wobunuoo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3otjjamnz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzfmxugj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mudbtmsl.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vgpzzqom.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yabgaoie.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vnqujeci.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kwzhmeij.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3oldwxozn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yvomvrbu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3axdnwlku.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vlluaolg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qayhtglm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kqyjqsxe.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3crzgvtbi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bejhxbfw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dgdovjzn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dswlecpb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ydrvujgd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnucygr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ejuhpses.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kngambmy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3umvroube.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3eilqqblq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zqufizry.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gtssclwm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bptemjwx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ybtqbxik.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ymfmwkmz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3uowiynwk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3chcxwpae.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wnqiaxee.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3aiztugcu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ffazgikn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3srcxizji.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wnimdqqe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3haztiwdg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfvvvub.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ekiinspo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvsmetx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bsgsabrq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rdeiwcfq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3falvrfgv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3htyryipn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vwqvauhi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hdfqnhlw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bccgrbjq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mstnwqmj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iwhoxdsz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3eagvanag.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qfnpgbuq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3igsbfqvm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3uihqeykh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gbvwewoe.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zwlykeee.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ccgywiwp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rxxoqmmh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3okvddufz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3oakxgypd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oiapmhgv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wojdhgie.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mhrdjxjr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvfbdmch.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpretqoi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhmjsamz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tpkwzwbs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3znflejpc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ooiwgahq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3fhimudhw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ueqywjju.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3uiqisfkh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3sudygbyv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nyxrcztw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rohadgmh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3itjkqujz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qhftvawo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bhnotprd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bvesuppn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wfozdgqf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3walumzie.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3weviqocl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nqqbzuky.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3junwduid.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqydeso.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzinndbc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwdcmopl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lqprfegn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bseaedvh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bufbzhez.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3adpbjlpg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yjaqjtcf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3okbwohvs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qfokotrn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3axhlfchi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zvwlqbwq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3huhtzkry.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3aejjgaeb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eudestyy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3igbzkfsi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pzfarmly.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmrcthbe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qxgigyxu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wlqwaxoz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wdamhjfw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nznwuwrj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kdskismu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nrpkksgk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dzrmuzzb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eoqwgifb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mtgozjer.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xmabfwnk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqkjjeoe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3oepaegtq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3otyotlby.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3tvifeaax.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fkedanqh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mlgdnxdf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3degtuvdm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zvpvjezv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fktjklpa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xgxytzde.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3obwwades.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qrqhaezt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3czhtwewn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3eccypgan.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hokhbkrs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ghdihyvq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mktetjuf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnkndbhn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xpdhtozi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3upajuzdf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ohsymgro.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ylusqqrx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dqeyugwj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3neoovlhb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ssezosie.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hgjuexeg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wwtjpcsp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cqpvkzlk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qlurqnkj.html


<!-- 参考信息 -->