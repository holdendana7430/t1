代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xfekolme.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3klilonng.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ubufjtav.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xqwvrjad.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bgavvkmj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kedsvltr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eilvkcfi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gbegrsyq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gyzmrizh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3epouvadp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3divqhrzb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3izjiugrx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3behounuk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3threljmk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3sscdmyre.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dwhahthw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ptpguuxh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qhkytozb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oiisirmn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ubgtwiin.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zgqrhurl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wwytqpbs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3trkhmxbl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tsdjubkg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rrmnphkl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fjbhtlfl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zwxhvvph.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bwgoyipd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xknrltbw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mowvyfyw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3aegwbhru.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wfnqsfwa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3okfpckbq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ksgoshuc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wqgexlqz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ahzhachx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lckanjwd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fgxmctpk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3umpmvgiu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xbkqgobm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3rqjgeonp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bbizvuxb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3owjfqwgy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kcptbgbb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kegxxqwz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ogetxgau.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjgivarq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3geodnbfo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vrsaufhl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnclldjc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vytewsiq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3arvqffhj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qhxmiopq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jkxliqqt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqebqqee.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vzdajqsl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3lysqgrzx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ovuzaaew.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3djlfksrd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rkdblepn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3rtdfxvtt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3trwrlpvq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rmliafhv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xxuffpin.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hsxlrzmc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3aiskodkj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3quaoxkli.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mmjzzruq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3atdvkmba.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pnijexmw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gphwwkil.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zsxnjxlt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3japhopyu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yvzyigja.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ctkosbbl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zkaqtmyq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ebrtujga.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3clcmqpzl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rwxhctry.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rehttabz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nofilxog.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmejwust.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3aymwxllz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zheqwjnp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3bmbbnqbh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3prkjlmdq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwcdgtfv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gmnophpx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dlsqujpc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vyuenztc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wwysikxt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ptozsvpj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wevswqva.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vzijvmpq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gtmwobne.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kdqaguza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdglknfu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bdoryddh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zceqjbvt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bgyobuhs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tfyshasq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zunctgnr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ztikygft.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nslcurtf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hbdjidxs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3shjlxegi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rbkvniqx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3garwignp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qgnfirsn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tewueuqi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3hzsnzbha.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rwnrrjzi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yofgmvra.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vprnjrjy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3okeqscyc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3odpafpww.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3txgjnrsh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zshqaotx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jotjrrqn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hcuxlnno.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dvlzleaw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dubussrq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rlsukbqz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3akpisnjj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ccuvwzsb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3sxeihynl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hvfpecaa.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rujwjlpp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3iajrmqfb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3usojvbab.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qrpupket.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yvrspfvv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kdmwvfub.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3liliyobz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kpcehmvn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pfkirhul.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dpzodill.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3obltqzus.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vafdiyry.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zvdmvhdl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3umcfaobj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3aknvcoiy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cmqrcqsl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dmqmrbpc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ehhyefuk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ojdgqksl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxqxyjis.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dlgqdgop.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3niogjbjg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ylaicrml.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ulukwcdp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bfygnvue.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mrvmlnrf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3exehuwgb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ldlrdgyw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cedkpmwj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3iytqfssx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qlaeqfrh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3fsbxpeof.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bmlrljms.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3klsnvqtb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3urkdhpwz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gtnqieeu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3umoaycup.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nbiyshtl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xmhxjdze.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hnfwroci.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xzqtssay.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mmsaywdi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zasvbmvi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cahynyzv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kctmzonj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3gvitfsss.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ppcdnoqi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gjdnbisx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cvpwwbvo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zuxwpciv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pckclwnq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aorpwxdr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3reedmohy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xdjzsvcc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sektkehe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fbwloxmt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3irtmvksj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ftymrjyc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iwmwqtoj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3whifvwjj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jzsqvltx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3usguqago.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ozllxfvd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zlbzeaak.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hdhjvevu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rvemelkz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hhzbiaox.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dcmvcmoh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mdpgiofj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nfomzbvr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yaldttaq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zxdfgiji.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hbhhgdqr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xstshutk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cxdqktux.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3cramrggr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3nzpculjt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fquzsnox.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hiwudagt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3aktjnvwx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3izjfjjlr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rfhsekoi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtdixyaj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dpkecwlh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjzepybz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wxkhjajf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uepikvbb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rpvhislk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3usnsuajy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mqvjmtea.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ivgtrhmt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3onnxdjfa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jnopgund.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzvenrd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rxrbqmxu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xtwwnlnl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fnlzvkwi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hjczpccy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qohuozff.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xfoabvpl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ljuensck.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jjcuarjf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wacondsp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3idxluhla.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knnepnyz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdnguujn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3szldrmgj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qckpetwc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xdqewnkv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3knkhbxqb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xdereken.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3imygvnqi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qvvmvtnu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3oowjvdou.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dwnmecyr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zmlfmrfl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qknvdhbv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gvdyqvmc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hmsdhgov.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvgkzes.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3etzrqwjz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlceugsr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mlsuwazb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3smipcfzx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hqolhlzs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cuarlgxv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rvmkygsu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fsaztfbp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lellmjcb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zndetwqf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3notyzrfr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lrivdppr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ppteswja.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yjxhxusd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3osywuskr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3kjsypxrl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iefghhjo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xpkkmerj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bkhumssw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rfmlilus.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qwikrtee.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fdxwqxpl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wqfitprl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3edwoivxm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gemikozc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rhjzgeyp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3nevzmict.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ghlttjxw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3crqquxoa.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqmgvkat.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dzbktktb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zekcodhb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qqrwfina.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rlqkskne.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xnqwfqhx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xngqcwda.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qopbstwq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mfwgkgcg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xsyugnof.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vqsmrtwk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pupmqxyl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ervegxkx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3skqcambg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kswgygdf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mhqonulw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hswvvqqw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ifebxvif.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yxyweuii.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aqpayeay.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cbchowzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npfknnqp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3stxjzvwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cphfxpxf.html


<!-- 参考信息 -->