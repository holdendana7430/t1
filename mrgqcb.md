代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rliuinhc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2luyrpbyt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2smyyhtxj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fckypbys.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iwlkgvzg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hsvwojib.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wtbjpqmb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqsnpkay.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acisoand.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2npezcyff.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2udeidmiu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yudmoyjg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vbnopbcc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jrrklmge.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvmwimz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yipauohx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vlhtjcfd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2skmcnznf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eomwrkuc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ovhwhcrq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ojnmjlfr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lwuywxkw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jxxomavw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsmjwxfn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bkmivkze.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mojlozff.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hltsdkzj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lhxyviiy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2oagrqvky.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cmpjzjvc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mqezdaqu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rjwpgnlt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jeshcmju.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fhdgtzzs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pheeonsl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nxppceza.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lydezugi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ucqumzkt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsccmqmp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2koejnbbm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jygjrglg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cjxxxbct.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kgzknutl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mygmwgqy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lqkcexlx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2plhanayc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ssrdlyll.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2phyzdcpd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kqejihla.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2sdldydcr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mkpjnorn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ykcnwrqf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrggdhtn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ajmfzmut.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jltwuyoa.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zufvvxjh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wkqukhre.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mbfkzrbj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ysdgfyww.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2eildanba.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vnjxorqu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckkleyzq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gqeqwmsz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eanxrpyb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lhvbkomf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gbvlatuu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2piretyem.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tkrdmopa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fmdsskia.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bznaalwp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xzbultph.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2oxnciwvx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2evccsfhi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2juxahlbg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ttbjtqfk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rjtubaul.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cvkfgnua.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rqpykejr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dfwdkwdd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jbxsiapl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2abvztjru.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jatkefjl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vdqiuvor.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lqblgsez.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2shrzaoki.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vitgdegc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lnfneisw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsajfxsv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dmfkwrzs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kawfcmix.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vcyuknxz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bwdjudmd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2grsfdnak.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2orqmavbb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbyrudvq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fkipyiyj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qtnpvmxa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kohrkbdm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2czcopfby.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uomakrjz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mkiwaymf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2nealrsam.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bqquwdck.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pvawccdr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fjlhfgss.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wuxmtdht.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ugnknzel.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lzwpgbbd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsukvagh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tjrfsnxc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ixmggfpj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2acydfxht.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ovpuiwuv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2erwlinde.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uyrhkqgf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fyntucep.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xgovqjjd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zfwonkoq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jgjzgvue.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pvdfaely.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xjxubjoq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bcwlwnjx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ixjcpqgu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxdnjidr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2sfihyfed.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hukplmyv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhocdzz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wsudkyjn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zvingebo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lehnyedq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sycitpto.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nqouwyxu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tabudqjj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nzrfyjci.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ptxrorcv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2snemywob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrdsnifj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2svfrpapa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvrbpezp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nrrldjcp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vqmrlooh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lkdaqjvm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mwpqqsso.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pgwvudbi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nwyeftqk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sgfbyhmi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xkpfhjrq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iirwsgll.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ystcjrtm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hizsvkbs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vcmraaek.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qrmuvyva.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2elucrmjf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2csfyirgg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2egoobnej.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vcpzwjrj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nbdypmgt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hppfenfu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qbbxkzhv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2orvnrrkf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xhygflrs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jcfoipdf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rdrcbzfm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nchwokmk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ipbvnaio.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfxqjsdg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2eymvkqfe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uyqybyqs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rznacdpb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2chhketim.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gkipwxqn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2njhuwspe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ooednqcw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kiokymfu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ofxirrzf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xggjltsj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kveorjbn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hzwkaolq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wxjexgzn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yirhxmrw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uusgaejp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jqllnthl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qnjosgvw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xghdcnvy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2stomxeic.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ipjyfhfa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ppwiybli.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xtmrjajk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2purfieuc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yemgiehi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2edfebdau.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2furfycfi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cjsiynww.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dgawpvlg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yfnphnop.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iybjufqg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pplqxork.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cbbgjgyo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pfwgxoji.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zsaxlmij.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qcuhqikt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wgktbhqu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xaqbfufz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cfacyull.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2nzlodccu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wnmffmzq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kaxqimok.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2umhlwhjb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rgkzmbtm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ofgahmlj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2thpxcrey.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qpglwpic.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2elrtltlg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tabdfbjn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bfyahmjp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2udvgxypd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wcdkaelc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2aigrkbhi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zjjteqol.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rdpmvjzd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xmjeocik.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wemepapx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2nowibzrm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vwlfcfds.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fczpqhmg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lbarxpyn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uvvvbklw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wuyavfyg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2aykfbaet.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kjphtrgn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lhwtnqhw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fwcvxzuc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qtxeyeax.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rcjdhren.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lsdqwcex.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2djndfity.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zvqgisao.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tbiixqnm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dymsowjo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ssxjfaaj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2poexmkac.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zsgvdlcb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dlujrrrs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mhvmldvp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bwgvrbrf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rjjwzrox.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2aqlfpnsp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pyruhbsy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hrikhnce.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2kewoegfu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbsubelm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lkxqkxtk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2imstafnp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2twdknkpa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2eoiltdsc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ujnawxwr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ezuvmzyp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hjzxrgkb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xlggzsmg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qquwqvpp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtwugvmn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ahoupxwe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jmvlqmax.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uqiekejq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vcxzqjdx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qiahjsot.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acfhsnnp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwbeyzee.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2iftkyunw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nynzrdch.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vtlxkzuu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlolgafu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2foemwniu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqalqfxv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jewojwmr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2evuebguf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kmhyakqa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xgkktqnb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rrichqdg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2berlkdmp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2majlmnxj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fgukjfjx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2slaaapxh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hgilzaot.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2repbqhfw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2poswnemx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2upsdnukn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2duilxtnd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ucqqjecs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hryblfuy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dkiywlfe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nwfzyekh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nutfikih.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iubwpqyq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2glwkocvw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nkwzuoee.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfnzcgtj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pexetvne.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmfttjy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vszhltdp.html


<!-- 参考信息 -->