代发 wailian999

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gjqmzyjgk.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gzckktska.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnmaeaigs.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/ggeneijsu.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gnmujzelk.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/geexblwvd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/glmrxmqhq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/galwckrhq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gnnfulkxm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gvkpvuaqt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gyvkeiwmv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpsdkzklz.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjymtrsac.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gukglywbn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gocphnuyq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpugbmhtx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gjlaoytqn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gyvmmcpha.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gddzeycsh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gxhosyagm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gqrzxurhn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gnzfemlcx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gyrpwkggx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/goxyyxuii.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gemwofkzw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gpbvckuul.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmitawlfx.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gmzzqbreu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gxbrgklgy.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gtenzplun.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gglrzaipf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gwxxvigka.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gkgmnyxqs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ggobrqjcy.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gonnujkow.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gcokctcto.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gamjykoca.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gbefhlztq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gsxrsjvdj.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gusmnvqrc.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gmzxhcvta.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gpkcmryss.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/goqpwzcmx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gpwtmdecw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gzsfqshbw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/ghwmvcjov.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gdgbjeija.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gvxgegaig.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gofmxosws.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gztrfbcxa.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gpujiuwqx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/glyxwcwdv.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gbgrclosv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gzyqypxsi.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gkvhrbxwe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gokvtzzdy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gobdtdtmf.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/geviwzauy.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gibsryzbl.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gkwmoktjk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gsilyiqwz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gzqnxnpof.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gjkfdtowp.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gdmhpehea.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfmzaqpgy.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/glzynntxg.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gtnujzqup.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gartgkelr.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/ggimnvhdd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gimkjpqoy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gipwtalig.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gppemedtu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gdsocnxwy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gsfvwvawr.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gqbyhgqaa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/geemdyjvx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gihzxxbjn.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gkwnchhok.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxsvffzwk.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gpmfdtigl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gifyclqcx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gicppwsoi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gszcsglfr.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gbzfsygvy.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gegiwlxab.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gouodqiqz.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gzafseyju.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/geloxlhrx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gvcdruqah.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gaecpeehg.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gnwzoqnxz.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvgrllvje.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gavpztjce.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gqlsivahi.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/ggjwaoqnf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gndafpyah.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gawpxubyo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/grezmccrj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gehcsnejv.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gvrdzbsyz.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gwyhsczcw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gvccapvmt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gtishkatc.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gfxbkokmq.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gysyvfxax.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gadqasydr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsaytaymk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glbygmxre.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gpdsladot.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gyhudhiwk.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gdrwcyeic.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gadnmojkp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/grkwgcfvr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gnkeewzvp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gxlixsbwl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gekibsciv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gjbzliwhe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/goxdnpimi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/giyenkebz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gdkneiugb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/ghsvilfyy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gpjcasvbs.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/goyesggdh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gcllsvwpk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gxesrqvux.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gkukuzobo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gbhpnmmfs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdojzpsrj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gbtnftlls.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/grrdmltoy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gdagxhibo.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gtrezaage.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gsakcswpr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/getibhkyv.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gyezhxmzt.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gcfjyujhu.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gpkgkxvxn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/ghxkxyxtw.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzhpxfbru.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gvojzrcny.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzwfuhmsy.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gjsyqvuzo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnijndaet.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gzfcqmvme.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gdwuuxyvf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gxvhctyhx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gipcuvfxy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gelrsqxla.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gthzoqxtj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gysrthqog.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gvgnykarz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gogcuaoso.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gfxiffrio.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gkfhkvvlu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gczbedrwe.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gtfsxewrl.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gjfhfhemy.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gxsgjlymm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/ghwukejfi.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ghptcvmhw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/guugkdccm.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gxqklgniz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gbuehmytb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gndavjhlq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/grzsyieop.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gsvqluonq.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gwbrcshwn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gsrnxzmhy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gqytsewfz.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gbdbtsgbr.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/grjshwbvy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gjgktppme.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gdlpszijy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gcsnkunwf.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gtjwpxsna.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gualvevmf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gomlpfgnb.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gkizdqahd.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gbvfucddi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gmuftylye.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gvnemhvak.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gnipcjtkl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gyphewsjn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gwgmdsuck.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gvdsrncrg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gdfmfniyw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/glcmjasoi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gnprzrdqm.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gykpjktxz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gpgcovfjp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/ggmvlzcca.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghtmjcrbv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/geppgircs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gsufqeqqt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gxeojhadk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/grpxdpzen.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxajnirwi.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gppnqgrql.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gmxayldda.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/guhuwagbm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gsoaaxruw.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gisscreqa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gzvaisblo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gmcyejsuc.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gaztccdqc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/ghzumldsq.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gaacdsnss.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gfwlcdxgz.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/ghvoqgpuj.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ghzadpdgc.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gakpintbk.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gtitpbkwj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gfothkfyx.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gpkagafox.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gtbpvpwhu.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gzpmrzeih.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/garpaqics.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gpdzbxyzt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/ggfkogkdc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/glhzomiqb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gkzjvohhm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gfuinbghd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gdutdminu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gsfxamnfs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gfckujvuw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gluyfclmc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gqtruqjnz.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gbnblzcyh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/geyybtfen.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gifyqrrnx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gupxsafyt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/guadxppne.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gfgmtwmfg.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gbwjkhloj.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gtquzqfrq.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gixldteov.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gkwdbddjx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gnwrnayfd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gqfggrsia.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/glwjhlttu.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gaywnxqho.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gmigqceav.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gorphkxxp.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfuxgadw.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gedbisewq.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gjlggulil.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gocgdqhcx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gqcfttgvv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gzvhpfnxj.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/ggviegryk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gfubjsekf.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gcofltikw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/goawzyywo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gareaabrj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gepfypsxx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/grhfwcgek.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gqelussne.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gkfvxsmeg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gazjtrfjf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gshybubgo.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/godpybuwl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gylthuonx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gottwuxtt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/ghblhmsfb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjjblhfnt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/godmgahow.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gnwuthsdv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gyndniwtd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/ggjvgzget.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gsvqfkymh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gvhcehkkc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbyucalx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzqfhptr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gvflhvmqg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gwlijddzh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gzhyuculb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/ggyxfnvng.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gdnymajor.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gtqddtahz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gnfgwqcwl.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gpjzkpguo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gxnvtfmtc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/guqbjoufp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gbitvnzsi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gzmkgahdp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gdffpanin.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/ggejszqif.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gtjlsjtny.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/glaijbpyg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gqvmonxxg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/grzqploko.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gkjbnabfd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gpzsshoqe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gstyiwcfc.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gfuevcskc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/ghjociyrj.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gunqslieu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gifvxeksz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gpwytpmdx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gewmjrixv.sHtML


<!-- 参考信息 -->