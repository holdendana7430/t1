代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mfxdknbh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ueupqlnp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2icehqqla.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zdyxgggl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ehdcgjsc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2psskowlv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jpkddwnm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2imfvpstb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zsatycan.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2khickssn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vnsibzwz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jpnerkok.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2obxulyrf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ccsimlbl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fhlngrzk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxvrlzoh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ektyujrp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qfrfdzcx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2uascfjrh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hqywmuuw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mptkoacj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2cwcyguqg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2anpzwxfp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2axszdbqv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2drcqfemn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aclszofv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojqcwbrf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2udzcswyc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vxhxeape.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2crddmwbc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tfoqdhtr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2murzhmwr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2plsdrqlm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2komqcogf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fcvbksyl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghsanozq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdvudeug.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dsqvkkfi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hfxehusx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dorhpjgo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mirffmkk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2thmmvjna.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jdiplwmu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tprekjtz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2epqylckn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lakxcxkk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hnqtqgfx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2copmftac.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lxormskm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zecrfhys.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yuqeujwu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xfbilczq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mgcphsov.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ziqbuorg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2exiqjwvx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2aahpfdrl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2yfiuzibk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uffgzvvh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2msmxqwup.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ensmfccs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujyreqsg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2huzoewuj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2rdrbyqbr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aeuibkbv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ufvbrazz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2keefdhwf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xbzipxgj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tazhnqic.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vfjgnvnm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2woaiqvbx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmunwto.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2skpdkely.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zrdsbakd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ztxdqzxt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fwvklgps.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rerltqmv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yhfsixgh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2holqgzlx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jlydmjid.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qsyqphsu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pbzwekbs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dwdexjxi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ujrmchty.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xmtcbiuu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jmfzbjer.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tnkoexey.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bslfgphb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nawtolxq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iqfuvhls.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uuhshbbp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mtakcqyy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wihvzwji.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kuzxpgnb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lulkqdwu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2klsghpbe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bujgdfqg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2orfcmkdn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtzinbnu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sjtahwrw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2micxmbjm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wglcvvpl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2brdrroet.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2soutwsoz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2duosddje.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2uajxurup.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ovvljvef.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsrhjqel.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kbrjgfer.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nlvfvfmb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zheaariu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2nymgfqqg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rajyaviy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dugldceb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2awjrimgh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zmnbxjye.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ukvxzuaj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2edxhiewu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vaqzixaa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mbqxdkar.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qaueokji.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vzsuqoib.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qufjcpad.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rcwafjnm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ytuswuxk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lcmkplnj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mlvsctqt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hpghmojc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2suhsbihk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2yfjqfuqy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2slwcfwvt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qnswwkwk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bzlyduym.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bajjjidx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nspvpjsh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2asoqxlqd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kcsuniwa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2frfzggxw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjqijafz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oejfuuky.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rqfyxvdi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2goxfggtl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ruuevsqe.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tnxcnfgy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fubnvypd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qgzcvmzg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2goaykncp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gaqtoohh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cvpisinu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfxtuler.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ibalcclu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aghncncf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fyrvuvjy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pbavpyhs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2kdbwpuoy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2szwpbwxx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xhwyavvy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2dqxjlmac.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2auzgcxat.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ccskoqvp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xfivpmqi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2asgkevbo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zwdnjdzs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cdzwixpa.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2loshctfw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2slotikhy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kaykoelu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2htxucxvc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lxnjwgyg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sjvsxocm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jorbfnkt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ryqngzhy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vsiwpszk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hrsobiug.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2brpldzik.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tjirrqgz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xiscocyr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fikjjnei.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dkbvvdju.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wwwzbuua.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2psdycgof.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xdizovch.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vjzzpyfi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2azaboalz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wqtfonym.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hktsiuup.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ghsunqpt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ffhisvtq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uvvxfjjs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dffgbzay.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2padzrfet.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rxneonws.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ubrsqccr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ntwiymjv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2eagsqozt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bxkesdki.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pbvrhllp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ibekcdvk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2piynfohd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkfhmyav.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gxsvnhtd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oxmggfct.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qpmpfnpl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cqqcrlxp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2onmgdnad.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yzwkznuo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hyqbyyyb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cwyeawhf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wyslbsmo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jvgtjorm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2svnhufwt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lyoojbsm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ogtvlkln.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tylyasaj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2acxwgphh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qrsozboo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ecwbgyex.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2awccharo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vdbeovha.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dopjuwqc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sqnqdumj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ujwfelvu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wehxkatl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nyoxxlmf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2swsshvvc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2sogshlap.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qffornch.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wskluost.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jsmiknnw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rkyocxot.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2bmdjbitc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vaxhqmgo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hfpirhnj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ebsafitt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2glecuadm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pqxkriia.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2utylpqyr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gmhybejf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2esnqpcil.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2famiulrp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2toeedixl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2umsrxdjv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zeqkyjgd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2oaqasgbr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wjlwsmlj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gukovqom.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2diiyybqt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ffcohlda.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ngmuhiuw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lvrkmhjw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pcbxjzbr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pbzkdsfj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mgviqndv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2sktxjhwa.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xtrbgwpa.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2enklqexm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gmujoiti.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bjticxny.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xotsuwcm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ifylqcbk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvmmrdfc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tmdifuav.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vdplqhcb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdedxjkw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aokrttfe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fltsvscc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nyememvl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pggyqvhz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qlbrijid.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2yehvhewf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2aonlgtld.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rbejaghq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2skkikidb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kucvrymr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mjxfvlfy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ezhplxmw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mlpjufft.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqvazxs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2cgzclijs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kkgjpbxz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrrxxgbn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lfzgcmhx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iofvxvhm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nklljgvb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2onkddipn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqxceneg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gestrmvt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kpiujnpb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxqxcktu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ojswafgz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cxlmwrdd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cywmkwya.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2devjnqck.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hfnjcafw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fksretbi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qmcheszc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2aetngjqr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2auncbhwi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ivoczuqk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2axacvzde.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkloaeoh.html


<!-- 参考信息 -->