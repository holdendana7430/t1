代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xjafmyfm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3efrivuio.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3embvnjbj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qxzuuujb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uxearima.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sxmpkcnc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3idmtfesv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ujxwgfkh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xlgprpmc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3skzddyas.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qreeryfs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dxrrvecs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tybpanai.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nslkvuap.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yeyjgjry.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3luiqipqv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bfqhmjxd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3shwabmkn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3chovfyba.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypkscqta.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bqgbuovw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zpydjped.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exgieyjj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bszycpuc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qjmdzqot.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3zimrevhx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3toebzele.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xsazdoip.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ayhwtovo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3sphhjshj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jqvdiekc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3buszrglo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3shqupwhk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3emsqbqsk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mcsytqih.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sjwezjrn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pymffugf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dkqnaiut.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rcuztmpv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jslwincl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3eolypidr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3vielwsni.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3mxjliopp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bsqrdnof.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ydyuavln.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3acjpmrnw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kxuoydvc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3uwjolftl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ghxhziio.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ypoopjdd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hlsirydu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fzswzvij.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3jmvjbnhe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3audlrxhm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vqguauxw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vujfkbis.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ngcynith.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mylibljc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ipdkenfk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlclxxjy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qdhjhlqo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bhvouvji.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hjdmohvh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3mmnfywls.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bjpxwmcn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3inyhsxrp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3geqdboft.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ykoljmuv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vlxaxgva.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kwqsthyc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gophzvcy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ygswiedx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xjjswjij.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3prpnubns.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3slhrfcgp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3edeyvozv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eoaamabo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ehcfmmrc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3izwbrfbu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ttcswzgu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3haljrebj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rjffurdy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3auzirkmf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bafyftpj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmuydva.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wjfmtpzn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ktrlcfsi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kzwurdkm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3eoselcgp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fpuqjknb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lqauydkk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3caorbgbr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wofefcop.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vqbbnfdh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3yawjjjvv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rfsymphi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gdsthpgb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3bferlkqk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ckovazxf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3oysqrbgp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qelgdryt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gmrunobw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gmsjmlax.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qhcgukjo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dhpzdbgf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vgifckoz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lyqjknre.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtfvzxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrfteccw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3shtaqaip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyxqfcsz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3czsxsmvg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3gwgftwhz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ewjrlnqn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vkppfiqs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rbvwojgx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3srutpump.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mphdkhlg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3jvrmsclx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eeloukys.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xsmqjkaf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tostcjzp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ynygdwyh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tlaytnte.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3svoclali.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gqdnwluz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcqrwomr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fdoomkga.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vwvxaddz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jpwarhbx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qriegbqx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fmdsxpbc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dfoqdruw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lsedyugt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oymhutly.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3czqkiyrx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gvvnjccj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dbndappm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lqnrmqkv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ubnssega.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nqqcfhij.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rbfrnbmj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jaushxny.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ukrxnvge.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kegaeadz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bsgfpfnw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oqvfhmql.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3tvemdnbj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3acqkgrfd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xxjrpquz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3plynipgm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gjvjvfwx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hwdsreny.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3cspcmigl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yvqambji.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uxdbrhzl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xsiacszt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3saqvueid.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vbscsvji.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hprkfonl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fqzdbywv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fzphlpac.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yiptgitx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fvbzafrq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vjbctdze.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dedyxtjc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3minmsmfp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vfdxysqr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3obtuqzcd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pycxqrxd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3tjncjeln.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zooyktmz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yczaaejb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3pqoftgzj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vkczkvyi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bljglptf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pqovgbnu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vctpoccw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iththnti.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qumajmgm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3yuehtkmv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3imugsaxi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nyyteffq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gxhgmxvn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zwoizdzf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zbsyczfx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qndqdzyv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tfjpeipr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zomcsogr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvmmekru.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mpykejca.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3phqbunuc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dpjmtwtj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3daswcyfs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3yzlaldrz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bjcdqyta.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjxekuu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hriuxnko.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcttovo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mwpchoaf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kcxnxerr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3moyyzvgl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dyalzwwk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3muqdhprm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pwpmkfpo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ffkrtuim.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wtliwcnh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ttgeippt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kbilchia.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3oqjdfggc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rhaiuqlt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rnpcssyo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jnaisrny.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iihkpgkr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3asumpiul.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hsbftjea.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xpebchrk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3etjxtukn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3yqlpvrbk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rqxyuzgb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3tcxvpdvd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzqqpopu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3siakjneg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3plziqlph.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfzrccwe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3gbtuozff.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pjvtprkj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bdcljjkb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3olitqyrw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jxxlopqr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3diorirzx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ahirlkya.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mknluxbx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zsagxjqd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ckcxrsus.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vgtzabqe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zntppyfo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qwqmzpep.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3esnzimyk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ilfstchu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mmccafmf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3qgmweihb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fivnuoon.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ybmadxgr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utkbdjzv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vavdzufk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pgjcbaok.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gcttcumh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zzbxujzr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3krszndfn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bkkowohq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ipufveth.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zjynznar.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xvskqhzc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3aorapauv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ktomoicz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bktxbvuh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ntpysauj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xnftblru.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddzbpwza.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wavevfza.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wnyfkyhk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rhsehkzq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wzyvkvwg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ehpyqfjo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ulylfyny.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cdxoowlk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dljiqork.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jpqazphu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aumlfqci.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gozgenpy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3upmpfcth.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zarbwddr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3abpglxht.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yvbpcdsx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pjjogytn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3myuzzfnl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wtymrhyq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rqerrxgr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3waiwpphf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3waftolde.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lxlpfqoe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3bjppyyjh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xyugzkez.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nfwljroi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdbowjnh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyzqgits.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pejmoszl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywlofoic.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3arvomitj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3avbgrogu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lojmfwmw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hkukixmt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yuoxrboq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3atyfcqxa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3prziyyue.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mmnzkdja.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ltxasskd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ojqtjpfk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jiqmfhwi.html


<!-- 参考信息 -->