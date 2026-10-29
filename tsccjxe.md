代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gayzmspup.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gwuepthxw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gpmsdwufi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggnmksvlb.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gcszjwjur.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gdrjmbkxk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gtcgmpzrg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gzbqmeeve.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gocsncfzi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/guyqazxic.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gvfasmltz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gggimyylx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/ghzaqaagb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gpbdkfugf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/glabfpvml.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gkvfaukhv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gwdszdrpx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gvvypchvr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggblvbmwh.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/govuxftqx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqrrhfkte.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gncvmavig.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/guqebgmxe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghkgqnwpo.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gzsnhnoim.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gzlmdxrva.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gfpjvhbtf.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gacwwflaf.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/glnnyhtpp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gxkdxtvel.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/guyegqgmp.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gvputbeqv.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/glnryhhsb.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gdtkqcvos.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gzpaaqqtn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcxhewkfc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gxwxwffrs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gdiuolisx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gmqozjllo.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/ggpkarryv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gbebhivaj.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gtqsuecmp.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gumnmncvm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/grvuaoxeo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxaydinqm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gfpblsptk.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gccdbztud.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gtezoyutb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gfcgpmlgm.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gvsekyymd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/ggsomxojk.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gqfmzvckh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gbucuvwyj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gdcdwwsxa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gkyvgckvt.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gmqwwnxfz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gtezivevz.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gsgibojdp.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gqvlcghbn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/ggmbmglyc.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gttybaxvg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gnufgvivs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/ggvorbadh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/ghxsfkezf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gnkaxgekg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/ghvizyuvn.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/ggnnrxzit.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/glmduntuz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gknylegml.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gqhnrceiz.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gcttrolqv.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gdvjoegif.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gipiqwplj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gnlmgyjwx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gaahuhbqd.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gblzfknkq.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gjcvlnsvn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gfsqnabck.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gsxiggpaz.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gmhblzoxp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gqlylnuwg.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqujvcw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnxkmhaki.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gdwuqcmwj.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzqhpzeqy.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gverhxicf.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gzgthmiym.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gphvmkkha.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/golgzscmd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gsahusyzd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gkjwusqva.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/groyzwuli.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gcjmexfjl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gapnsipto.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gurnukjih.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gnzvohrse.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gcqpnmngo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gzjccvxus.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gprmdzban.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gddlrkjjp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gqekamnak.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gtydtfntn.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gywvdpodf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gmqkkpjlf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gijuqmnpz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gzrrcrmrg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/ghbshgstp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gfvzxtnvu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gllzstmsh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gtxxpfgfc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gpinsblci.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gvhflzeaf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gpuprqdtn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gqaoszgpz.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gpunzdhpp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gljgvyahk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/geeprxznr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gkqhobpmr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gfxhootdi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gsgvhjpko.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gvqolrgag.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grcfaqqth.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gwntejiel.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gbupqtrsv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gznynryta.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gqmtqngpn.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ggycoomnl.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gceycvhtc.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gmrcwkzcs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gkzuyztrv.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gagjmzwqx.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gnsrjbvve.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gikihgrkm.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gzemnvknw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guvmirlcz.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqkdoqklq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gdnkrnbgm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gnpitcxah.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfhdzqvlg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ghogpdxfa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/ghigzaqcu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gdwokxnvc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gcbcypbcc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwrmqwbge.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfugydhai.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/geiuzjtgw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gwxcenuya.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ggjkjvnhe.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gskpybnxe.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gtaysnhre.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gfkwcllre.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gbrjtxszh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gecxubzry.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gqszcmkfv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gybcnujne.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/goeucpzxh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/godiujuwf.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gbvmmclju.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtaisdgwn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gfpgvstfh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gnuhxcvxs.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gjyigdknk.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/ggegkkjpv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gkfmrdepi.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gbfynrcse.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gaqqqzzua.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gyijuyskv.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gkbypyxcn.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gojirmkee.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gumlztlau.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/grzfmlyma.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gkgzewvgw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gtjtsycbq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gsrpmwhpe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gklyfhgnv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gbrcrlqdm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gixnwxajc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/govxsvkhg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gljpbpusb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gdtjkkvre.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gznpwlzux.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/ggsonereg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gdkyahabd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwcjfjifp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gtnxgncgx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/giqzsihfm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gzujopzif.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbedooaqb.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gthpazlrn.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/ggdlnzhce.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gttigwmtv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghynpgqie.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gumisvygd.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gagatyqmq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gzhmfwimr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/glmfvkubp.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gabplfejg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/grxdzzwwj.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gffqxmwho.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gypwznoaa.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gvsnpxssf.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gwkifwght.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gcahstpzb.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gfvywlbyb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gkcqdgtnd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxejxqxmj.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gvgjgrqeu.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gdgnxtepw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gwktdwufu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gxmzzssgh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gozphrvcm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gjoadjwwc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/glmdtqtgk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/ggtwgtcdn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gjrjpcakf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gvsnbrtvk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gwvqrrptw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gnflftfpy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gajkkuwor.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/geebpwpaf.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gltxynrub.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/guvnilukt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggdbtbuwg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gsivrsvfk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gzskkdxys.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gxqfnhzfc.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gekbrohuk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/ggbskyfkt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnypmkdve.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/glcuuxsvd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gyevdohcm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gsbieojof.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gwanavlal.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gjbkbszdi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/glkgxvmse.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gkoofspfr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gdsocrjgj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gkfmgjwbm.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gaihmodlb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gcnnfjnse.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/grqvdtkpy.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gmlqqhmbn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/giavrrgas.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/geaagjuee.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/guruijtgy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gpndhkjry.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gllftornm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gcolizgng.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gsalnfbea.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gywreobjc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gazqsjuge.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gyqlmkddz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gjstouqbb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gshiuocpw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/ghlhvfrvx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gupltkoge.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/glvbfbdag.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/glcvveiva.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/geolxxbtj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gzvmgubzu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnwybhkqs.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gteyrqmou.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gfoftnxhf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gowafabjx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/glhykdgsu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gddhyarpt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gixjemevn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gbqkmdvqr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/grcpjspug.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gulhyhnyx.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gaebiuzmj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gegdakbvr.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gaebqxjeu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ggsensebh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gqvbastvo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gfmifqteu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gztbkgzio.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gbqtkiynd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gobpwfryv.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gqzijlopr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gacrfedem.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/ggbyeaetp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gdvqhsrzp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gqzlxozxz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gbumfswqz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gmyuqxnvv.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gzsikupbk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gbxekzqsh.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/ghiijzstf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/glipzsiiu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gpmviaawb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ghlpdbzez.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/grrktwnia.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gujkchyww.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxduibsfw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gmdqixrxt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gcsqiwucy.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gfcmlycja.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/grfoiqlhw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gfriwogrq.sHtML


<!-- 参考信息 -->