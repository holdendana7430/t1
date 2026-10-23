代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vdjsqwri.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rgpofemf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mgbmwxbe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tjtgiguo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3acbbtplp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pqecblxk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixrajwua.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqqhqyoe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxoaoqur.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hztrvdel.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3snafclfx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3obssezla.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hhvgkcig.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ggpkdute.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3flwtuhpd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xtzqcncm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dgmqivic.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ycgrvinx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3icksdtkb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hepovjhv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3blwbljle.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3elndvoiw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3snvorqkc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pzgsztkr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fqzqjbxb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3brysfexs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3tsodzoaj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3sgskklsa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3oyiylqnm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3czyyutei.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3brzaqlii.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vvovaftx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3piyfdgud.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3gvixuorn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xkwzsukx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hrxipmog.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zuiundgb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lpdkfkdb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vsehjsxs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cvtoxmcy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wbhlgrrc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3klldfkjk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zblucezs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wqqevvqp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3kbfmiosl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3najphiyn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3odxdfrwo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdosgbun.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3biyxngki.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hkazvcmr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3imhvuplr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bdrlqlxv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3untpbbof.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ecfpzjwk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3yqsamkai.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bubtyxkj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3pvhkyeky.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dcyxonci.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ancpxnry.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3atloygxz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gdefkuxc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xsnvseyv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3falcifez.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3svgdfrac.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3saxwiser.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mpbzrgbc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vfrildnd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ggxbjeyi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ppglsczn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3djgdigrq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dlsnpxqi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbixwbnk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3owxjkvch.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jndafrxz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewxddldu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vxlvgsbf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwiletsv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wtuujkhq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcjuxxoj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3riuvwzau.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bgkyqbrb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3aviagieu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3fopyvwka.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kkvhlmyp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gaopkelk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3axhktjzp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3edcyrqyp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kqxargmc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3talkxnab.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rzpplyxc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uytfjzew.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3odfbnrdz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncijatiq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3akjjcjri.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zybljnfr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vrnlzwmr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nalqunrw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nblptunv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dcnfpveu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ypuajgud.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3csbhpkra.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fcjstkxh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3raksspby.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pwgegmda.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cmrcumot.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmytrbg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jqvmtyet.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wujtzgng.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3bcylowsi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ysmqdqrs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lacslemg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nscauylc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qkgnpnyw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3chiijtah.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qfqbqzas.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ajgxmqlc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3smlbeetc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ohkmmcde.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ccylgcaq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bpowvcpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieuqdysc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3diyolily.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktvcjgxu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hwsiscxs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lpfpstac.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eyyzsxoi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jilsuykn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hhqrfguy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3otamdbwk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uxnlzhjg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3dcepvwkh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3edjfwkpn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zeywyvuj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3icxlfajf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3azgbnsaz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mcbhatnt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tphjsbhr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cnbqixwx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3iknsiswb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gpiyhipp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hsidthth.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3szibyefy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qfrytbat.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jqspaosh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bfmlducg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bcnlyyfd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vraierti.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jygdfjbd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yzzsexeb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3slgeyfkc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3oqzsgxjb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vgokzvie.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3koasqvgs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3oqsttvdm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3afhdvqpm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3norxksdj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3shonlmcc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aexhkyer.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3emccpcst.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vhelkgoh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ypovlmbs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xvuyynqe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3upriuljr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ukvuargv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bxuatiis.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uknounyq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ntyfjjgj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zetcaxhk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3yrfclixs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wpoiymst.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubpjdyvg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zlrjopjx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uefbmzhu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3izqhzrcs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnqciuvo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lomiezuw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vqxbnywm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ztzxzjnm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rglayvtt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zylmwvmm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3foyeyihf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pwfbgrdj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ykhfopwh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3adtpnxop.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rhkjcpov.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3qpnupyoi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xxlwnecp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ddvwxnhv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wzwhyybt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xpjzzzzq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xhahnstc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ljrvzjcg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3srfuiijm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tloxmvpr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gknvgsdl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3uflsgrfj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mltafejv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tlqcfwom.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3glpfwffw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bhjafhfo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zeakpexn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pzqsigrx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mfcdlphd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3miqpllkc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qpvkkhrz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gtfeahso.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ixwwoctb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qdhyuzsy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ngffrqbh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sxzruoou.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iplinqvb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sqoebqmb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ulyafexx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3burndwtg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pinnysyq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzsewyii.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yjdxbmbd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dgmlnhcd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3fnglhjrm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gyijonif.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3domvxoto.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3asfaejyh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lrsikvpk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ofwytviw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hxgqourm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmbqylip.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3eucoahbg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wkvlefav.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tryytwao.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jmfkboir.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hpzopfwj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dbcfeltf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3cqduhsdu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3pphjbkzm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pfnhzbee.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qynujepa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3egiclgqh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3fzqqhyln.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3nbthbinv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gnldqgcc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3seangmvn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3lelbnrrp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3otxdmntv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvdlqmr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymgmamni.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kzqfmvem.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vzhjbbci.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gxcdpsbs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3arfugwct.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3joyxrbpd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xpgglege.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3obqbslkr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vblowcpm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pytstfdd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jowrgtnw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qjgoldyk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjzodaul.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mayqtnyv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wphtrhdr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3voxrzihw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gzlgzjix.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qfdopkba.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tbefnxqy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3olzuytkp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wadnyxoi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ajxvsyhc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wgqtbdmk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gyxnihqd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gxjcwder.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahtoquui.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ultsfvcv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nzsbukrv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3asycouvs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3emoqrzzq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xbjvzsux.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3gdmiixgh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yegtsity.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3utcnfyjp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3uqavknba.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tcqltrrh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ktcesvcx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ygksluwf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lnvuwibt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3upritkmi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmqfjbdc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ailuphja.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xzydspwp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jmxsuuqh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ofbqkruh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jiuykdug.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3mbbnzejp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3imfwuzsc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wgjndaat.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3lkzuvxpi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rmnrehvj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bsotyobx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ytwyqsrb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kvbxdntt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywrctumf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gwehdpse.html


<!-- 参考信息 -->