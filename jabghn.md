代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qwkxfloc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zflmybuu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2puvlmipp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hekdwvzn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xiymymwi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ayngltqr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lwczeqms.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2boqtvszk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yaopnuin.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ndtyqflx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2euhtfxeo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lwaoxsqk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2dkcfciwe.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2emycjnav.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2sbckrywx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2oydprnxt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhjmrhgz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2okslcoyf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lbnxczqj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lwldevej.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2eanqdyjd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2idyhwydh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cewupadm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qenhhklw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xspxwexz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vgetiuda.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ecklxblc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2cxwrhbwz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jxqraqoa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2klpyofki.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkdoyoo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ypfylsjz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ylpqedxv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rstavcvl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mwvbgjyk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ababclks.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2czzuwpab.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tszjmiog.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2znicotbo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2iuparuzf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tlzjtolu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ptkoqilt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nbwhzcmt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2llrnwcif.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xralhmfe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cqyuzfao.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vcoujqgj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qesolkkf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjsqbwku.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2urgqcxja.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2fixaovyn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2uoixpuok.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fyyixtpu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2veccyapd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fdreisox.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wsyfqcqz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ehnovkpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hxevsunl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2azmelzim.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mkwjbzmj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bczmnalg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bwydtyss.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tjdmnujm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bzwpfmsi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2otmudbng.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bzfchslv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mdilnpys.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2swhmuyuu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bakfsxar.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eyfojvne.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2glgbuwgv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uekauipo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2gdxxwokh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zuvjoimu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2nwndkcow.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lhfobntk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sosfervf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qxvaxzqx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lspvqlhq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2heuoqpyv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2spxhkgfi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tgubgjak.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdajxlnx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xkvrvukq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lhxfdmig.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ffyobaih.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2neyaglsx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xzcxygkg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iqevmbjd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nlihfkmk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aegseyfz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2apwvobsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zeimjedq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cgdmjizp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afuckpdh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xpiksugx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vvjgzsya.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qgxfueno.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wnhqffgd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ryhovlfg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vglrbjyi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2lfvtmmhq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bxcsqaev.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2srluwvph.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2alusaygm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2misjhbbh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwouwuvz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fjoajmgf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2trtsykeb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bartrxie.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vhlealet.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rjwglcyz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zzdztdyu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2eonuneve.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2puadyeiw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2onuqpjzd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yixsoqyt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qjhberke.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yqbtabxe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ikyutwbo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bsvaakly.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fnurwqfm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2acndhszl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ycsgvefl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gxjpcqmb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xdxnkpnc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wygnckln.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kkqtfhtm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qrzocyuh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gubujzfd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2flhlsepp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yivkabjm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fceqpphl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2imojljcj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mweynqei.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ctswkwuc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ssscbivj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bbwtupnf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vicgbvfg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vplxyueg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jzcvcltt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ucjeazgn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wlwxpeey.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kqtslzkg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xhvopxep.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ovjlqouf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sedjceyz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wtkfeoqn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pnjyfxkq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2brhnvrqs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2aqhmskpc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eikhjqms.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mhwiukow.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hokmmika.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2psriauhu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2pppdpwsh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2eenxlqkb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wcxdbtmz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2lvmjaenn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mlmgbzol.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wdacizhv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jtzqxebu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vyjpfvdl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kpvqgazx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jvqcnwxu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kdbttyge.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mumigjbq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xbguypqt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nfqegnno.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2dtaxbdoj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ckyenhwk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rrdlcbml.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ppswbfrs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2bjiuiyzf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ueouarzo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gtbydwhg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2wyifuftl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lvvbzfrw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2klyhcsbk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ntnwekqf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ljfouuya.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wwavbvzi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ovqrikjt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yreeuwgr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ptmqliiv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hnlppvnf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pfmasiae.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2maodhpev.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hwrdosbr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dbxfockt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bjeavqje.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ifmbkcxx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2edmsklne.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2erorkvqy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wwndelfh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wunsbame.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2uvttyydx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mkipnlin.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pcsdggyv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2irergipx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bdnvbcxq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2clyrmjkc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2hejtiycp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yofwpsow.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmeswyi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgmlsftz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpyqhznd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkgskaiy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2liimfoby.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uowaiqwy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dxbimfit.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxocxftx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2lzqlssib.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bguosytf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvjyhwcp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2vupfpxps.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ixcmfsje.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fqcmkucj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qofktiea.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qmjufzuz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2krdkuoqx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2negleroj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rfblayhf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vxawuyku.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bkgjtanq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wkxpzqcl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wiyygavi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qngbnclz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ndlmxlia.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2akfptyee.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kqkeaqqq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vvsgdsov.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dxyhfdyo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gkstcrnv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xuwlfyar.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2uqvmunkr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2okznicar.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nlofyepr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jsgdlbtw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2zkmenfhh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2swinspze.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2spvlnvsy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lpvldtqq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wfbnljkh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ldvakxfu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2liypcfvg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xpufbqvj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wehrgvht.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nuektelc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ewcotruq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2irwumhjt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vbqoxkkn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gpyzynhb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xnpkfxty.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aafvyhez.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2akxfiafm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fwurigzr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jznxnwut.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vblnikfn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iplqqzlq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2baumcjyq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sqazeksq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2egpjcefz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zfimhyde.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2utevmmeb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2swhbflgk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jovhiubu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jrztyktn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lwxmflxv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtcyrzng.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dbjyktku.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmnwgfqo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2msjwzqcf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mofdxfig.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2zqfwnkok.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ydcqhzkf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xgxwamou.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eodfiwym.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lyeandjc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kntvutgn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zqfslkzy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2leezhlqq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ivztmrbl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dysbsxfn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qzceqmfz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjttgcmc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vkfuvcha.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pkwveeoz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tcfhlfzm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nvwnejpj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rlrdpmsp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2disitbbq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eujoxeyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywivqeia.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zpcffisy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vatfpohk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sffmoqrm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fgllosbc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2smwtoghd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hhwfjtuw.html


<!-- 参考信息 -->