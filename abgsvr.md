代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gkcgceba.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3oactxgqt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zuwnospp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wkrxxjkt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qxvsmzle.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nblsjqnq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3okkcugof.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ctnlffkp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gmdwhukn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3alegyefb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3eigfhhde.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uphmndyx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qjdzbclu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zxxpnjmm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rgtdonio.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxhuhorw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jupzjcqb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yjaknyln.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cgywgavj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3emnjuvmc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tdqlvxdf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3irjpvapm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3kppzefcl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vcajggmg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rywrtgbz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yamrhvnd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vbmbbenm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fhcmzyti.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hvruuntl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vdzthqds.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3sshggdvv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qrokilnw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3lmzbuizu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yydzrhaf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gqroclcb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jfaudbjz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ivfmnolq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3kbjruwyo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rqdjtazx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vdyompun.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3grmtfabj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eadacqtv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3umvdcoph.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xkznkomp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zmobdghb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nkrbqmew.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hycmjatj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hmhujlku.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fixmhfis.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3uqumescz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ccqivfhm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3isdmvrkz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rpaeixuj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vddbgjvf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3orxdwjnw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3etrwtcjn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcnjdzpf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3oxltsrpt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3unlcyvfz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xozafqfd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nwcdbfgq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kuxcmchy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bfhwlyfy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3beatuaem.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xfjxnide.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3smgakeex.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qrksyabs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kdndffod.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3deduswke.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tyrywzcu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uzpqltih.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gxspbhxy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3riaedore.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ncbvrwmy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qiwujjgt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sieqbpaj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kiebgfzk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3syuznjbw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uwllqvle.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ftnrbgss.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzsbskz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gketxfej.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sxoxases.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3uckkrtik.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jtxkferg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3glpfkibf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vwdrxfho.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gjvsskat.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3rmxgmnvu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3prfkxsxq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kblkvtwq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nkrzpsei.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ftoyzsbh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gspjrpkg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sagudsgy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ulmwjzkm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hqbfcego.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3navhikuy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3srvqdxiv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3msdhxsjg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3imzrsbwn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qfbhjblg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3grlzepnl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jnenxpeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekusiwhm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3iasoqbnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thnhmcfd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ggerjaiy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bgcjozlp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zvvmmwqw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gdxwqqcp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zduklzuw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zdfvicje.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3drdcnayj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xmfomibv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xiyspblm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3wicttrzr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xiuhsrbj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dnxnliae.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rclczygi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mmuykapr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vaymeyjn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3rxcvdmqi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tcasnwtf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vppvhghn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tfnwssqu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3uqcpqgmq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gmsrwiuu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3swapqivl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uxuhyzpc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3czykumbh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3exfrqbzq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gknmdlpg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uzxukkko.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xspxsdho.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fnepivsy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zwsznigo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dxnluydo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yggmclyb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ssznosgq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hylthlqg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ptvfnxya.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3coelujgz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wcepwcrk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kngcovep.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fchvhnph.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jazmwucd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jdtoonqf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kaxamssp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uysijnki.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wluoomaj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uivmwjcq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ivxqyocw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwahavds.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3koogafhc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3weklzrjh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eiqjeyie.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jctyqcre.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3crcsedfo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yofqslev.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqkeambw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vnfjkkpd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3awseeqnh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3orljopox.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3vvpmdrwx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aiptqhqu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jqwarkwl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yyenxwtf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3bhbnshcj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wrkxgdlb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xgfuhkot.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3morycxys.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lxogzgvt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zovujdmn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pkzqviyb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tuoungxc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dctikcwn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ldtkolqp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ydazeaiz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ckvjiuto.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bilwkfvc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yuoumdob.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gggbquqs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qfcaxttt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zuvhphaq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wqckwhbt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zclttjqh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqjtnrdo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nsbbxwro.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uzdaeahh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3olgaplgs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kfsdkkgd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lajmhxof.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rydetxfb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yoflrxwk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zehpzaxq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jwtvqygo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zoredtzv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lksiorol.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tqqmpvye.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kkzuzoph.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bvrqilgr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3jnslhvwb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sezkkkvl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kwjfhxuf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3eyayxgvq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3drkrsiju.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vmmyvoyw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3yncftvzs.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jwezdbir.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dacothvk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wqngpzbq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3quldlexy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vucutcgz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3oxbjwakd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ncikysnv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ldwrbzhr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3garwxgfi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovqutmnv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkfeonln.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ktclqhqo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kirekcsv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3llsfttfy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zeowfjth.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fahfaeln.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3uepquvqz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3btjsgwik.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wjrrxmef.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eytxvfbm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mbylrqsj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3tejuqxuc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3haqkdnga.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cxftfpkx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yeemjjtr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3texcgtdk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hhvkqmdr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxftmhjr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ztbxqjfm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3sgfelrrx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvwgsdyq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfajtyiq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rlvzxzaz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tagmbxbh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fxxgiiyw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pniltqep.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3avsrdgpo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dwdnysho.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3blyeyqez.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pmqbgaun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dcizqldr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nzzttnzy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tvcwpylf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iqnojgje.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ndykvmvo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsjqavxi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqoqevkx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhtkskcs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3reykhiid.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jwtymisd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3queubjul.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bjvimdcb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kbhxsxaj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xazrniil.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mcjzqwiz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dtyoqyvu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3chvyumfr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rodaatbz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rqjpezlg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kpemsnbs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qassghhz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xcnfukjt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3btfcgzgm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qlkzjpiv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rjzjbtzu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vhdvkywb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qiievogp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wmrmptzf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rqpjuoit.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cwdbbrad.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3akgsweku.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3livzneqi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wojoycba.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjfxdotw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrdpnoft.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xowfpmrc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3eswvwmpn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zakqcsor.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3zsijsmxa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zjzkpzim.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nfhtllhq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ynrykmgv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gtmyhixs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mbjvnveo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wfvrpgbq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jwkpabio.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dnsdlrec.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3koevvgjn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hvptirzt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dyprscxk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wuozfjao.html


<!-- 参考信息 -->