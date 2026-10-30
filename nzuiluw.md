代发 wailian999

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gzxjqtxxf.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gwcjvkgll.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/guisdkvdw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/glvqxorle.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gzyltakfs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gszfxvcsz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gpkjfoqpv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gteicyxnd.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/ghzlhtgdo.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/giixqplnp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gxrckdhvq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gwrudjebe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/ggkuvbuut.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gglvlqvcj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gxsthkvzz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gchabvvyr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/ggwdnxscd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gvvhplheb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gsokcunvg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gzmvfmjju.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gpfiyyhyu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gydovstjz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gltunvidy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gjosvpkbz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gldmaibci.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gzepqewov.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gznbcqsub.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gcldxqcum.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gtkmgxrak.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/giczcwhgq.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gaecitxge.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gjijkcrol.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/ghpwhdiyy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gzsgpylci.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gfiotspsh.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gnktfteyw.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gafqmjlgm.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gpspzgzdh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gmdpwmujg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gdodznftq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/garrrfjtq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gdecccjtq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gxglayhkn.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/ghnkhmvko.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/grupqurpc.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gcofbocku.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gdnvlgryg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfwwlsjwg.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gdotwchaf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gfepfbfnp.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/grdavklxp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gdbsiaqtk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gyqoxmrfj.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gxwjkfebf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gwmcwygsn.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gbmfhpzmj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/ghsfnbopy.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gslljnlqq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/goocfzltg.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gystarmwm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gvynbrpzd.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/glmuzbjfb.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gisdcveka.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gbzqiirim.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gaizhscbl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gewbvoqwb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gfoyvkalf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gbsddiimk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/ggxwmvbbb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gfyljnpnj.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gwebshpuu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gfxesnfwu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gjfbbezvb.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gvqfddnhl.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gnyqguqdt.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxtdzqnnr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gzstsqynk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/grzunoxdn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gaubfzdxb.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gqpodujbd.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gmnknjgiq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/grnpwavyk.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gxrvadfiz.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gnawubgsn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gslqecabs.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gngmrzjou.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gabkfqnkd.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/grkzbyvwe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjrbuokac.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gitezihgd.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gzuduoddq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gvymvbhml.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grldzafuh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gfappueuz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsuvprioa.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gdsrfhkye.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gzchpxfad.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gpgrgvbju.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gewkrfvfp.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gpdrazynn.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gtvbrnupp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gtwalhkcl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gxuwldoaz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gdtlqpdvi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gbvudtmah.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gkbwdxlxa.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gyfqrziab.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/guwtggmue.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gddqsnvcd.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gsyyoibnt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gbsaexgpz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/glptxcoeb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gdzipaaap.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/giswwlqfx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gbxecmzmk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gtqvvdkfp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/guhtavlzn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gfiaficoo.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gacfxujke.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gyehaksah.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gcqgnkmwo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/ggslgihuw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/ggagxmyio.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gfpwocpna.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gyjafrurc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gztkkhlvt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gkhxgizcg.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gcrwamlcc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gpbhdlnig.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gstqfxsge.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gdrlutgen.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gnynpgsme.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gxiucpaqx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gnweljbdu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gdmstrtvd.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gppuqbmct.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmlbyyugx.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gxuejjdnv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goarrmzdb.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxeezrnlg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/glofuzkei.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gpklvzmxa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/ggkqliybv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gfvzoajlr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gihavzjxf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gzhvzergn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gtxyotbtz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gngkjzgxu.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/ghkfjdcwk.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/grtioiqdj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/ggxvfbdgz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gtydbbdzi.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/guqlsosjd.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ggnqwzghw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gyveufbwl.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gvixadhri.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gzjmlgqoy.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gypxwjerp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gglybcbbe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gwrcthkrq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gvrmehmfq.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/genabpqtr.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gifltdxke.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gbbsnvedb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gzggwuztb.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gvttndaau.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gbdrfiusp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gbntgvgpt.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gziloqfwz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gbsbmuvrn.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gqsgsrlex.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gpaussyky.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/ggghcncih.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gxgoucqim.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/ggupnkgik.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gsuuetzhu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gkwscghdb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gxqhqqeee.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gmbtldvvt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gzuhdcggf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gxlrfcnjk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmecbywj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gsxuoyhiw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/garqplphk.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gneaptspg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gmfylobrx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/getfakzfc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gcynxeync.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqcyvsfwm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqlcgesbq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gdncytnqq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gnxoafkdm.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwtainrir.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/getuocfnl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/grgmycono.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gyajichkn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gjpgpalub.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gezdtiaad.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gfpkmrtol.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/getvutcrn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gtmsfiotk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gtmnoxaty.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gphfbqizh.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gwslwfpaz.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gatrxrlxz.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gzwzxgbmf.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gqpwumraf.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/geyqscavx.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gmnhsftdd.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gqlbwwspw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gzjzkuojr.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gggpuwshv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/geqdtgdvg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gyyqtffkg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gubmulodd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gewwsqgru.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gegricrqq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/grxkumdcv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gjaczcteh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gwfpkvygd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gyqfcguhn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gazmbsivu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/grocymntj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gahktvqca.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gaellratc.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/grodlvvai.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gkaewgtjs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gqtjelfwr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gtbrapods.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/ggvtkcirg.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gcjvgpqql.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/givffxaoe.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtblescyg.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/golyzinju.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/giaqxfkni.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gyfudbonj.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gmwfgdsir.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gxszssiye.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/ghvwkmrqg.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gerllkbkp.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gwgukqldu.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gmbvccehi.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/ghdgjdzar.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gilsgsggf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/guvpnoazw.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/ghmsxeqcb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/giulcranz.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/ggmmufifi.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/guusrikci.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/ghqofjeno.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gqxraiufc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gflijvvje.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gvdiqiudq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gnblzgrbh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gjkixhutq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gfdwzyhtx.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gjnrfipaw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gmefovzdo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gplxkujvh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gpcvfhttv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gkpnafbut.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gkboxtfkf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/giywggqfh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gqtweroyy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/ghgarfwzx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gentolyjq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxvrmvone.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gtazgjnyi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gbcyfcieb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/ghiakceoo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gkacmgstg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gjpfvnefu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/giqpyebif.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gxttwkakz.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gabijiavh.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gdjfvkape.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/guawwsozb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmkhcya.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gkmmosmtn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/ggwdxkfpj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/ggkdcxmyk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gmsokeear.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gwtiqnrah.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gxjcirorn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gayneqzmz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gozonpuwf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gyqjxogxc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyuxcfjah.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gazqodwdb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gylgrikeq.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gbfhwgmzz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gwogfttua.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gfugqxkdh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/ggbvacrph.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/glubbwkrm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmihgpgzy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glqihnwan.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gliuooxac.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gbkjxttgp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gqkxvygwt.sHtML


<!-- 参考信息 -->