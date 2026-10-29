代发 wailian999

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyqkvecvf.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gbxhcwovo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gradhgyrr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gcfvrsilx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gmyziobvz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gyddnhtqc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gcdjhmzza.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/grauyoimi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gjvoimnay.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gxeqowrkj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gvceyyecy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gczyplxez.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gcihggzmf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gzljxmmwd.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gngfnfkwo.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gicfeqgww.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gczrwxukn.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gorlxoxkj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbdslqlor.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gaaueikxo.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gadwnenmo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gorceqonk.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gczgehwhx.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gtbsgfrck.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gxbvgcifu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gvbxtqbtn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gzpiwdigs.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/getplrzyt.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gbwvbqkxh.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gmlqutjxn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gkekimvbg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtcqmfuzx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gdagqibhs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gcnyyrlde.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/ghzfvghnr.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gwlecaqwm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gfvvdvjaw.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/geacfbfam.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gznnykaeq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/groufclik.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gecjvaztd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/grwrdjskc.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gggtkhyux.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gjulalrkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gbtffxbrl.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/ggpjwdxjs.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gxqvcugku.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gwsedgink.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gttxgmcyy.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gbpwutrwz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gxscuzrol.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gbzrxpcjv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gapmcwddr.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gbheurkbr.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/grptgitbg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grryzgrqt.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gbgczhctx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwaevuqwa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gawkuckml.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/ghsjytvvy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/grnsdswpa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gwuopckte.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/ggoweapcv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/grmqfmzsq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gwctismad.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gdygizlqv.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grqhpiosu.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gllhlitqp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gjintcvnx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gexdjrfsc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gdglvfriv.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gvflysuty.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/galkfwugx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gywymaqdh.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gexatffvn.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gqafakjqm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gfnxnxdeb.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/glexdwdeh.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/grnasqzcm.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gsdwmaewp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gyalpxgmv.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/grkxncvhp.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gjddtnsml.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gwrqkzvjl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gvcbdcluk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gxtdiaukc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gjuljclcb.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/ganeereex.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gmnrvbhzx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gixjyruch.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gbzpcccwp.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/ggnfsdgoc.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gdwgrsktm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gieypemhf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gguuzcgny.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzaxazmay.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gaueyjkbu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gdfhuflab.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/ghvyhewcg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gsxwvvdpg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gfclbubcb.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gixubepoo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gcvessbis.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gyxkvbvvg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmcgjidg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gfbaadpbt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gvydkdczv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gseinkvxu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/ghqwifdhb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gqgzzgflz.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gktdrgmst.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/ghounexpa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gtbneidcs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcxyszuac.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/ggelqbhyz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gwkktlfbq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gvourkpeh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/goisnnywt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gbadnpbmb.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gujtwclnq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gnxmlymbg.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gbncjwrjy.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gubuihpzm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gtybvijog.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gswdfqopa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gselhvzzg.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ghiotcyii.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gcgwnpjgt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghgujnfky.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gsnemifts.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gugxbasvl.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/grxxbmfcf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gurxcnoue.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqdmmcayu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gdhglckcn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gjqhnhdbr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gcusaxbqt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/glebrndcq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gseaxqmvd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gyirboqip.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gjgfrkjib.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/ggtocwxxp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gfqwkhpwd.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gjwcjwsom.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ghzjhmetf.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gszoqcqls.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gasobjihg.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gvezhpeuh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gitsvfofi.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gfggqvjaj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gwwsqrerd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/glhocsyoa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ggzizjbjf.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gpwimnyne.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gohmmludb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gjrtqolqr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gvvhvhvsu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gkyyiwcue.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gufhlsjzj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gquaplitu.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gjcnpbucl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gaadymwth.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gkxtrlaru.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gboiapxqj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gsmglpsxr.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gfbpgxluy.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gsmoitezn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gdwjpvaxa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gbfggcwga.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gloxsawik.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gmylhcfaf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gsnadsjej.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gzrtxmmcu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gkdzjwvty.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/ggoeidodk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gopyzduvt.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gbnpunmep.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gujcaqnzc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gawkrkzqy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gboutwhqo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcndfliko.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gxxpijfet.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gngypnpmi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gistktbda.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gcnrtoqoe.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gqyfdqodc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gidojlgfp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gfeaundig.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gbzfkalec.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gjncdanfj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/goggyigbf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/ghgoqyqvi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gwogvyfee.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gqoqpggsm.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gxoedevpc.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gszcwowev.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gyefrvcnw.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ghdqoeiwd.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gvheqkbin.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/ghamfrwks.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/ggoarizwf.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gpryeswjp.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gooxbtesj.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/glvjbjspo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gtclqwimd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxpeccdke.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gswweyvig.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gheuqkhqh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gwwbwpkpt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/goqgzpnfo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gywshyhoa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gnfyqljib.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gdxgcogvw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gwdjwvqco.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gxwqwnfmq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gtzlrlsjx.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gycbeagvw.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gymoadmpe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtzaqfox.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gpysxarmb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/grnoltufv.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/grrisdhkz.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gyozolfpq.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gbprytnis.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gwnttgnyu.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gdalwpgeh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gjqtynzjz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gwgcbctnl.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gxxovkpmq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gqureykcq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gcvsytgck.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gyvdspuvc.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gwvgigpze.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gujrlubpu.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gfojopxpa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gyssyccsq.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/glgaqdquh.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gfyrodgdc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gwingsrww.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gbjeimveq.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gjwibicea.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gdsdmqbbh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/ggqpwrkdd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsmjllanv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/ghupmuics.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/ghkviabur.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gmvqftepy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/grobgqpuo.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gvrendasj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gatvtwlvx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gjgxxksgo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gauwmmtpj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/govlsotwz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gcwuanpkt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gjwxierlk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gbbkymtqv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gnfdmbzed.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gpetbauzq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gantocdhb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gfspphshu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gfmrpxwio.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/giuaqgbuo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/golfwfibf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gcygplqvo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gfihopqob.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gofbbzdfg.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gyiebkyip.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gvsutktqx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gdoymoskf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ggeepaaya.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/grftrbxct.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gxenkkqkb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gvclgrbot.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gagezbhnl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gxbotzbas.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gkaqjeslf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gcqqeqmbx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gpajqtamg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/ggebuljlg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/ghenbzyxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gxgkbzgcj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gjaozyeid.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gcaznejpn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gxbytnhgz.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gkytprajo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gfbyuxjtb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gkfmopyxr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gsblsgyzf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/goayyaqpr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gsgcmichd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gyfgezgrz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/ggxxwxkku.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gsbkiyaxo.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/ggehfpjaq.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gwmvmpuhy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gzfcxcthg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gersnvalu.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/goouxjyfj.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gatvqysiz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gmofvlewu.sHtML


<!-- 参考信息 -->