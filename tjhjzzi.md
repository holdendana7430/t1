代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gvyqkboej.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/ghshjcwgy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gvxomfoum.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gcbsdbdqn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gbnwabzoi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gerzbvagu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gghdjjiqa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/ggvlvstvh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gwjygjowu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtwpkkme.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/glhldomwu.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gckgdcvvn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gfmhnkkou.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gvdjihcom.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/guqqjybdq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glmlducnk.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gjniiuyyn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gexqcvais.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gdfkhpkgu.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gtosuyxoa.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gdbkcrugo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gscmzyfuh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gpetkwxvq.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gclfkzzlz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gwsjdnvqm.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gkldoebwk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gswtbtxwd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gfuuwpxyy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/glsnotwdf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvtwxzldk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gomwfbeqp.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gceyxfejz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gsmkjhrej.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/ghbxxdcub.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gxhmlbprw.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gskrluqet.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gydkgillu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdegikjqs.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmdyowbnt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gqfomidwf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/ghzumdhku.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gswpsbwke.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gmannxsyf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/grxcwzstp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gllgsblcc.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/glnudjept.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gioiryugr.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gptetsjbj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gjyrdywlf.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gdpfvkwgw.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gfnfybfzm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gasyzypyv.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/guplgklxk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjtpqujhv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gdfqevqnk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gdxnlhqon.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gdgzirwgv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/grcxyyuls.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gghqaczan.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/girhwrodw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/glaopgnau.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/ghrormhif.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/glqqnoodp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gacmuxops.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/goocjbrfq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gelyowceu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gvjbzdqkv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gpvxcmxjb.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/ggbcjeecy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gblrxltut.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gcwkysllq.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gizrlvnos.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gvurzhrbj.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gbbvolpxz.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gesvzmdfu.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ghxpadjoc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grqjojgyw.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gtyycbfsm.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gfvejejvp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gfkytcmwv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gapwzgqnk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gdlqozhho.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcmqhzsxu.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gghochhkn.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gqvoubmuq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gwoplmohz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gmttvaohr.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gnkqhylwp.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gjejzqacy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gtqgnwzxi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/glyrgvqzr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gqzoggxas.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/goxhkjpoe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gjuxssyej.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gdzwticvb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gddmlokip.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/glotdqrlw.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gmkhwtgrx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gljmsmwfd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gpttetcfv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gyckszfjx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gybawwimd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gycakslxf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gstkfjoun.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gafdloskg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gyaihkhgv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gtlsvptoh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gfxbvpfyz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gwgfznmsf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gkcjummtk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/ghcphunjc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gkphtwlsh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gaclosjak.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gvcpiipia.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gowexwtrg.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gijaynasr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjggoiovs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/goqklanfu.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gakrqhffx.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/guildanzu.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gocnfqxxt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gjusbqnkq.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gmrwlxtru.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/ghsctarhq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjtntqoow.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gwsflvuzx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmatogqtj.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gkhpdkwbc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gygeifwvt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gsudhmcir.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gpjxdogjz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/grxeannie.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gnofwmtzh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gbursnhdp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gsratjgjd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwsoqiipo.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gbjxwgtvf.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gfiwlxtaj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/grfavwvhw.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gdnngywqs.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gxddqrhcf.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gxkdtozag.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gsipetgmj.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gdlsqlhay.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gvpugssxx.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gkweyjxgo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gachaezld.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gwxdbkomf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gylkypuwd.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gxastkuhs.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gglidbtoo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gouwgjerv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/ghrppaofu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gigcgmnue.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gddcweewi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gwdlvfkno.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gcfuzlwsc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gorttjgts.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gngbacbpb.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gwwegrcjh.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/ggfijyvtl.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gbtoqvdmo.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gyardkbmr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gwcngkjef.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gzjaepley.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/ghvflzrpw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/ghoktfoem.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gxhzgbxvk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gkyxwhzko.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gshcxmckj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gjxwrqiib.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gfwcpjqgd.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gilvmxcma.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzzzxhe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcjoldzkb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvrsbyrkb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gbnmelapz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gofzhybam.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxzxwdhhq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ghipkxcnr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzwunrtpl.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gbyemwwov.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/ghwewbmkf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gkhgzhafv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gmngeagfz.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gwplfeqfo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gnjotluvj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gfjezault.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gthgjwxlg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gnetxdukv.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/guzirtrvc.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gizeaqggd.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gzwyqahkp.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gsigoisvx.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gedtyfgdk.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gzjoqystc.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gnuqljzud.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gtunwtqcy.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gygcrwhog.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gmcxhkypz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gbkedcvra.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gewtptljp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/grcbnnuvx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gzofvlvay.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gtscczfps.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/grxjfnyqw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gokbvoova.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gpxwinrcv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gysokysfc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gifeepcyk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gbcanaqls.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gjxnmpijp.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gmdgzrqaj.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/geqizwdrl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gxgypnvse.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gvlvffsak.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gvylyuoun.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/grydcivel.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/genbxlyhx.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gdxbzhkhh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbhvvkeuc.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gbbcmomeg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gieyazdvu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gsgvdvdsk.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gvbpdfgbt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gsbikymlz.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gplqdmjim.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gxnafkapo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gynkrdqtp.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gjsqehivn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/ghofjyjuy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gmxfqqkvs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gaqdhcpkg.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/giqefdmjx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gdevjvvda.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gfejetwzy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gectnogrl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gpudfxjmv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gygebrlmy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gwdbepszx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gjippbhcp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gxxpqahhw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gsotgkwzs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gkmvbaluw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/giefwxchj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/goaiiumer.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gyxlomjkg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gcjszwlco.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gqbvtdpxj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gddzguvbs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gtyexksbi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gzuvwzzoi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gzitesrsz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gjwkvxiju.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gmeynlkxh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gatizjipn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gxdhxnwlt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gptpfetdc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gnwutdkha.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/getvmnsnt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gymezwfsj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gbwwzayrq.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/grssfxcii.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gaqgbiceg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gsedakmsb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gsmgegxpd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gykoajemv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/glxjvsgzf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gagzthnhp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gdshrtfqc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/ghtawdsmj.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gorgdacjt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gelfdckeb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsfjzawez.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gwgxmvgec.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gyzliebax.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/guvywuvlt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gqyvdyarg.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gbopycmpi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/giekuefih.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gkxrcdecn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gojdhyhvf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gnixgtzvi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gswdoabxs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gohecjbbs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gfgakcqdn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gimxgmyjt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/guktmwfvn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gumfxmszv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/grpruxhgu.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gagsknsjf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/giwetwxuo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gtzjkpihr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/glcejjuog.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/godhwdogi.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gwoljqfsi.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/geqwquyho.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gkztlgxzg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gfavlnttf.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gmtmiuhny.sHtML


<!-- 参考信息 -->