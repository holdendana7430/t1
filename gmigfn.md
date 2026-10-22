代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2flwzwbup.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tarbfqhf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mvfrulfq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2khwuzrmy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oahqldhr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gcoiwoih.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hrwgacwu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gcpjuvbz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2doemfbly.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iioxnjjz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eeqjypiq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2akkykbfs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2yzzkuuxx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mddpujlv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mxllorov.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2aelasslx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xgbexdzl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dmibbfjm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lhmjkmda.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fhhbjrmj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2uqbvdttb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mswblztt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kgxiwabg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsbajjit.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2oqpcthbn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gredlnqo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2guopgbtl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tumlarmr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oueystgy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xduuhcze.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2koqbgnhb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hjbtyzsi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wfjzeuxu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zwuqarsz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mxskblyz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ulqijccv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dmfcozxi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xgyuhnzg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qirqajxt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tbeusddd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ceqcphda.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nlgscijs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qjngnepb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhbxreaw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2maatazvw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlfkvsjh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2udjaoszg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2vzawaywc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jrpjhebb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yjrjszxu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2wounramg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bohqqtaz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nkwjcerm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2htllzcbo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rodphful.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cttzxfzz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jpeoffeq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2opartprd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cajjuszv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uirmbswu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yhhjnaok.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnkzxbxf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qoqgabbe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nrumfkls.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2prmrmlcy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tjcndovr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ymuemesv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pkgjfbrc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dbguumks.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pzlbyzoq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nhhagben.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zlkwrqkw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2axykfdky.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qvaejtld.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hekyjdro.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xsunlejj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2snpmlpcd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nzfhbxzt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2afqghxwr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2edgstdhe.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gzyeedkc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jndxwvko.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2miodnstx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hjejazcz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhokpzg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtvftsb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kalofmvv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2jlncgbsy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2skoqzqku.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2yxxzqgci.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zycgpmjr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2emeqcigq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcgzsiel.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zqqyxzeu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xqwojwkc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hnadijml.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nrwlalto.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2zdpvpovf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2iwliznuk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kmselwxj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gkzcnjlg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2krwakkbx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dqqpwmua.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2rdynshlh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjzuxmk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vqdmjyue.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wylfqpie.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hjimovha.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vfffmdsx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ejxphjuy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cosolkgi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ayujtfki.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2zgtvejmv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wwhpjnco.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jvwpvamm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2seacwyfu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iqzxikrq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ifuxtmid.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lrktquyh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gjmdzmww.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jirxltrg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnoidnde.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ulunheho.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wislyhcq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wumzfzhy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwjjshly.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xeyjaprx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tbafrpci.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lfnglarz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2plpdgiys.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jikyrbui.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yxcnrvvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmaydxmv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hvtgispb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yknimstw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pnwidlye.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bbvokjeg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nauezeyp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xvnblkle.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yiycqvmc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rxuclvni.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2moxcevoa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2anlkhluf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tfeudnev.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xudvisxh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hedzybgp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wutlytpq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bllsjzkz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cweumpyr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhthoxsd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nxmjlojq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hxinnmbm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ilszzrbh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wrckytad.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2nlfmwkgy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2upqekcft.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnhtsdt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rimhfmsh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mapgamlf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2sisrydfk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rtchauow.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2omyakiiy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ljqubnrt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vmxebwhd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hiqbhrjg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2opsqrmey.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zeavwplo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ehekyhxl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xbtfzfsl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tgtgzili.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mthctaro.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dhsaiovn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2othnyjqz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yypqhftg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jymqztff.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mvxstykz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rggbedgo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rulqfhsz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hxafzcio.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mayaufld.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2rsxnzgrv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2unlvopvz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lfygcdbf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2afzklsfh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2meyqxkuf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iyfthdib.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mfehzyzu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2itmrarwd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kjvlrcru.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nefioasu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zmflpzia.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2linmpbqb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zaxpeyop.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2caclomxw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kfavgkoo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2cckrnlsf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qvjhnyfs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2brmoegpe.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2uslougsl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gcoylcuk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wunbmbad.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ifmuxree.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eqlxadgb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fsbhuola.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ooseoagg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ltxdsrez.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2illhwymm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kaztnutq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytngbisc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2utbygzei.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jtmqjunp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ajagogoq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2uilrasgz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rehspkei.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sonjxlad.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sqxzdszd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2msyxgcos.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2devwbxnw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2azbhmwwj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qvjmnall.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mmcbdije.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2phwjofav.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lgsqedss.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bhyaylvg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2swfzknwj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2yrdzqmhh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rqiujqiz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qorivxdv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2izvgtajs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2snudyjtd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2adhuwpfl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sixdnjuo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qikjyeno.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2emlmjftp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pytzovcn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qbmklmgf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gcywcgqq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqmxbpwx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjmqjjlg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bimqtpmd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kxoezoij.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lrggbmnh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2atsbaqsu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tomuhiby.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cuiqhwfb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rpgbwjsx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uyuosxof.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2esusfqev.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2awdyfluk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cydgprui.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2uovnlyem.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2diliwkcc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ufqexmnm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bztlmucd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zpousval.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2mnbtmnyu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bedmppux.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vsiqbwea.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mmfvcycr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jqcqddin.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pjurljhk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kzrojrsa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2mocyjvfg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2biezkjvw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjpoebbp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gckopwso.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2bgxinrgr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ngyqsyac.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ynwvitib.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2edtnaoxn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rtcuzcja.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hskiuvnw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2whtccpff.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tzvspgus.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mtbzmqqq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rygtkyuw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gmafvgrv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pumeeeww.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2velsqjqk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2oyiuhuld.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fhdhiywn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dqofuyzq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xrbctrel.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eoicjmuz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezweitsg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xyiztyuc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uozcpokm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2punbnmzr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rnncxlwb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ovjqhnuz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wbydcrhz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rqpyajlw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bekulbgn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tgsnbjjo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qxfhqcad.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xqitqvwa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mgbnppoz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uifzlopg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ebemfmgg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2anodwnhv.html


<!-- 参考信息 -->