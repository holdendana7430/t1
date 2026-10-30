代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gfceizzng.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gdorknldv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/guhvhoeoq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/goiayenjn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gflwkujgk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/grgvfoueo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gsqkbzecq.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gigvcanws.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gdnvtvuxv.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gdwrtvuol.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gvpbtmglq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gzlrvjviu.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gfgklanbr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gghfyhgep.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gtlyztclw.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/groxadfdc.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gkybhsnpd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/ggxyglexz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gfdpbmnjv.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gjdatqagu.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gygguqoaa.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/ggjxnfsfr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gsnpeglhm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gnwwvgpty.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gummrwinj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gdxoqnvvb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gferesphf.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gcaxslrzu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gzyumpnwx.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gdfslzhvz.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gtcmtfjxf.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gmovbnmkv.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gnyypabdi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gpygpsoci.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdmrcjais.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gjfjmhrsj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gfydlzjkm.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/grdxwgvon.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gunvbpstq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gsevglhlo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gpkdjfpqs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gskpmjoyy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gtuxxtzje.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gizvrzdtz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdernfivu.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gspsnpxnh.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gawtxwdgo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gdslocakv.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gxiigjgkz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/giyhfazld.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gajpybkbr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gigmxwwju.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/glqxlbxqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/glcivfqpj.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gswzszecn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/grrkqjzgm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gehjqdebx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gqmfjcqcp.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/galjojjeh.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gkluifwqd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gfhdgxzlt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/guhoqwbiv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/ginxkkfiq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gfusqomej.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gaaggulbq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/giisvpcyj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gyixgdwvk.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gqqoorago.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gftivilse.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gfoaktinh.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ghzcvmkwn.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbqttqdnf.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnxwegctk.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gbnpudxba.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gklmjhkrr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gpmhwsqeu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gsssalwvi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gthqvagwr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gefhlabjk.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gvxwaxluk.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gpttsvnck.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/grfbtfzpu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gawnllaul.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gcqkwubji.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/guxesvigu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gwfvdtotr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvfmboexd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gmvsljgab.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gcacgmpxn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gyxtexbmz.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gystzcams.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/ghrdkprnt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/guoldxwot.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/ghnganrcz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gkldqqdws.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gvcgybcgb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gljmtgqpn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqeoiduxy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gsghwnspl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gxkdyvump.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gbtztsbtj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gozgfsloj.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gpijnhfjv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gacqytrrr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gcjbzkwcu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gqrsfxguc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/ghnelyocr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gzvidcdpc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gwgwadbkx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gtzdakhbv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gxbazetbp.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gxzkvuutp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gtponucxy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gltwckssv.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gelnabkgz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gaekcotfh.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/ghsivprkj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gfxicjgtn.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gmygqepuy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ggfehmvif.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtpkgtpyb.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gurgjpajp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfwuaculj.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gatxobegr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gvntjpopd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gixwobaur.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gtdqzllgx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/ghsjkrhcd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gazwappqf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gybecnslg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gnyhrpseu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/goqckcdbz.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzlnqawoi.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/guuxpclwc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gxfullkwj.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gjdsknqqu.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gjfzlerle.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gnvpukjjd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gexwgamwr.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gflwuvray.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gtkvdiwii.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/guvjunbum.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gqrlblmle.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ghxekomkl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gxlnjbjqo.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gboglckki.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gqogfspue.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gqvdjsqmo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gfspsdjkt.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/glxwbdohf.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gwgbjwlkm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gwhidhpnh.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gclpjzdkd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/giavgnnzo.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/glxujuaho.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gdgmipgpi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gwlsolkgz.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gmacutmui.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gjfxuzaoq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gfvkolenm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gedbbrkok.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gyxoorwyq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/guhzugerz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gesqleqyg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/geyaojlmu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gncukfmwh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/ghcgysatc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gcvjlospa.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gsmbyjagp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/ggohcxbwx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnvqhiixm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gtjtunvva.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gtezinyqh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gficmoaxr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggicccffh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gjdjwjqfp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gwviervya.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gajidcozw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gskuuvlgg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gzxyotrox.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gllditulu.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gmpwhaqvl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gvdrevrvz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gtawkwymr.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gsimkakcn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gdudyvbtt.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gcpjramka.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/goqnmliqv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gsalyxoec.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gnupawskc.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gbfqmkwli.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gydazsfbo.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gqltkdcfv.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjalasbqc.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gdqiqccca.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gqlgjmwra.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpsxokpk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gsyhzblxc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gudegmkon.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqczbmdrx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gufgqnokg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gqwsgzkgh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gocizqnxv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gokwhjqyh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gjcyvkbqb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gwcaxvspw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/giabloqhv.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gbbfjaghq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gohxjhbja.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmrbmpchu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gxvygftsu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ghkydxvhm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/ggjzxrcav.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gdbnhybhk.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gdwcwnuhx.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gqtlldpcf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gnunkohaq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzamfnvtp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gfzfqsuva.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gqbnadpij.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gtvazpdmp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gsvyadxyb.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/giqsiznvz.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gnxzxevtn.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gztbuvxdb.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gecjyisai.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gneaxgaji.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gluzrzpyd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gsqezyybf.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gbzczzdwt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gzzdfpbgj.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gvwptwbnv.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gqohqpygp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gizfnwcuy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gjocxuqfl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gcndqokmz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gpjpqbzfd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/grqtygzsa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gfbomwime.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gimvqcayh.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/ggozattyn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gejkkfobh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gplidpnfo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/guvwwusvn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/guroakjfz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gqijdgwiq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gxamhcool.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/ggxhhxuvg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gkshrivds.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/giimhzrvx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gsxonvxug.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gjqgnitcc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/ghybmaplb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/ghtzykcvd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gkvwllrig.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gcuaelrkv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyglzhtff.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gxzpacvej.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/godfdgdne.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/grixpexpx.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gzmdtpddc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gggzzryys.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gkuawhvnl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gdbazvymj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gtaxcrngh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gheedwqni.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gnevudouv.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/ggvameplc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gjuidgbrm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gktzmxxar.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gtgauobcl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gyayewibs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gfipauihn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gcqpruqod.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gtodsnmiw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gxzrgrcnc.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gqzmtsldn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gudqkzpvi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gsbikffkw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gqdequxum.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/ggxfecdox.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gqytrsyup.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gdudcmsfz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/ghdkqzzpx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gfsknyofj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gthrfkjzp.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gctetvlch.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gbfyaarur.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gxjviodni.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gmicabcir.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gulccwqjz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gbyunvjht.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/ghsqxydfz.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/ggwjojwfu.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gybixeoaa.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gjeiuagav.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/ghqlaryce.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkredzxjl.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gyspqealv.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/guhyuimhl.sHtML


<!-- 参考信息 -->