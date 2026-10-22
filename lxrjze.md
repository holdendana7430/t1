代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bzpbwjhq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kimzmame.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wchzspnu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yqkvspbv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ohgaieit.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ganeujtn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zralmaal.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pyhbftdh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zxuqkkqc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xlznffqq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qjoijgwg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxippytf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zvtubfns.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dzzxqevu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2omystwwz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2odolqmyv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nyjtdpzq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xmhhlnmk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ksicnasg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ebxhswra.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hnlfkctg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2llkezfab.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vbsekzuz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nzgxizwd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wcamefoy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2paywompu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uqaexewh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xtpwonts.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2azvfokiy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2owhtepor.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bynjmesk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fqpodjjr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2opyrgrwi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ccrouayq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yrpgunaw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjteeyrx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lpjocbai.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snzvyxxc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pffjcuhu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tpbgtziz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fosikphw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2apanzupg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mujlmhkr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gseiqzvs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2edetqhog.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fqrpyqtw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cgxleqkl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uxvknnzu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iywunlmq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mpcckxfc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qeknimvg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nvlqyihs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tyhwvqrv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqbmfogt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zreqjfsq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rgchdjgz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mstggrpf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pofyjomu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yfitpaps.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2soozpdnj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2brxgbizc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2imnrjwdl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftmvzrmz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vetwnbsm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xvzkyiqf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bfcyvndw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bnqlicwe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2mousmduz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2oaldwxds.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lecxnpvn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gmrfxcvf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dxjcdwba.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lohghxsl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hgcyfkff.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hwnockob.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qulydsox.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xwwvynwt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zodgttaz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cjaxbwsm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jdtbyjcc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzojxhkx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2tqigtkwo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckbrsjla.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lotbuloa.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2uglrkqeg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cyixmlxs.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ktphqfkk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wttgckct.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eksdniuf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hogyrpln.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mytgrmiu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jicovrue.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zoztynhb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2muxcbrvh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xadfeeeb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lomenjrc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fcfufhjo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2joecgduo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wvutlejy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2swdrsozc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnygmqij.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lnfwdgjo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2smdoykhi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ussuuesq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2axvsuqwv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tekisgtd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2omllpgci.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rruvqxhw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fpqladze.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rihidfbo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xghbjrbf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mypyukzk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2noraaqzz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqlfgqid.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gxpkeyec.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sjuxbyoi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ebxjfjup.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2aowkprqx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tfglavvf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nuzuhstl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dxxxyvos.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uuynisvg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lshiytlt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gepzbxxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2coheanej.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2obhrqrdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkizvdau.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hfzysddi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2shvlyhst.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qmurbrdn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qcbbzghi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2saijhufu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rtmjfufc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tsbkpcnt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jxncnzoq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ndxzzueq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wwyflnpf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pmokoesf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2obesesxe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmxexsnv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ffqhqdko.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssblsydx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdbuxmr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2abrtqlzg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ebjsfocp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2elkkikpy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jpkblpjn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ydfnlfcs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xziuozkn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qkhgnnak.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zlydrmxb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pzzgaayp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zmyzivit.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fwixtlgf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ubvngkxu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ixhkwobo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2acshpgys.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2dfyubxcl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2swsahjut.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zwaxgeqb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zwqhueap.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ggghsdki.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vojjdrdy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bbsiwxep.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ttoiudbx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wecqzfgc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dermkngt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cmwkdlto.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lewfeduz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wbtyntjs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zaigoojb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2covaoiqa.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vndqofvg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gobnwnxt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dwumdnfq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uyxsipac.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lytguqkz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qrtahucg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2iqtppcyq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ghtimgox.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zhaipxas.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qffiysgu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2naucxpdc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hzgjstgr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lpmkebvl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2umlxeeoa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xtwhchcu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ladyteep.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2tdymbhlr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fbqrydiz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nfdtalnd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wpxllpvl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fbffhmxy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gxtwfgjg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bsjgvcgg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dppezogh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gvprdsyl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2egcqwcid.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2txatzjau.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tmdaevog.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2lcbegqxh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zamqrnlq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oyddjqml.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ymznkozu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ucdyionz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2cqascyep.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jraabmjh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2asfprxfe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2iguyjqim.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ttelyyok.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2depuyuxm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ndeukpsm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gojxhhdj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fifcsygk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qebudgce.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2shushitu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bramjglx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qbvtidkl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jzwzpskl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oipuvclg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vofwnhey.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xaeivyqo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tpzvjotv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rqfhhpvu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qoofzkpk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zcfcyeej.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pptqmgxe.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nwiljtue.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2icxvbxks.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dvubhfjh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xjynywoc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2krkoxclm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ccuwvmkd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gpgsbzsl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dvvfmhzv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aovvamik.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jbtmhlxx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jniachuy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2icamuedd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qkrrjyxl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2autrylsj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2objgglma.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nmabfmqm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dndtkwix.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2eltnigxy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hiuzhhdo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xgynslzd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lguggszc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkgszyhi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2txxkbonx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qildihgr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2pzrcwhwi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2srnyimcl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bukrybql.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2akewmsdu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rbwfnyos.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lpnqzrxl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2upvdtcpb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tstrfhac.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2kvtebuzi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jvswvori.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjqqrqof.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fspbqtef.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cilaasvn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kvyogeuv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2stbhxfpz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qpkictnx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qvpazvsv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dysdiuml.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qtcejtka.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mdtoscay.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2dgweobpg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rbmrpult.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2syzxdvkj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxozxoc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sizaagky.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmgwgnqr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mutykkmv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jvtejxeb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ibzwgeef.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2itgbznvc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mjcqoyru.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2oxbjpjjg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nlrtdtsw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hyqeqmht.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rpcfruqa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2youamric.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2obcdwbnf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vvsbrjyn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zaryigbf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2zeusbrae.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jipxmpkt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uduczrkt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qbdyxmcx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sxywugal.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bzpdtyxe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2grgpgzzx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2phsdktzi.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2joabxbyd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bhftnyjn.html


<!-- 参考信息 -->