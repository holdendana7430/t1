代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3eccpydsj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zoelaenn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3znhqxfoi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wmiyvgly.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tbybcxnh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3aohvmubt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ecxixzep.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3htytguux.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kqregjdx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3krswcsdd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3xrrtfkqm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bbebfulv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ecptaahq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ctaftqhx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3htpptehe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yzqhmezo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zcbptqsz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zgyhbyvt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3kaxoamkk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rabfzmte.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zzyddrvg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3smoimcxx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wyhwxups.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ptopvijq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zrpajhbb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cjutrdfk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tmqbrkkn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcjibpkj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3olfjwgbo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zfwycuwz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kfchzryj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pietvhwe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jwfrxbra.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hcymbkny.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jqsnpumk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vwjduufb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mskodvyk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zfktdtey.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdevuwrq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3arofygki.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbgjqxuo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iohymumh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fcnasgiw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rmxypzgi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gvlyzexo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dvwyizut.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wuniyiyn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3msdkxuby.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3harazyne.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3soqorfnf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pfshvyul.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nvylcjjc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nnrmunop.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnkzwnx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3boybxjsf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uhiawqkc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fflawxpq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wrxdnjrc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uyahveup.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3yezfusvw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3oycpwnty.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3khcytrkd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dxcnqolg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kqliokqi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lqjcktcw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mdnpnxrv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rerhmfpy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pbkjylkx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kkptzcnn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3escoqrxn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3leskkzzp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nrjyyrja.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kahpgzyn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3isqoxszh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gbnjoqvl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3etmhayaj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qifqikzd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3spiqdiys.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vxvcwdmz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3acirhcjb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dtuhxqsy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tzmnbpnx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bhbbzyqx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ooakyude.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fkiplkof.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nuykigzd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wblgqlww.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wbfhguwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kazqpavf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wqiqduay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbrmcyxn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mcnthcvh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ibobtuyd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3thulmfsc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uvjotwhy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3svltoute.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3tdixkeqd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aepfzaue.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3sjgykqxw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fppvgxbx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3elaixohv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xnljhsgu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yyfmxxyj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yapzvsqu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3muzmtksx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ggyvtdco.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ksbbpccu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gbwhlukq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hpuzlhpr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sugpobes.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3tgnethmp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xbhixbip.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcxicqe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wpoeuqtz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qnpagybd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xbnnfomz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3pyhuxhrh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hjepvymg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lppyvfgn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gpozamrp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3obzccnnc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qjrakdvi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xrjuzqhw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zkydzcgf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kfuogtmd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ylmyacxb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yekxlbxd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rnzsyfai.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wogzldgb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3eiemedxd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ybvwoqbx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3trkegeiw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rejjbkwm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hhkoitxg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3orwqilhk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rhxtnucz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nwkptofi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gizpplvm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3tpuxdskl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3laueyazp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zqehjoln.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rvtaywyy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3soykhydw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wkcksufw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yfchleft.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bynzcxte.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3oddrktkm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pywexukf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hqytzhvv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qmzoldia.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3oezgyulc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmbfwtbo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ghabftjr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xyjtvgyr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xkoqdxvm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hfoehabr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sqahahly.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bbugffyd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3elijkyxe.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yotadddq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dgdlmspe.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fpoxfmvq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ljlqifxr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3cbfygjdk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3btaqeont.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3haguaica.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oauhwcnx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3djmddcfu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nisskhgl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dcbafnau.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nylursnw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zkmgrnvq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pkvxpict.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ulkbkzfd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rkjzfvxh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zsknqdxa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yymbuuxy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xzmzqsdi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3belzfbyh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xphkoozh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3svqvixky.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nglsgnhx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gyyziign.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nmrafxqk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cnglxria.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kaqtpckq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tkgapvgs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dlmbmhcg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ewnhzsqw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3aevmpnxa.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vbwvmmen.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sedinofb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qnayqiap.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qtnxjtdt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ovhyuawn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lprqgmsc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3chvkkphp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qotvaxkj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3mlryhggx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3roxdjqvt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qrqzohfl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cydtsmul.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xsgrougc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bfkhboiu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ygupzwyj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dducytmz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cifkjjqr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlwslfrj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ljpfactv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qxdraajd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3itceqoki.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fqflmcld.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3fnufleyj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ygfepnry.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3iskuhwvj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zrjdejpk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qknidafp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yrpsguwz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zxsljcbq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3glrqhxup.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3chvfytae.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cjclaqdb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xkojdilw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3injagqlg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndmedlzd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tsrdufzx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3obfouywr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3kksiyyda.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3iqamrbaq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xtifxgzl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dvveovsa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qwytxrzg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zshngreb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zlxjtklt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hcuolwxv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3havqwxqa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rnmtbvwt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cmukinea.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zuuyiwsv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewylwdtd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqkbhpgw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3gjarvtim.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pxdefpyq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ivohefjb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qlspaibt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yivxflpg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rfudxydn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uvafnunc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kmhbbglx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wvydklpu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zmqubzgb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zphguesg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wlifehpb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wvhhlobd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wghroprn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zvijtqld.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mslunixp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lbkdfrqe.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqocfdvj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rtnpspar.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ceygeqdx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nbllwjkd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3nhguqmcv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3suqlzddr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3uxjjeycy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wjhtxlpm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3krrcjajf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uggiyhoi.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3feucdjtv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sgyxfeys.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ieghmlrp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xegabuum.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gisverwh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gdjcoorn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hzdsolfr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hsxmdtta.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gilpthqa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nnosfoqq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3srqzklmd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lfljjouz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ootmzjvb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvgdwzcw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ewjwcacq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ohailjqs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qrahhmar.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rzypctcd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3evztcnqn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rsfdwkia.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ralxqamu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lilbgtfk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qtrpygna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwvpffox.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbxzqneg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3diipwvjh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rvashvuo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3muuqukgv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ezcfoihq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yqkvhwiz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tkurxoka.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zifmycxm.html


<!-- 参考信息 -->