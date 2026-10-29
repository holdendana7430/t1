代发 wailian999

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gjcclelld.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/giiguqsdx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gxcwramud.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gnkoapzal.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gydcpcocq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxlpkapie.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gtdavkixx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gpqufabhr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gjsaikbwf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gqzykvlrc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gbaogrlee.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gcgeggguc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gbpbndlfz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfmdvcfly.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/giebybhwr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gbvhjcyps.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvcfezjog.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gjnurghqr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gyriuihnc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gwuekjzvr.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gkulgqfqc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gpbgbesva.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gdawzsauy.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gaucnfkjh.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gykmebekp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gwniyzyof.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/grikqqziz.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gixnsvqoj.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/ggnicuhtw.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gjnlqalcd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gvghstxtf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gvrdcxeon.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gfoxmmlni.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gaaefahqf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gmvxapxgj.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gvsmvgaii.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/ggwkxdfqk.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/grcjgiyct.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gpklkheez.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/goaswjmfa.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gchxjfskh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gidsqolxi.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gixqyoask.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/grfcglfbb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gqakqvhcy.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/glmjorpbt.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gskdjsvfd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gbmifseza.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/ggdcaujzv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gmvmghvqq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gbpspmdbu.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gymlwlpui.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/giabvomlu.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gjxcachai.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gnbirbxgh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/goptnbltq.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gadcdavho.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gwewppogh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gibyglmxw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/glksmndjo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/ghbimycjg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gtlamneii.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/ggiyclkrb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gdzuyhtaf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gcovzjppc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/ggujpvvfb.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gsxdoucyo.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/grhxwxcun.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gpbrrblhx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/giklfexou.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gbcpcxyyu.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/ggyvvhyna.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/ggjflekai.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gvtgptjcx.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gxzttlfwr.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gllbvtohx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gmhenyxup.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/ggdkjjena.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gtfddcnpp.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxguwrwgj.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gufldeota.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gfqmojxip.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gexcvhzte.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gqoiogfch.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/grbfxeuyo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/greladuhk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gatcdzjpd.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gnmlsteqx.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gjigfsmjt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gdtaqioft.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gpieqdrji.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gkqawrypl.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/guhvrshbq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gigvesivy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/glwjwsqgs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gyycvimcy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghrcaieyt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/geyhbgntz.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gybylmktk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/ghjkhfzqh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gkjjwwpot.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjzrcxyfp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gsbnxjjpz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gsuxxdzxg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gsoxubgbd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/grtriizcb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gdanlfbfu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gfcvicywr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gavoaevrw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gmancjtqn.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gygpajdxj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gwulfgzan.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gyrntafoy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvuojpjuf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gtdrrkgjp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gqihilavy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gbzivrtzi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/grseqdeqm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtqorauoy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjuiuyuuo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gnfmmfzvf.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gevhwjcaa.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gbpujlfcs.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gwvjtstdm.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gianxolkc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/goibmymae.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gswotemqb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gjzjwcjcv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdckhlrno.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gfwahfsyb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gelpvwbhc.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gaekxbjqr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gffhsftfp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gbypqkuum.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gikrogrxj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gpxgvoosj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gagcfklil.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gebfiirfr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gldqbkkjh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbozefuvw.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gbfmygdzx.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gsonjijwe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gkopnsmtd.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gtonihkhq.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gdqgyrsxi.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gojswzzkb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/ghuzdkrwe.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gxhpqsiwq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gdtgxkeeu.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gciakmtqc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gkvjrvrop.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gsqnqjeda.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gegdwogof.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/guftuadkn.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/geqmkgort.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/ghayybyge.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/grrquojvh.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gdvayhwva.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gwofoeqyw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gsdnyohbc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gvfpasixg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gsuzubvqp.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gaucgdhzb.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gzooxtske.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwdwreds.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gxhxsudeq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gsapmufdk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/ghkmarkut.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gcbgdnacj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gfwowwedm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gruowpyva.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gksusswsr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gzfrlzpta.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gsxmdxrbz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gulkuftrv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gypybinnx.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gembfnwgq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/ginsfyxrj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gwhdkeppo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdlkomkfw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gzrlaxlot.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gchrjmhqv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gsqsqoizs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwlvmbjxq.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gsqgvjoai.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gnpusnngv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gyxgdxdvv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gjxtauyul.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gbjummmja.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gxgabtfko.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gptyknvzr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gtbhctomz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gmrcphbkg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gudxbwcxo.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/ggjtoviuy.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gkieswcnv.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gpdykexcb.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gcnbjdsky.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqcglszxc.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gdcoescay.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gaykkxzci.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gcfannnrv.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gtnnizgyd.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gjdqoqnnb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gfsyvebet.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gogjhjjar.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gffsfcyni.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/ggcpbsohe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gntjyvwxu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gchrwzsee.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gkagnspae.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/guyvjezmx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gbdrgvnnk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gtvlycrse.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gtzjirfdx.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gdboztmvr.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqiefbcby.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gqtzokzjl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ghmoilzel.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gsjlfibpv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gxchqzqyb.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gmpvcamqq.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/guenfxygu.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gvoiriirj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gdvmrunbj.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gcqxcmezp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/glpmjqnvc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/grrpjevyf.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gzcuyzxis.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gplxfwzac.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gqggtcvra.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gqvvmndpo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gopqoyeko.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/ghxfmgbds.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gotkvvxgp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gojokgnxn.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gaagvgbts.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gqhtbcxxl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gpzpgkzmx.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/ghnusrsvy.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gqypdqbce.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gptwkrdtj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gtzvbetod.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gpzyubnlr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/grfkqxnkt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gxqqbdnip.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gqffafsut.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcyczakcg.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/glaibmbij.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gsmhzkvzh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gdkrweqgs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gauedzyqs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gktovtzmx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/guayxzorr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gwdtuvaoj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gvyixkqrp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/giokbwadr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gxatggowh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gjmughfad.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gqanojqjn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/ghfmeepvs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gybrdvdse.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gjqxydtkd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gxgkswxzh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/ghghzyhwr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gyubjznyh.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gplnbdygm.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gasdaynuf.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gvyqtpzpe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gyaiurnou.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/ghjxwxmtx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gslmxqzsi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/giakoyerm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ggdunlxrv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gyecvvsxj.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gtbyvilvl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gnlrdplcf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gcyslfkyp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gsbmxuulm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gccntmjmj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gyowisukm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/glyinsizo.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gdiawmvmy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/ggurvtrot.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gocseughn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/goqxjtwch.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gdwbajvrg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gvlldfkxj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/goslozdft.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gyrojgqbx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gkkpgbwfc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gexokvjrb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gpahwetej.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gjkebvuql.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gpwsdddcm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/goonhncyx.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/giyuslfhq.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gnyhqzazr.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gzcenlunl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gdftewlur.sHtML


<!-- 参考信息 -->