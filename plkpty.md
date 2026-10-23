代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ibiupwtr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3epdrfwto.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hcdkzfwl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3tveetebh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kzuhxwms.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mxfdjrap.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3egpezuja.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nzoovjps.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3omtvkytp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zmnjpimr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ixxvceof.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hcstmyde.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rdmhvbso.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ezinkvgj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3jrwnqqdq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3wdtnsquj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3otspnxij.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3nmmuhcbh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ncveoeza.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wfrqvtao.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3druuntzf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3yhtcylve.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mtxccbgq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3sorgaqgq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lxnhsccj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lznqqsbm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qzurkhem.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lmazwywm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3miookaqh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fktpvmen.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ouyzbpbv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3frrvvizx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cxkeckgn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqpvwwtc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3keyjbdct.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jsaayupq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvfmmmt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gsqxvcsp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qfwaxezr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mxfndiix.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lcpsqzkh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ooffjkcn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ljbiuwzz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3oddsqjmk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zsmuegob.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gaixoaxj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3eyumwmyk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hauwpfig.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gsfsqops.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbbehie.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iaodcxvw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pntdgaba.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rcdhkjmk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbrulfo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bmzebonk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hhnkpoxo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jedqyiqj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tyojysfs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jgxsajry.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ykdngvec.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3sjcxeutt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mqhxzhyp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ljhpfbcr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ujqacjxp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pauarubu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3akikuwag.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lrqghchp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zvdprwfw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3rlixsyrt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsrqphlp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gokzqije.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nenxhvln.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3scjiujjk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zyplkryl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3prbzfivh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rvycdcdx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3indpgjre.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tanmpldt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gqmedcmo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vjfkvoit.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3scnaggxl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3irugvnps.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3miqdziiw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uarzecqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kuuwfwxd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jezginlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvkixvac.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3whaywgau.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zqyybozs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hxfhmdhd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xewrotcw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3etbdngga.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwdxuxpm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fjlgstkj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xkpwqhzd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oalxmwiu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3otjbnoob.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3clxftsob.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jcfynctn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lmhasial.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ogcorlei.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zkclnagf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uesqxlag.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qpenbjvp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mribmdzm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3utjlcjcl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kgxfavyx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pqfkokjd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fbthgrth.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qdvqfceb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3aeksewfo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qijgpmme.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dnnaufli.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nqblmdhw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pizppncr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mohbkdih.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3twffgbdr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ljbtqsvv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mpjkrhgb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cguohvqb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3aknfwolw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mzkrnhmo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yuacboaa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qeooyxzf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3csqxprdc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jyehzmdj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ltjumdtw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jlcczpoo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3snqwjpba.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uekqvqlv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xrjvltdq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nqqbhmrc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ccsdaxgx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3atqiaojb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tsoqufwz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tokxyjhl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ndrjxski.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pvspfkwx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nlllhqus.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qcoljyta.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqfkguw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yjtbbxrh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3gdbvjize.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3frbjhbjf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3gfqzcvyr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ndwyjryp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3yfnmeecn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lddgguyj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kmygstgr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3egjxaxzx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qlmjoajw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ltysvswz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3uzxrobyf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cmahxzkf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3izqashnv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3euelcyfk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hriixqjl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kfdvhhka.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cjuifmct.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qhcajjdw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmvgzmyo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3awdkmtup.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gzruvegn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kfoowmxv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vustrxdh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3iebjqcgz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ekpkuyec.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vqypjvhd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3snopbycr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wpconxpm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zkteyrhs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vonmmhjf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ymdhxrxc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3swqiaoof.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yijyxouv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3azvsetzq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qgfrmjyq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vlxozwhu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qxwllmax.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dqngsqfz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3znlmpuzg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vwmbxrpo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bhwynicv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fwifwdbz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dudsiven.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ojvlluhk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gudumyeb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qjnwqnpc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wiulxece.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3uvghnvte.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qemkwjug.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3scmahjpq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3grjvudmr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rnyslwkh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3izyxzvhg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sudynkiq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fjkiolbe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3txtbeixd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3adlotwip.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lkhbuxoe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3drurnkue.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sjxkokeq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxqkebq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cumnjsgz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dtqpqzbx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3obdlnbmn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dsoqaupn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3subfwuwr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3viymvlib.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ilrzyzqa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nhtpqedz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nokbnhla.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3trhgrjrf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yatcsucy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3euanvfqh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hzudcqjs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lsyvdusg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bbrtvguy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3plugcoph.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dskxfrvf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kydtjnck.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3eszmpegv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jmyplvvp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqytmtlh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3velgztwe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qmkefuwj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3covrnxbl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qrurqlkb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fvybiqlu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hrvdakjx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3izhiirok.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3uygaquuk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mdbdtrua.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ubuhaotn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nptqglme.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgdomnni.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tjhpunpb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3oquznimo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3emczyvya.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3nbvcbeyd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cxesstxi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zolmvuqo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kbkwwyvj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yjfaviuk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mxmiggse.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fxwrbvct.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3szhlllkv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vkfvkjfk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jimssbpl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3brmiqxhd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ukmwqszm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3puzwisdt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cocguynw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3epmncjys.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hsreudow.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cjeukpku.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kvlcibxz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3onixexbm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vpczuhgm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xrbvmbww.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3yrxqynxi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zozywbao.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ffmrtkbd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmkqfabl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftgscigc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xszbogbf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mchkelvo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3hcrrrusl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zdrsrtfp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mvglfpgh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cuywxnyh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nlkmgmkh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lgfrmkgw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mlpjglzr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rbuxhdcq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qwjjxhof.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3pooqvhtd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvtjbtvq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3myjpgkag.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oeuxcnxf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ymvoblll.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yyakqaym.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gsrzvfsi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jzohoukd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mxhfkjnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jytudonc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zptlxivg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpifcoxq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kjjmolbw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bjclclvh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ckgepzxv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3howainbn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wnmiabsr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vktywnqb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3stffgvbm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlufauqj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hosktzdc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3iwvzeicz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dbvzmbji.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3navlldam.html


<!-- 参考信息 -->