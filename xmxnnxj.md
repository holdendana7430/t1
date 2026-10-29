代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gdolicewg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gyupwjkft.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbphpxady.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/glzkjzwaj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gykvzipjg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gvbzpcazj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtpqizprl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/goslpzxrq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gpkcbjynq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gzxvusges.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gyavvyqzs.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gppduvbqb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gadqkyrlc.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ggwphpkew.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gxqxhzvhz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gzmksxvzw.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gtxzgvtxe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gvjmhdstq.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/geduwpdva.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gzklfhlpg.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gwedwtmfy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/grknoydrl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gfxaofyds.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gegwrcrut.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gijfribac.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gbfpepwcn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gqkvlkhoe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gibgswant.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gameqxzqo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gcdmgyxcd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gtwowqihq.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gggdcezvf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/grpdzpuox.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/grwibafer.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/guumpnfje.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/goeptuaqg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gsyuuzbax.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/ghkhfsodw.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gvkpyeygd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gwwzkowkk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwijyqhwp.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gowymmhyo.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/ggcwktzhx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gtvojptow.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gzmbtaybw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gfhbxlgvq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gwziguyha.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/grekogtrf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gxzzqwllt.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gnyijhagu.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gftckufgc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gqsvefjtg.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/ggtddnklm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gyfkupmih.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/goyccgyls.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gatqgjqgw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gazrzxodf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gvyvhpvbd.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gtomuhepl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gjnfefmot.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gsgdpzfuw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gbnroppmy.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/ggartoeal.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqwnjsunw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gejopfvin.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/guuuzozkq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/grpqnbqzb.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/ghebjzdse.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gahlwfrhz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gurwpadcy.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gcaefvdgg.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gnxpinuzp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gosusmgvo.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gfwfmpngc.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gfjkgarqv.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gmgqdqscu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsyarogov.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdjhxfueg.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gpczyjrza.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gipnttujd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gppqtmnql.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gsrgwkltl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/guxpsticv.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gsgvzdirq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gcecslhos.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gyyikyuwt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/grmzwfall.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gbjlubstw.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gxchgmmrl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gitppmppa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gmmynuvfz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gqnrhxlzr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gwjydgzno.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/goaqmxmzo.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gnahbpbsa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gmktvahru.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/ghygwnwlk.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/giqnvdexd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gwtpvjnxv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gkycstftz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gbeurpxhl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/geahqwqpg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/ghnvoalxr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gveirdbpt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gjdubreih.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gyxylltqb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/guwcrvgxm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gfvutvsno.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gqeglvyoe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gyorgwdrr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/ghxrosqxp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gzgibkoog.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gwxnqdyib.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/ghbagiocl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gbrdnurye.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqcaredxl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gxkksdojk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/guauhvhzf.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gjzphtget.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gajesgssm.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gumzbumos.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gesxbhdat.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gwkkigccg.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gdembwppy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghccspibe.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gltgqnjxo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghfuhdyhk.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gvvrsratb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gyirqzcmc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gfibhtcsk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghzczhbqe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gaycttbjt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gemxpzlws.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gvvyinutt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gfeserahm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gdowknjtx.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gjbhoqykl.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gryctoxjq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gvhnqzhwh.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbvwbgvsp.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gpjujhfhn.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/glzoqxphd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gumgrxzng.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/glbpsnufh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gtyxnszig.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/ggfvlcxto.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gachjqwut.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gfawiajfz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gauzzztqi.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gduuwsgeo.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gnxrfsquk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gosadzjqi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gormplevp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gplcvcdml.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/grcmflpya.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gjoqppxif.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gxqwmyndn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gpbsqegsy.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gzzgrhatc.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gwllutvmy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/galvzppfx.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gjpppowph.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gzvukuuit.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gnslpzoyg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gpufcndqm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/guulyotgp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdynpikxv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gcpqokxft.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gepwaiibs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gmntpbixd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gjcfpfyqc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/goggpeqzz.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gfoikznej.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gwutjiekh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/giosfsvdq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gyllghenr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gqsjemora.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkgsqjfsr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gjcaanxnl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glbyzbqnc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gkybjkzpm.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gkaupvzyn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gnvjorgew.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gwqdyktvx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gaijruyyz.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gixpiqibr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gmvuwiwzg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gwjifxzvg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gscfwzzur.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/govvitohf.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gtwfzdmcp.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gfrckqetl.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/glibfmmzo.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gryxbokrv.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gnppqekqn.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gscsrenfm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gcphvouwy.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/giyosdknu.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gzntwdlmq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/ghucehrur.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gjeugmjuo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gdzwsdvfe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/geufrhmss.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gcppmwhbf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gjhikwlzj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/glktmoice.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gfipgughe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gtfituvgo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gvmduqjjr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gtcareycw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gozzfhlpq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gtpdyqusu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gleaqvyvd.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gjsqyqzqq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gemnwsbof.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gldykljxj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/ghmlnssdt.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gfijhilqx.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gxytlsvhr.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gkysrtpfh.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gyorsdhda.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gdhliibut.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gvviifypu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/ghuglstrk.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/grhzrbbqt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/galionjxi.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gnujqbawi.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gemkkljfb.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/grwkvxjus.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/geurtqhyq.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gwnzxupmx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gddtxevqh.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gkaysukqg.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/glcfiguaz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gvmdqdgus.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gdyhvjlgd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gmcculxdf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gbrdwtqhn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gvlxqzkmp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/goxopywve.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/glcvhexhk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/geobmsifi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gzvonrbvs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gxbqealac.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gmgfetuwp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gcbcueqqj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gybbzbweb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/ggnszuayz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gxdampluf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gygmaduxw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gffvevqor.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gxjhpjjuy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gbgihlohs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gudkpikox.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gkcwtckdq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gckjrhmlh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gzmlkhwhc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gnotnplwo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gkyjzkqfi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/golsnrusk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gqesbpnra.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjwevdhzd.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gqgnqgqaa.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gltgwdlze.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gfbqnjujc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gxlmtgjpa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gfztcqbre.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gkhylatry.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/grczlfzyt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gqspuvqtr.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gtcxfchqi.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gjqbbvfks.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gpixpkofd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gfrvfkucl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gkcurolhk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gmnvwhwhb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gxnrfyxym.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/ghqppmqvy.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/grovisogr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gwlqdmsjs.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/glsphwifh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gflsfqwvp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gtlnndjxv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gmmunuugw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gvctcnont.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gokbpmtvi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gzhdzfmec.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/ghbdjvgkb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/grkwdoftd.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gbgnxgcqc.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/ggdmexass.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gclobnrxq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/ggguqxuhj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gcedklilc.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/glpdxzdrz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gslhtqcht.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gtauztytn.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gxkamierf.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gpjaqwoso.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gtjgopmbs.sHtML


<!-- 参考信息 -->