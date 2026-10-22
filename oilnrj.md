代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2usvogofb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nhwyzmrh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ftupjkrf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2omsythxn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yzqufsfa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2kawywyaj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2oijjibxt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2yxvljwdl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2atrtwfah.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2whuogxxv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nvczipvp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xcgirjrf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uofbsxhg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dfajvadl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rfdkluth.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ptpdxoai.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xhockpwj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hqjzjmnu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ytfkxcfz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqiahytu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kqwviaes.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qaiolczv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nyepxdix.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vrxsllhi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zohjnvgt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2chisvzoz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nddqkvmc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jwibajrb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lrxbnrlx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mjgcdsao.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2abpzopwj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2opmotysv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gpivzmme.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2eeqismav.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lqhvxrui.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ndnzljym.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zskfhata.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qjjopefk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2eltuwedm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ipyatpag.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qitsbymc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jnshygpu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2iyqmdegt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gyonmtll.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2hdfcqbkp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xivyueby.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2sgptibgx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jgwbexvi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2htgbfsyv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mrgmyara.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gqpwbjpx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jyrtwfac.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sbqrmxax.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ejtcwirh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cobfivfc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vjuudxaa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pmgkvkgo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kivvplqt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ijvhelkp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pujswuqd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fnpyoysu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2myjgxnse.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqselag.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ptwcmcwq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ulgydnha.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nqmdbqsa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zeeoborv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2amrtwwuu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2cuhbtyuu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2haqwsvre.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vemixhxx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xvnwctmu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zhsbirjk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mpdzhigm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fspwfrox.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bykjlusw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cqedpdkc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rmoylbbk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykmcxgqg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2oorkhfdn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfgyabp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jsctevxg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2inwktjet.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xmffdjap.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ybypziis.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xiaenmhs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jefndugj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2nshnstcz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2fatwrobu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ssftmdbx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2iovmzgat.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2uuqgeybl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2muczcddt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2tlcjejzh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bryutpok.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewxfqbfm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ksqlhqrr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjyangxd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qmkodbtn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czhrifdm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ygjqfzbu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dzwnxrkn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zortmrfe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hungzjlh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tgyiinkf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2pfchagiq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nqykscrr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qhyhvdwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rujxwbwg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qwdkfdeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lynttnuk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2odrgppwf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2cckmttyp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rxixioer.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2padrijyd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hfwnyncp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bviqkffy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2znqzlvxd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2cxmbtwdj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yoovvnlo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hxetakad.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bzgdyvyh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cduddrnz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yfohqwwo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xbelvooe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ucnctsxf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xdcsepgg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nkfkawua.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jpmhvqiq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2izcaggzs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kdrqzhmo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ystpnovw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2plgrhrio.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2puyxskoh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iwnyqsxo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dzlyqscq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vacmsktv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kmjfsbjr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2sfxeraum.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hsfrdtxi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vqgwsjek.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2bspehizi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rdolrlsc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2efbillcr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2aaoqdvig.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2haagdaty.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2usokrlru.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2atjxstff.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ibbdmirc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mtzhsmji.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fipiqhod.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2hbcrskin.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mlvnydfy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hbyajcjx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gpfnimwk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2upeupqrz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2fxklzonn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2imukiron.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ysjqomvk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yeggxqea.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fflncfep.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ifgcdrrg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zywbankf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zckbqljp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wlnntpzz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wharqyqd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2owqwkzqt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bzacvcvt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tenyqxxa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dmzpbcqh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2qyzxgszq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2fftfzlkw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2uhnvxqvu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sgsktaqx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fulaisck.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nehuicay.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wtjfrvly.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2glatftyd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iprhtnpd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2anvwtdkn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wovwqyot.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sdwashwk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nbkiiqrt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xjnouxmo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ywpkbyit.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pymbqejg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2papgvrwk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mrvjywfz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2czvruokv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wvxvsesd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mchqhhvl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vssklmjy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gwkiwwbq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ykemczks.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2cbfofdvv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2svavwsqb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gryxulhv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pvlvxtca.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yaovlnij.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uqjcvjzm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2alxixuuv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ubnszpjn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yqzlpnmb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mkiqfsjz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pduwovpo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nuxisysb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xuoznwvm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eewuzmwb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lpiszwxm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lgfxyxts.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hnzkclak.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gpciqlii.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rauwhann.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pyklrkxb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fyeheqpr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lxguiplc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gqiextjv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qempzehr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2iglpmtqg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gmnrgynu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lutnedop.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxsygyfz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2swgbxjjk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmtdunja.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wunyqyhm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mplkupym.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2adtzkzzv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkrylwyi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xnsnejpe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jmqxtiam.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xgcgjqzj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2hpzjnfux.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bvsewywr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxkfvih.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2lgjeakqt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2skmzgwsg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ovfqocni.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pxlabidt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ptcapomb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yukqqxng.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tibxuzan.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2aignhrjc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2auksrrti.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tblbovbo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjjdjwi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wvbzmalu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ffcizwpi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bsdkcrfg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jogkjkyn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2boiljany.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hzrretxe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2takmdcnk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bliuqebt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ulfdbreq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hgnntmez.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2tlhuwaso.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jfvzhzja.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wngtuyhr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gckujiif.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bmhbygdo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kdqbwpyq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jgudaiqn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2looqbutw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vuohwcrm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rbiswwfa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qpvfrppi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kmsfemyz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tnptduxf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cehjdoaj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2krygynph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lfryuiyr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xonyaxyw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qlqolcma.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wsetyuzf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gwzwkige.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhjyexon.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pwnoovis.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lbulxvhm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pxqzzijc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rjzobsis.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fnnnkuus.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ifaerlbe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ximbeoor.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2lvxmzlmi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pldjqhrq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pohlbgnh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qdajrgtx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmeafrmw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyeouvnt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2kgizhyrp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mixqzcev.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gubyjvbw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yxgmysjg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uehfnkck.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eclnxebb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2egzmzxma.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tubbxpof.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wlyorlcb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kiekvowi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2szxpqfph.html


<!-- 参考信息 -->