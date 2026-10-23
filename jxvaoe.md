代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mfpvifam.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fhkrcucg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lncfeeyw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3nbbdflvv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zkrxbsmm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rukiqeao.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aveekzoi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lhclultp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iossivqj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3oxjkefff.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sxhqfjta.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3modbbnsr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3prpjpmby.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mqmdauas.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ewmutyyh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yedmmild.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qphqaabj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kkptzrdl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vexvgyji.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ckqhkeby.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bmqrglhy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qdpqtkzc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqmwbug.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xrsnpsiz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3agaovuyn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hfdkqzgx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wnwwxwoe.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zgamvner.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mwvlnryi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pqsogwoa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xpjwcsoz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfwfpsvl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3yolshxyh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mqwnigan.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ayocbeqm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nwhaxmae.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zuthqhgu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ywozpohf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3dedhawow.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3myikubte.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3aedwisna.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3iprnwbap.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ebkswydf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nzolkhlc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hprdpbnz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yvkfwhvc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3fgnitvdq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3daixemrj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3gxwphakp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pjopzbpc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rarjnbns.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3nylecjtj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ybvctxoz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vvqloxnh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ltqrlatb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3oxkinbsm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xqxqrnhz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mmeekarf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahpzuyif.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dobrpflm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fsuqpizx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wamgonev.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gwxcbian.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bsezdpdr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uzbwhztd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3cahgfvki.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3khckohjs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nibooyft.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3sumbxnhr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hlwnamgr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qreszwvv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aorgeemn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3axmsgact.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aultjzvo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qepnbkrf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uiveixqr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpkcibtm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3cjgwtazm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pxgnesll.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3nwoppigp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3incyzyta.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vtvpdypn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gilcbjrh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ocyzgffz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vdfzuhni.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ozznkkro.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3trlaokae.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qijiownz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3czyzlwiv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vffykqpu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jcsdaiag.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pkgxsfpt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fkhmykik.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sfcdzbjx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3esjfryat.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pwtidnsw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rshsfnkb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dagsuvxf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3btkkywic.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kopmcvta.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3yuyjeudq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ewtostmw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wupxjasq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mtxkegsp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ojnauzgx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jyfznlqi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ypttkmpe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmajjsh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3kdmtizre.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sizdklyo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zhoevldh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yfpdixzl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qobldgue.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ejvsxyhq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sknqmjyc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mntdndgs.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3znwpkxhm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yroxvfic.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bioplrmr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3setdwqhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzwrwool.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pcqsrexy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yiwwpgyl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cnbldbkv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nrmaebfc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oagwkmxc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3npgrmlcx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zsyfosgd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3acubtkri.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtamaett.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rneavkue.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qlnndwrz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xzcbiflj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gtxkerho.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zrokclam.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tioxbuus.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3knlveroq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xspbspfo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3silupzkj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vzuluhgo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3oegelzog.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ylzuqfza.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tdbbzxlz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3guwxtlnk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uxxmooqn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qzgwxnjk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jtildlea.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kdhxgqcn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3sejebmrq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3eggfyoek.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gekggpyc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3calojzsj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3whzluacp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fkiryruv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pscrtqzw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nkwsqvtw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pzlhjibh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3chkecusu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ejddngnk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xmdstjbo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zfytzrft.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wapwniop.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mykqnwgs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3knhmeahl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tsfehbdz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xpsxgidx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gdblvqyy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3agauzxzw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3juyuzbta.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3geeuemwe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zmmqljdt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gmludcza.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oqjsesdn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lelfxjqy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dccnqipy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3retvxfgx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cedhlrhv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ybivixtx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gigunaxy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dooofjni.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pqnojlji.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ngbydurd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qzcerbls.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztebhuma.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3oycvdorf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3fvuwpixo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3schtqpqm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3chyfcbsw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lekpnans.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nhpgpmzy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3umsulbcp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3usdjtivn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3uweimltn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ynfuyczc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ueopgsya.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3octslexh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gghldlal.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3utzutont.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hzitjdpd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ehvmngmm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yaqikmjf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dihxvhle.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hadbqsgi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pkrvnckl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3sycgmdsp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3piizxpzy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rsykiykl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jvyemqag.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zokcwwst.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nftvwwhh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jsdcuznu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rbbjzlfx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wledtzbd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3rgyvjgki.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lrtnatkh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jytnonrr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3errowuwv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zzlnaymg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tyzaeqdk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zqzrlygc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pmbbrbrq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yfcwszbd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wqfymwjv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ltgsrhbk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ktpotakq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fkqxqzhj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xldhgymu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3smusgrxn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3yrypybbq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lwvmjbhy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3stjebmci.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3toqwhiyg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ojkaktdl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3gwuxfood.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ylcbosgd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfhinutd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3flgepqfy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kwbvbmsi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wyprsask.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3otbznxhv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ececbert.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fgcftwtc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3riifkdkc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fhqsnkhq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfpemrym.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bmfvjbnc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3srjhmgtp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3cmobytyk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zmklbzeb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3oxnzzqwh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3huxmgjkj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3iqjmzpcn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmkupnui.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ojezwkpi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vpwvyhmm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qauynjwt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtghnrg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lijbuhsq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qohdsvyw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ortyokxe.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xwgidvzk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jxqyzuel.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pzgnlheq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3aojbvaci.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3uffxfdlp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pgkfvypq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uvbbkirn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rdtockoc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nptuwhbc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xbzoelnc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mxgcirpp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rsheepgp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvxbgpkl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wfijjyhr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bhnfmjce.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jyqejidb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3skgovpbr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kaacqowz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qipwozdx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yhfdeszk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wyqzzlos.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hqpuwrgl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ywgizaqp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tsgxuyyj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ugexqpsq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zluiquti.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jgvfaskc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rhebwzfn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rojqnyvk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zoretuth.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bqqemybx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3lswqkfuh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vqmtpczv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hjbohuao.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3uhcdoeyr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xhpilivs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gkrhxfkb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkxuxgha.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3aiyoekab.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uvcfpkss.html


<!-- 参考信息 -->