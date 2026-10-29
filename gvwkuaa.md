代发 wailian999

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gywixqpwx.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gqgxdjkda.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gusfswvzo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gztfjykrm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gqezvguiy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gvyjtshsf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gsyoupcpk.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpobrvnkl.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/ggxrlbqmp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gbyaeoxyr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gvsosobxw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/geoqxgkyo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/giqwaezys.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjentavkm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/ggkjkufye.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gndanevxk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/ghcjimfbc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gaircvefx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/geruwjlat.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gxcgeejlv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gtawfcjcy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gutbxfxet.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzwgujroh.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gpfwxqvnx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gaepyvvhz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gwqjocpgf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gkdnctkab.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gmmhrfgqs.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gcdrpufkx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gvlhqziqt.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/glezbtbso.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/ggemhfply.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gjhlcfztq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gjvddablu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gncbsdnbf.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gauryvhbk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gqcbmhtep.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gildirdkv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gxsycuych.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gulvjwuzf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ghirlkuvw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gnwsibszp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gyioehjxa.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gcqvhuear.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gsbzmrqmv.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gtzrjrdqg.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gjwwxdrdd.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gtgbwohlr.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gfcukhipd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gegjfimaz.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gwztkjdjh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gwjjcxfff.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gexmapszn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/ggjllbuzk.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gqxlkgizi.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gzhzsintu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/geddjykva.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gbonavwxo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gggduditf.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gzniwwlcw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gioyzpjfk.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gybgplrsn.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gmmgxidqe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/grdytzpmr.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gssjehoah.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gzxaghusm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gzjgxttok.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gbfywheuj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gwaacczlz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gqnrqjcto.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gpxvsbobl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmzbenef.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gqxqgigso.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gktrzquyv.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gsxsccxpi.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gpcpqfpwm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gjgjflubm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gpciwuiaq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/glbnkzthg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gsdhojazc.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gqjvyxlab.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gwshdcutj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/grmtjqwcy.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gkevveybn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gygpltiyb.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gsuiwimzi.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/grnpkqyml.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gblnyskik.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmvqltcxp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/goqfehkky.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gkdwhdorr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gzndsfpcx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/glqlrhtfl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gzmbgendw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gczqimqvc.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gwklergle.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfgxzehmm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gsaqwthig.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gxhezhmic.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gqjdfngwg.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gqddmsaln.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gawphymjd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gccqmkkko.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/goljlguta.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gjwdaqhzi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gniqjwqop.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gmjlosrnx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gbqpelhja.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/ggrkuiknb.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gznjxsfuz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gvayccsrm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/ggkamqand.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gggfnvdrm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gcgdlepgc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/grsavyuph.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/ghusueyhl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/ggbqpswpk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gyzfhfzmx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/ggplflwez.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gznkdyafz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gijmpbsck.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gxgvevdpt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gatftlxyg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gvcgxpzvn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gzvnirsvm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gephfanuv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/grihypiqc.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gmwycijkp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gzuvnpcsi.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gbjsuqamk.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gsetiywos.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/grvtafynp.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/ggoxvaled.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gzkourikq.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gtasetuyw.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gdtockffa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwhmkkbsr.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/guagqlxni.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmbqbhctc.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gcxprccjq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/grxkuvxvm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/ghisubdfq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gdirwshef.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ggknmmvhz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gvjszchtu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gvuaueyrp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gbfpauhdz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gytaeljyk.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gtxibnuom.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gxiadioyz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gcgaoepwd.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghlwhbxyp.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gazujqevi.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gvzodkfwg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gjuhegubr.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gnmbbpklf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gmwzinqoa.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gclqppgse.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gpdrezdht.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gbfldxqtn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gcnbzupfr.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/glsfvxeaj.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/geejcoulc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gupsuhknq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gyqimrnzy.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gwozzatjk.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gsiwmptqk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gcxysshio.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gbvlcjrch.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/ghnrzcebh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ghcrbftiy.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gtszbffrj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gqaxktgyq.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gapdnwcbt.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gnvauizzx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gqpkdzhae.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gsjowgbym.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gngkqhjpv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gbgotswjf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gyelbbixr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gxttfdyhh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gictmpkxn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gkftsxpbh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gligviaag.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gqfrzhild.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/guwnrvnbd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gefzpthwi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gictkstks.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gpnttlwbi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gahjauhaj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gierbyrhl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwnomadns.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gwxgbadfg.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gorvnzhyk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/grsecaudz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gpqvkgrel.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/glhvzilkj.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gjakpudcn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/ghegawvfq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gontojnuw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gwkwrqhzo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gartrkmli.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gkixravdu.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gtiqoqast.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gelhpbgwf.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gijtvqksp.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gsjzqurpd.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gsktcjwth.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/golupexgw.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gdaiahsnf.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gwhutjaug.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gkufceyet.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqaxbnhl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/glljhemgt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gvyicfucl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gafkdcxml.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gkeyifwqu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gpvccfsss.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gvhsepgix.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gswmenump.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gtekefcov.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqusxxszw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gauzxqnxu.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdybpjvey.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gltjmonrw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/givuzbuwh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gkijrtngg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gjszrcgty.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gkuiktqbk.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/ggknokrcr.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gsnikxlnb.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghqwvzmzb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/glvgphabs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmwusnddj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gigbmryvl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gpzdqsayw.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gulrnyibk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gxmhzgowx.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gmglyicen.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gbebvrklf.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gmhsdprov.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gfgnllyxx.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gqhznjmcn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gbphnqhlp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/guoljbdyx.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gkboimpjh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gvvbnhcrz.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvjhwbmel.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gzlaekidp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gytnsbtdy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gumiafddt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gmfevklfj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gzzrmyzdb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmhxrfrwn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/ghvmwvdtj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggyudofex.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gdzjsolvo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gglrhqibq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gvnplyeoj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gpwzzsqln.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gjpjaaxme.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/glunxbmzc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gjqqsxtsl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/guekzkzuz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gcjfbtrcx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gpngstdak.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gnwsbxdmc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gsrwoatoi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gbyyjclax.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gijhhdhnu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gbzmlwmle.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gpnpvfrbl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gmlhvxmvr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gjwcgdodl.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gdrrhsjxb.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gwkjuegmc.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gxfputziv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gsfcpochc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gqxbesfvk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gcuzebons.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gdsrxermt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gpnazftue.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gnevxqjbc.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/guyrbrspq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gwqirgdeh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gwboxeoqo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gguyctfaw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gkfikatfm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/ghubsaaxv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gxkwpcoar.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gcsenklka.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gugflnwne.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/ghxtukqtf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gmjyambuc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gevcnhrbw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gocjptxhz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/grqzwryea.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ghtqzqtsq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gwdhacfry.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gspdcbxbm.sHtML


<!-- 参考信息 -->