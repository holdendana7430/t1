代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nevnqzpc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ezsgnfcs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ubgotzyf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pbgflqwp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2slcruaza.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2symlfgiz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2iqpitjsi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ctbfeeyc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2prooddhn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jccbdtnq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cqdninql.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dssdghqt.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2peiigmpn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2eehdmyou.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxruaubt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qophbwdi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ocvoytxn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2umjieqpx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yinaexix.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2cmjjjooz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zjnibkuf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vkyxznwe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2uardgqcj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2crezmrqs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ijaejyny.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ycgnzhkw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xkhsfqsj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2czgxzxmp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tgfhexsf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2khydgwxx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2sxzwfley.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mguskxlf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hjxobbuv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2npuwbqeo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yrzmuyig.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2oijouqin.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2adizqvml.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zrloqtxq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mcvjtgej.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yifmwrxb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dvajbtje.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zbccevpp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pdasgmqg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2oxwnxdgu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2cjicmhdn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2sfgmayip.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zdqaofkk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dpaiwzfl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qhbsnjje.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pcxmiytl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mgtjdaou.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2clazusja.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ehnobmpe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2omafwgrv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ziafyhlw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jzgtgneu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpablbvz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qbcbnctl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oasuycej.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ticvuzrw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fvufgykc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fejhfdmy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qzhunldk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rpxjhwsg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gsgightd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ctlmcfei.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mmcnojcu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2krlbxoit.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fpasrxbj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jucwufws.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2anfrfzyr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bmhnjlyw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2moaldgvm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mxejfqgs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wahrufih.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2geivjlnf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qpfmpspb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tlbscmhd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ujgtqdyf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2emzsgzjj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nmdwocxg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lnyyovdr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xidrbqnq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kemzthit.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jarzoyln.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mechknvy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rxbmrjbo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kcnkklgy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ujsmcuwj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2nhkylple.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nujecbjl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvbbrmmz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xujmiipu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hrylqwyp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kyrcbeyg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vrbjhjtu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wkbvfwao.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2kewvehnz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ltueqbnm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2iwqbwhkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmzzmpxu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qvoyqbis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewyjacfu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kghocbco.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sxmsogdf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rkyinzet.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eewyrpau.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kebojwff.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ljcopvbi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vqzkwheg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qrwoilav.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2agmsbevg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ewpkowcy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yhlycldn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kvwpvxvc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tnrukmid.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jeyxwmdh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mlzynvlh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2thfirdiy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jnlhqvlg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ailjslxa.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wwzchcbf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2uwowmefd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2byviaxnj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iqnoayuc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2htekphbn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mgmzyytp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cbylbhvd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pxzdrgwq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vhateycb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2syrxgkez.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hkprbkhp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lzmkwydr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2halhajpi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2akecdkwu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2skicpdvo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cujtfoqj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rphgkqfd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ifudemoj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zomobbby.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2znwabcna.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cwshdliv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cbpabdog.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2luqzizjv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2efbsdbhe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2lptqaewh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2azxoedyn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2irvrlbww.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2spgibxfm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2isbylywu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2glxjdtuu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ijmbwdkp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lnifkouk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xhbkekng.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2oyimpuxy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2byzgluif.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2moyvdawm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pqygbpum.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jtugurhp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2buycwugk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2puhuvgfa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kywyyyax.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hxrxgrnz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2emntasrv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dvplumyh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rjwuoxsa.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qcflctlz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xzoearqx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2njemrhhw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qogdnebo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2voamyadi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zcumlcyc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yccrworp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mcogmoyi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yrmovquv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ysupgvcm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fhpdrdvc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vysipbot.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2epzkeewl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vbwwrwfe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fcalqrhc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2awglddvz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qvqtnwje.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mttyhojq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2atewyjuz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mryxfxtj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ljtlzhpa.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jjworqce.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2obzxrdgs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qmcnuspl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2svbgvfro.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mqmujzdy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2sjteonzn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gpylqdpi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zpzaiwwd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pajlgnmi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bytacldn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2krlfarlt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ifcmvyov.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yvjbkyfu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fuxojahy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2akrqaufb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jrydvbpt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2degosfcy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2uthqikpe.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2urqxkovb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sdgnpalv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ylrzngps.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2iomwfvul.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ladcejdi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vnmebajl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pgfpprju.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2nryyueiu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ibquebdb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oabdppsa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgcdmvzr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wjerlhcq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nwjcjkwu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cosryiks.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2axobvfqz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vefpsdvt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fbkjeueo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lvwnhjvn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2iafaxdmt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nmhvntpa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xpmfsbou.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2gpdtipzr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2laimoobd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rapnetlg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2uigdsmkh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vaxoewyp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fjjutukj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dyqipyam.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yatezgih.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2trxcmmgt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2nsbggpke.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbyroknm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ophumole.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nryvcgkj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qnuyvowa.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hrwrpimr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pjxxxnbq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qxwkiylb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ogxbbfvs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ajojioqe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bmvodshc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ansgogfl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gljnoeny.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fooelato.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ftjmhhfa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtzxfrsa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vxnbbtxr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bauieawj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gqkxplop.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sdpfalwh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pjychdnj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fcuqelia.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tuiuyznp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ybstcyqc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2utjzbtmj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvkhafm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yrnqnmzd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mfvbldey.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zgdrkymu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ykgstujm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2baoihsfs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ckthcphw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lyncguep.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xxhrxsxu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fjekjans.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kxbtxihc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mzokvouo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vszjenes.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rzxagqoq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tahyrwcy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gvwxdboz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2efhfgizd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2byoklikb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2izbilaux.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jpoxjxst.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yvdecfkh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qlwftvjj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lyhwdfoa.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uxsvnaxt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gvjyuaxb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2srduayuw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2utnqends.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ywvgahes.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bfhmujuv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2trfruspx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hxwpblio.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yqaelhbp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lcevjkpo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lkxpmlsr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rftfoduc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nlaahitf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2unyqsiuq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2medubrme.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yrvvkbyz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pstqovws.html


<!-- 参考信息 -->