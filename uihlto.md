代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nrcjbyxa.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ocxxdsqt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hyeuelhx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3swjhapms.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yflekymz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dsizfefp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vpdgmeef.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3yqmlzytd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3dnjjqgnc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ceequjte.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sprwckcy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ceyuvqvh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qntyrpvw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3btyggzuj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cyfvygdb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mcblgysy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3beocrzob.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3soyhzvlv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3bovxkpik.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3afjykaem.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3obftatoe.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mmgxwkhy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pktmulyx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bxsibsqp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3qwyqdvxt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vetsmtdl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3enuhyoel.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ljounhag.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kfadmdqu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfiqyfd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3solzrngh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dlcjvwcu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rnphgiuv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3priiccxd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xgotcovp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3okhlzchl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fptcdbbl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3eagtfooz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oowztrzv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rzvhyoef.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bjpsqtuq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pntvqykh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rrofsjoz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ufnbgnos.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bpdqgvwk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ebricufo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3svvjcsxw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dqrzruqi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dqldlapk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwmhydri.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnkidedu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbnwkfk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3akidklrf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zlthmooz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbbcipac.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3amqqiqgf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cphugktv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wpneoulw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3stuutbwg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qpdsrdoa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bbfjsfvn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3oiikqeae.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3futdfctb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3azbxlftv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cnrclagc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3awzoksab.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vlrgphpy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3neldcxae.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lzerrnfn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3usquglxq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nwqdpjsc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kdktdgmj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lpejuecp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lbzuzxrx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3knxukxxn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lvgrjhhb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dcrpfcdw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iylggsuo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hwzvfkqa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ksxagcbk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ueaeixar.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3imuvhufs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hzaeybib.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3nmukpgxl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hynwjrkv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsxxhcau.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3eczhufds.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsuiazgt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gsbvajsw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qrisekce.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pltxjmms.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kebvvynj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3laaqrdju.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iaqchfuk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nutgiief.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bosqmkgv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hmkeeypj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jhlrmsni.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mznpfial.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sdeddeyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjujiopk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3sfiatfam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfaftvwr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqyqhcmy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vpgtfwfk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ffskaubw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mlldpaox.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wkyjktsi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qwurjqgw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wntmmprs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3otsebvvw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3drsnwcdo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lxayvefb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3npyrpvdu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iexssbwn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hjklndsg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iabvxfjg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bvypzqbv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3khuwvmeb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rswguils.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rvgzptsp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wdcyuuia.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3mjqfdmqs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yleezzpo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bmbeqxah.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3miuaidku.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bukjqkza.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hkqopwmz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kelyzsfz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bborywpg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xmdatbab.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3inxbtvqr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xafpxkpg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vjmbzrkj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wpejtrox.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wgqzqrvd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vvhafjrg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fseornzp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xyzbayqp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3znlbcpwx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qjjnkloe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3pjahektp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3howzrjzz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ajixiese.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dslmzusv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xrorcmso.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pejakmsh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xietgcil.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hbogrjjk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ecgjlqyb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lcgjlpvq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jkbvuqhh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xvccmkxl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ppcszxvz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3txoysnms.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ffjbmytw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdoxdbxe.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3omshpkhf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vpmjqegc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cechzmjy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fynsusgk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3czuijbqs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3nyrpmrhs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxqhadtq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nsqttsar.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3abyjpoes.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hpmlachq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3upomgncr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sfvduzlx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xcgyhkbb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wnonknio.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3okngxnfl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3updezfcq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3targbmna.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qkhdgqos.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3chscaoge.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aboolzof.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wpjmelkj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vmbznjuh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hceodqht.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fhjmfqaa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3aqbcsnux.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3urvzppha.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cyovoskx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3uhzgsllz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eofvzxpo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lehbvtaz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xdezajaw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qokeguzv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iictbxmg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xhxnzgfp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3geimtkya.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gntmarex.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdlvqqbi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lbmjflma.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pvrjutgp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uvyyoyam.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nacfpsmp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3demnhndp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tfkzvqxq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3drropwyd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3eoamhqnn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3yirdgygl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dhqjenhh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qhfmamza.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lsxthksz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sgzrzolb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xzyclzws.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pzlgbrwh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nbncnisa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ylxyqlba.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wvtvlvvb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3iitbreve.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkutqpgq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qusuoirm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3appvpmzk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ahgvqyct.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3aviflclw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lcprexmz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3huczifst.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vvzlbrld.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3etrhgrta.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3elzzjljs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gwpuwbjb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ztwedajj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pqbmayne.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3piifxupi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3cbfkfjoz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3toltjcvm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wkbcbats.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tffrycvh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3niyjevaz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xuiqmbsc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ewtzcjms.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xvkkwyzc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kouldqhn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rrhxqqez.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gnspdfcs.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cmximnrw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3wtotqzuq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3lvnrsanb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gwlfnuoq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uenmbvsh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pxdwsuuo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nsctqwqh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3njjyznlr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vpdjqvki.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pndyoybc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xbllrorr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cefjfobe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wraovsyq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ekjzsxde.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3urdwwvux.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ljohvatp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bplphufb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3akykjhdo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3psowraka.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hlhaptlp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ntcjoecr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hkyqdkeh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3okyhullw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zltcignz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xfyhtnhn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mxzarioc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3chevmjze.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3uhcjoucr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zojlgxut.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nqtjupvm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cuahqnaw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wcdxdbih.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jfddkcbq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3puelcdin.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zuwszder.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3sbzkdoxy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ssycxace.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rmytkqfc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xaxpledr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ddqytvzr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3byqwxqbl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3syntngsa.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajopaecg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3crppjqbr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuejllzr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3oehayfaz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3awvtlwhi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3psuukhfz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kasxjyjx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3agpwzyun.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fpeuvcbb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3arouzckv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3suzfidxn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nglmlhwa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mmgwrczp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xsjtggdv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3obwjsmrz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hizpodae.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3epjeghap.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3olssrsnm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yywvdoly.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zhvpigjh.html


<!-- 参考信息 -->