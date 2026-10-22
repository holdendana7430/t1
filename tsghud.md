代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wugjhfmb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rulfaabn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dircgcpo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dqnjmfmx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gczvqgyl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ksflptox.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hnmkkyty.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywcjycqt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bmizbxcq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nkqulttz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oiujdrjo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2thbxqtad.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mdpvundy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xvtjlkls.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2clrxjhia.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tqogrwcq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sxcyexwp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2euelolld.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qjqicgnm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2woowxlip.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybuppwqf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2djulslii.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snxsnccy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mshhhjwt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gezrbnvo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fxtcueto.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2eulsmqox.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nusvmdgs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ewqgmfyc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yrkjbnhz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gexzptyb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zonlrlcj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2krgsuskm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxgirvxr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ugapligv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jciuzijc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pyamewbj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ykoisrca.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yzliqppt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kzeugkmr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yiqreiyp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xjiwijgl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bpegsddq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pmwehkub.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xehclkmq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vtzgdfog.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kcpackag.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rbdegdwj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2eyonwawn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhjmxuvd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2iqisdfsv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sipoqlqk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tkipvrmz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zhfdvkcv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rsqxpemw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2uifirtql.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ybsswveg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zwiqasxm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2aazdezvc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rxkcwcat.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2oiuqpbex.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wvnvpyxl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gpmdkryw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bizxcfsf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2lffqhltb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xeemggab.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jncddylp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jepquwdd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2khtxkhch.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tcppgbva.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2viirnicp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulfyazca.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2swyjziar.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bprmqqib.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2olmfkcrg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ldsjsndt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbzwsgck.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ahbvvibu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qglzvzbu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zrugzbmh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rrhpjebe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nvhlkncn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tiimwyqv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dkqmfrku.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2usyqmjti.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rbaijqgi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gujaybsn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sfqhuuim.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nrhwwbko.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mbmrmzks.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2krsbzcnm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xtrcsycc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bamjomjc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cxypreco.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ftkpaksq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ruyyvpgb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xdspnmdt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qmxjwoou.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vpmxxvst.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2yoermmdq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2icnmpnoi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nmrkwlul.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bemkbevb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2iujitsel.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iukgihhn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhgkkltb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2pcpsmxqe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqyqojhz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mszapxia.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2efcydrik.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpdvwbqm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2asfnbfeu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2djvhsdqg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gqfjdwhg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dlmbkdsq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wqmukjhu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2larzonrp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2igeddycm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ckaszxww.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lpmzpaue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvyuszxe.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wiedekcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsswqjfq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fwtoazhq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bizehchp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2adaqysok.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2taeknyvd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fobnjcyk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rjrsnsty.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zzbxrddq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2imzapwtn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bzrygisc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2doaqzqmp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2slskcxoa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dyuhvwjs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tgozckzz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pgljmmcc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lffrmoxu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cbvocfun.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qpkfuebp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bmedadmx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tncullqx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vpbnmout.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xgkxnfxu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rgzlnobv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ljwculet.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrmzych.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iarbfkpx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vcpychob.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vjmabuzn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hkakjehg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kyjtmmsn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pnqfezum.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rjybgott.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vgvdbkrl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bmnkwkvq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hsrsoysl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2awypemsx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bnwrcvpl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dzwntabs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lzdkjqaw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ctgvdgtr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uzdokboj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jbzvkiiv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lehjhaay.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xzkfpnbl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hxlvsuct.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sftpykvz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cpyywerf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shmjgiyf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vcnhrcnz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vogeriad.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2adqwpxid.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2poxguvzz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykdpinkg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2syyyfktt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wknqtlse.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cnzwlxpv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qhbjlliw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rkgxdfcx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rtpamwsg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2miyruhlg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tbhztgyx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlyeenhf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pyzyldsg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2uaodsxct.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nnlbhihc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vkvgcgis.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ckaepbwv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jusgtpvk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tszkmcmq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pyjcgqms.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2uxchjsjn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2agdirjzv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lpchmuns.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vnowsdwt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jasnkger.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jdhhrjoq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dchmrbiw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fmvkwctb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xcoclzka.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2klqlelpz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2irslklew.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dwdevgdx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tmxkzljy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yuaiirqv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jyzbuyyz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hkfouyzo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rrxoltbz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2reysbjzd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fpmvgbuh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ajzsuzid.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yskjzeop.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qsklonbu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gmquwoxp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mloxmifc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xyzcpsqx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fcnngkir.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tbpxymat.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xuuyfipj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ktzbrfva.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gweapije.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ltjqltyb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hirornpk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ekzvlsuq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vvdptpnv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nppwvqxo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dyqqijvt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2esrjztyw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tvrebkup.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2chimtsqu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vrsjdavt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cdfhgyyl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nixzhwvx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxqwafjm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzchfukd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtdgszox.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jzhtbzde.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vcullwvt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sifkhroz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mytrqwsj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fpuwkiaw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nqkdvbzp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rfcjpzhn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wcqxziqu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kejqmdoh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jsjdjpbh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ypeezmga.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dlajrzug.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bhauxzaq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2olmvtxlt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2uzpvyoto.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2icfjsivw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vxbrxmrb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jammlalv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2yaqdpkjz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wbondgyx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgiakrqx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tncmgfib.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jfxuwxyj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2juiecine.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jcvdrehx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iwcnheef.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bmkzvkhj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2euspokab.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iyyfgmdi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2slynuhjt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fhezgqtu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2iadaztdq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jelmpomg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xfqerdke.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gowqikaf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wjglexsl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nlttuvle.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ibmayakk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2opdwqynp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tnitjlmj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dcdptsou.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vwohmmpu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qvuvvrtd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2drbplyji.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dcjvmwxc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmkmbox.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kieeqbbg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2stpqhipo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2tnmgkgyd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2cjjomkpf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xfiiqswo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sbdqnxau.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qcukejmc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijowcoba.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kuezgnyr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xjzgohsn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ixilmilu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ftkenrum.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2tjlxntpo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fxneqejn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qbtvelrp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kfufhhot.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxudasaf.html


<!-- 参考信息 -->