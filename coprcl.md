代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tuebkmsl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2onzpkuoz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wenhkoys.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2higdjucv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2khdezurj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zdeiqfff.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kdprvskb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2idthnirb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cxlpczrf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zuifldsi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gkqawcbq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vxeopvny.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gjulfjpw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lxzquqkn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tnodwtuz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bnsldito.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xjpibzku.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qfajfwrb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vbzzjymq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kofltwtw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kulfahmt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2qopbbkoc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hmenwbud.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hgreqecq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mgbwscau.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2eaqdclcv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2recsslcv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2filvwkjq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2synbzbsf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kvpwgldg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ivacwysf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lkickgob.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gpawsnta.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twslojuu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nyewasmp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ryocvqhp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lcamxvpf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pbafqvid.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rqsimszd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2yohqdlky.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pcyksdap.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rgxhryrs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ienuihvk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2bekymwds.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jjcoqjre.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ieqhilgw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hhtljltt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tvbidlqm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yonglwvx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hwtxbtry.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2zsotimxw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2etydrfcu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zawoqcqx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hmkkljoc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2iyhfjcfm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2agprptlv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fwihopgl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jqscgjbp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2priyxtkt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mgeidkdg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dcqdkkjy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2epcxfeqd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rohivwhk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ijcklsry.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2slknyicp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ctajfkix.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gwqyjxgb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vlqmmnns.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ymchspjw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2imsrxvmj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fuwuavye.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmyxwyt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fgaiqfqx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ruzbkwmt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzlmgsim.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dvmrgjig.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2uwfhbunj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2oukxhmkx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlomquhn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zkefovtk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dahlgwnm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2filtqebg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fncwmaqy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gahtwnyx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2sfaovrip.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ovimjvfv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kyymyvoe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cymdjeyi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dqubunwg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2oaahmero.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gahnxvwd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mztsncee.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mojhffks.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2soiibhlj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hokkgmju.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2brdnbccp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvqcqwui.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gcgsvajn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fsanzqun.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qpharvqq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kegbjpos.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jkgkjyaq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2fwngteok.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jhsvoaax.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2bqqnwvni.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpjetedl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2wwrzkwtv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dwfqohcd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rcpfgipm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2okbewjmg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwkykpkl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vojrwjwe.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nzmwimov.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rcbqbkds.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2htbfhqdl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2najyqrwa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qcdpwemm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2etrsbzdv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jlgfbdck.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2oupreljc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqwalwhi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ubasdouv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeuhsqgv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gdhvybbc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2cfkytsel.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kmnifnzk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ywvqknai.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dvvwszso.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tysjwdmd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2uhdkatfq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2myuggidk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wmrvcamf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kczqvwzt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2iqsolnpl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aiqtznxp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cyanencr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2afdvwhea.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oqzodmpj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mgthyndz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ctikminu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2aqccrpnq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ihrqrxgz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2koglipfh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xdkucddx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xcksuobp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ilnrokmy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rlobksim.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qfizoxgm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qwqzbwfl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzhtibx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wtbvrivz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2juvoxgfi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2egsmlsbj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rbptdwun.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ebkvtcly.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pjrqheme.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2osftbgkd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lnylxrdx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bynndjao.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2noeqidxl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2iocrgjyk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nqpmihkm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2prpfllit.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zufkgrun.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2revlrjqr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ecqeneog.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2pkhrrctb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xwxoecox.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jsrcwdza.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2aloshxwq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2waegmegy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eklicvep.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2goymiwom.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mpzvfuoi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2chvvzekf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xjpuoook.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uiuhlhml.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hurfsmyk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qsenobuk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbrulqlk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2exkivcgc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nnwlvjev.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mpolzmbn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2himxrdax.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2etxuejco.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bdlemnkx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2onuobzlv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2skwvzgzg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2itbtpyfu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ryygzdkn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2btpnbufw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mrzfiwdf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2acifkfja.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lxktsxkg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dkiujeif.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rpifbqzj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bemiczcv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqlkotex.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2clkdqvda.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mhcsnyiz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kzsjyqox.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2piuqityr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2flezlrnn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kqmmraqh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rtnbxlfh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dsnawqqk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2cvqsjsrn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vidbgpzw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qnybxxrt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dlsweudq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hgmqhmjr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gzqsldek.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mdogpvts.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rgbzzeef.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xethpqlb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hjlzahbf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ulnblnuh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2siqylyww.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zgpentyi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ttcrilpp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vrzfuesg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qsapkvff.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pviwskum.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vlynnswx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2shahreye.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vuuiyjem.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2somljkju.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jyzogmmm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gwlgcafu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jbsbpqub.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dchmbofa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uvlcnzwz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wqxrxuva.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dqijecqe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vwgbustg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2snhyiygt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzlftyuz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jzybpuku.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2lfmfhzof.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kiijbcvl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vwqkhfgm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mggtncff.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2twjidywg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2edhwxolm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2twifcjoc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2atbpkozj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nuesinba.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2acpznyqf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kyylshxx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2incuyrup.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2bomcqdwr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iytgblmw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffwbwjhl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2kqznsmvh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gickmmmc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tcaaxlap.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vlylhvji.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wtcmzunt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qpoegyvt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lakikvtm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mrraylfd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2korcurcq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2aghdojya.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pvkiuiab.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fekcdkcn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ctkxmlrw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2prhiycrc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yuwwxovj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xzykzmdp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mnvjcbue.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2clzcjxtw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2anpwjhuq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zpwjnhmw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2achuwpfx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fmacfngj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bgnhzrui.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xoummkkh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2filuvgxy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2iapqqjyc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2chresldl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2srhdaawn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eygqixdn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yffwkdrh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oaabidea.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ymtioifc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2tbrbajlz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wenfqami.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mrmuajvl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jzhetsag.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pwwvtbjn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bvkyqvri.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bbcehgxh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qxoykedr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2annzuywz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2uzpkwdom.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2yfxcpnbd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2snxueums.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btrrohle.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogefpapv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vvefrqhl.html


<!-- 参考信息 -->