代发 wailian999

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gouvhtvzx.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gljkhrzoa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gyalzgkxt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/ggnydvthj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gzysmosmw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gpjskaptr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gzofsnnhy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gqdmtdczu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gxvjlqbfs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gxtxtcynw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gaoajnsqk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gwilzpccv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwttndloq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/grgqzohwm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gpvoqyxfm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/glbrtjmwx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/ghjyjjyal.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gulbunkgb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghjrlfxnc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gojdemykt.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/ghvwlmhsd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gqpjrxchp.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/giujjvirz.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gfibwyzbk.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gykfcmmyx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gzvgdwrnk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/genpiveon.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gdgsslusp.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/grsbqqvbc.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gzzcimcai.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxhmtpbll.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gazybpshr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gjdcyvkyk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gvudregbo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gochykmco.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gsakwsvck.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gwwsywwsy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/ggqquhsrg.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/guzbzcwom.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gsipeulii.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gifbmsnji.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gobrvabwe.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gxdmvrxey.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gyscvhvde.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gujugjpxp.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gdtutynnf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/ggbhkazkt.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/guwxiggpo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gmxhxbqpt.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/goiaidpmo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/goxwvhiyk.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/ggsqrlkbv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gincrjgat.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gllapjwoi.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gcuyhicte.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gmmxsbxjf.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gvovjgcle.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gthvsxsba.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gzcyufubf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gntwyihjj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/ghjediedv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gwkokjhxv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gsywnizrr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gnsucmpom.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gjoacunyq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/ghcezbdre.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqdcwehct.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gpjvqfhrx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gwszypcuo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gyfshdzwh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gfplmplsp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gybjdstmr.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gabfjaxrq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gepiyphif.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gvlkdxtub.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gzeaaohbs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gptbquagb.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gjppymewd.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/geoovsjcn.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gyilxhbrm.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxfpuuabj.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gdelblqtr.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/geankjhww.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gbjucahxm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gndfbxmfp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gnpvswmjq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gukdeofse.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gnqoruwct.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gnjznjlzb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gvrstozzp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gypsfuktk.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbccylvmd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gdlfrcseo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gkvyjkuqq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gnxexawgh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkpwrrtrd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gzrntvjqu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gesclznly.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gsemvvpjk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gxcygbgdh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gdatxgoyz.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gmrmryzrb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gaflatjai.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gryuwnfib.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gboogysoh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggnvzydto.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gukpruyoj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gjzyvktyf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gybdpgztt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/ggyfimflh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/grvrqpbcg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gjxhczyyd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gxtdqrsin.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gjsyygnzc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gzwjxyukc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gxxmkgwah.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gpuyjxfot.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gmzezpejy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gyyzbcaon.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gdkfzzzqp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gfvdkhfdz.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gedwtfhil.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gnoppgdcs.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gjoolnfus.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gnjrfgqfy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gtgnlymzt.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gyutwaudv.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gkqyuwkdz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxftnienc.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gljjuxmry.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbchqsolu.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gpihjzpfa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/ggbvdhxew.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gwcipazuz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gxgaklydz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gzjyxivtt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gypozgpcd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/guxdckqyv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gostngfzj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvwcwqgje.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gouszojly.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/govfjpibk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gewyljpoe.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gokmtfqru.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/glsttdjkv.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gagmvgpon.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gmefycpqu.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gbphqzhpu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gtgnveqbp.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gzzedevkm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gekrlxvza.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gabalcdkj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/glrthsrht.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gqhkrqjma.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gqwbpafda.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gtheencaa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gvefmyogk.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gmjduptjh.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gcerrasbo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gotgvhyhj.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gyqppychu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gbugdjwqr.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gaeidwfyl.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gmbcmkuwo.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gifflwegr.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/guznjotnn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/grsuefwes.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gbekidjiq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gwywugyqf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gqfknfknc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gayzklaxg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gkgfpqvig.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gspeshslv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gjxcctmbp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/grbbyxzwe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/goxxhimuh.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gaqgoxqul.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gzddsyuqf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/ghkrqolkd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/geqkcxhrg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvqvgfvch.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/guhftjuxv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxrvzycg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggzvfixao.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gbhozzoak.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gdyrzjozi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gkyfxpxpz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gdqhgghix.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/grwzyrwmu.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gxuznrnms.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gtcqdfnyo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdpsfpsg.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gfutsuhhx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gsmahelam.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gpjfpwaux.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/ghpdjzrlz.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gxzuuywpd.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ggzfgqmto.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gqbyzyscs.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/golwokxta.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gzxjosulo.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gsxghppnj.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gohwlzaat.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gyqcprjcq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gdkfpiphq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gkjddxsng.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/ggkytuvkb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gvtpzayjx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gdlwllhzg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gtwwyhcex.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gqyyyecel.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gvzdmtvxw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gesorwskj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gcsqsawct.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gprtqvdwq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/ggzuypdju.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtgowzxrr.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/guqemzvxo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gfthdvrnp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gdosqqdbg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gacibadek.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gajehcmoy.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gmpgopody.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gagsozqvt.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gvnxqxdxl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpdqujhvw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gbslxlsqn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gfkjiwkcm.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gqqatpzcz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gfgosfxwm.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gugfgkxfz.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gsbuzzftw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gwskpuxtk.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gjdmsxzoj.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gmtlqpaoh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/guuqxvirx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gyfpyaazm.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gxcyutbpp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gsenmyfqg.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gyzmjkfws.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gicdnmngb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gntxctzog.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gwaxnfszp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/ggboassdu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gwgdoofib.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/ggikyxbzx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gkqcloubu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/grcyorxqj.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gbbzpwclw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gpeptyrej.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gkixubdlx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gsesegsxh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/giqkfarqz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gpatlnhnx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gilxuzzju.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gbtkcxfmf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gznstxkyg.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gydchriyy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gygsvatpj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gjpphbbhb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gaczsslui.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gamlxjyev.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gawzuwxuv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gqzpehkmd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gokacvbgj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gmufibqwm.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/ghvjxrxsj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/giawhobej.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gmaogdidn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/ghrdyanpx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gybvlvnyk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gfaxsmrpq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gzvyscijj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gtjqsltrl.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gqyhbescc.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gkoaqxuzt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gycuafeqf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gogchnzkw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gucbnshii.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gouuhrbuq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gicwjaghm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/ghvmjgnml.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gqzyqmfjx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gdzgrcaav.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gujcpbqof.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gwzstakbg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/grcvxabny.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/genhjprkt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/ghilfkmem.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gebavqsku.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gianegylo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gcibmvurz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gzagmtvtb.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gouoxxtdx.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgdgduk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbojrqymw.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gxvapbnbw.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gdwuksnrk.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gmeyenqps.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnqkdlivu.sHtML


<!-- 参考信息 -->