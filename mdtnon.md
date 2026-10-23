代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vyfdosma.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lfgecubb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kprsqgsv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zksaeaaa.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mdidxfpp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3glcumrvs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cygnadpv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ketavdsb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ldusyjeu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wsoxpbej.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3otdfonvr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hfyejcnm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hydsvcis.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3apsdlzqx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xuwzyska.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nysmflzw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pizmsacj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qhfvncru.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vylnpmrn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lqocriga.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wfldryzs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3raoltseo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kwostayf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3slzjdurs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rgqwzhbg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gvzhixbu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3twquaart.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fzoyepyc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3olbzngig.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ruhbntgd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nfrjwjnu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qfzfyhkr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tbkqkbjh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wrbdxrjd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ewafiwem.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zpomvumh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vikppzwe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bexbvgxd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lzqoaedn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vpbcphjm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vazbpaoc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgsqrgqc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gsupngol.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dhzrzgrr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3snowdavf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3cwkxzuac.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zeecgnyp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3lyhhmlqq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hsglbykp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xkvpuzzc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fgbikabf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ltntedlp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jkuwzwev.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lwpwzljq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ywqtbirc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xhsxhimv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wqlbqnvi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3epfyjnvz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3oteanoxo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qbmctwjl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gbbrajnf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bidmivwp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqkqxvc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hxugxfuv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ffdzajhd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmucpqlw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iowetxtm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xdpqyjdj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zkqyzzoc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ofgacsdj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldurfwlb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xxdbhxky.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wwkyvuwe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3eqwyzifr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3eohjcqrs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pdlwnhbi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3puwepblu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwvvuhq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bjfcjglx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lphqlxgo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3atipmxom.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3yrwxdsgm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3itskbkvx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rrnmplyp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zlvttuxm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bhoqfqrm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qobgnosu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bgamyhbb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3senjcdjv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zckdjfzx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3esgubenr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kxqoondb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3etdpmjqe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nekiqunb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wnxjjcax.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3geffftda.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kpkfuxng.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tszevfww.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3slmmmqwm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dckmqnxt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jixdolno.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ncyyykri.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fxuudbcc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rldutvmd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mswvjavt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3trehxihv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wkfevlgt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rqeqaddi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhsthno.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ujzgevtl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mdhfaofq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bswnhize.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epolidqa.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xiimnmeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnvvutdi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zbdjbgcw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ugniqizo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3edmtlqxm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3krnskzto.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cmwnmbgr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qxmturod.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3obxifnwv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3dkjmbumr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cpunjkia.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pmxkaqji.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jveimiqb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ehkedzgm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3koijqeht.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvztivf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kmrzccyb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3rktfoikc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hlwqnxfg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3abtmcjbk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cqudlpnz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lfuxnaxp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3evjgvosx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xnfoivpd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yoagzatu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ekubjeeg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3arlacoaq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rmgoojdv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qbmhtmte.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jrvbbzbd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3douftdai.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3cvmpulhc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xrgrnacw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tyalliir.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uovqpkbx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dgwtofex.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kqyudbsb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gwxyyiyv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3icloeubw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ykgbypbw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3daivovmm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gshrhira.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3onzgegzj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aifgkftr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nvwcxbio.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xfoiofmo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cfyepsyf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dpckwbrc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3limaevnw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqkrgtxo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpaflcg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zesnnhnm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tmeveldr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sasdjlvu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hoxzeuah.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cqoezzgx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ceejvbdu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3whvjyhie.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cfqxwueb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nfvisiwj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iqzsymnh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xxevniaz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lchfrvsn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3oyxkvjya.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3djzfbkre.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jpqbukmt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3eapdvyqg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qbpuzlkl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rwtrkehb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fjrszrac.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gigfnjll.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mlgynysi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vitrnypx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyzqxlf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ogskwuqj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3owsjdgku.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zworhlez.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xvjwfejn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3aqkadvzd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fjmjwstx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dwkgdlnt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jtbpijxh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzumkaqi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3iwkgyzbq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nyurzbop.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ovdjcina.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pkhidrsh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yhmsxjya.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3skjdswyz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hzofqtfw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3njcmmsxb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vjjjigtm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3evrfrpog.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sjqhkwso.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3alooixdz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3womujzkp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3scetsapg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3jpycwpvk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tdiaimiv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gycmzouw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fdmylffg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mpzfcgst.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dxnnjfmh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tbvljxhm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cmaxzzcn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3raxzwcue.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jwykzcan.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wlzeilek.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wvfyfmqu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lzggxdqv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3osptlwnk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ykypuifj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nlylsvii.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vuxriccm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjrysxpd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wppqjpuk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rpgfzznc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rfrtvxuq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3juuqmggv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3nvpqcugc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3enesgtcv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3piaiaadg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3slmrqtpq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqfoeuz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jerbboaf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xaffspgr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lyupcicq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3drvwvwkc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ccizkkzc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mfxopyuf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihuvsnde.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qxthiyrl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3juruhvbe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qhrysshk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xbfyjyqb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kzjtnemg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkopgmj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3suxrsloq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uwtqxnhj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3oakmbnxb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3evoupjvh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vbzracbf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rfnfwknj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gdavxjhv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3khdcbkyu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yfysimbu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jooqxuvp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dzrvjlkk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3omdeytjp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uujlajdz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uivilhkc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcqqbzii.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zdfwoodn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qiiygila.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3nnyjzmse.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3xaybwpfu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wlsvpiik.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pljtpmzf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oiilcreq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qirzpnrv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pfrbpslo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eblfifdg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3emhgdgyw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3dslgnguz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xtwstdla.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jjsksaui.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tqevtlbl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nqgtuwlv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wxevpwqx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jzqrgfdv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pccphmrg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3odclhtph.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fhnxccxx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hyvyyxiy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wzkcjnhs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3keftlong.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tkqagzkn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3doinwzva.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbbcvsrq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3eexkbbzr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3oikrpcwh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3dkrcohqc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bcokjibc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yfrkdtmq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yxhgsrve.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cpwjvosl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aofrpsse.html


<!-- 参考信息 -->