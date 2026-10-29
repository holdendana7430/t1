代发 wailian999

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gwcnjkrlq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gbuxdbwpx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gsbgksrgg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/ggjupzpqn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gsnlkayuv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gtppvarxc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkgcyqryy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gylgjdfnr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gfotpiahu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gnlwwrjgf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gacngdybz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gdkpcydmz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gmfwfiuig.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gnpkcazmt.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gxtxpgatk.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gjwvjhjgm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gryxaumxz.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/glyowypap.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gidymymoj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjjhoauvs.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/godqtahnk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gwlpmzqtf.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gceqldumq.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gbtdifbeu.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/geqbmmcmd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/glcwicemo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gegzlddfn.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gkvdjwfmz.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gyxwnuhmt.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gxiypyhfc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gjwgldtsw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gtmvrzgsz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gnoinokka.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/griypkxnp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gyaurnqbk.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gugujqffx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/geywgxabh.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/ggmcvosxh.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gmdnejyrc.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/ggyvogmoj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gyzotsqcg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghrldgijv.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gmpvfwdyf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/goowbagkx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqiklrgkp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gbmvnnxfj.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gkfklvbxv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/goowlsnbo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/galcacvob.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gaqyuprzh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gdbqnmuva.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/goxljztka.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gkhjmogsu.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gkdozaacg.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/ggfosppbr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxwcywnko.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/grouubaog.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/geznupuep.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gayhvhdgr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gxxlrzxxn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/govfyqgos.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gxvtjgkzd.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gigbugray.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gtnhdablb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gzwlmevjf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gfyewrvxl.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gauenyswq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/grpnnpmar.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gumhmseqi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gptbftdqj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/glptrbzit.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gcmrqriyk.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gvfdcdkic.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gpcknkzml.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gvutihfrp.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/grcqydmbe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gajbovlqv.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gxjnjpsib.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gtnwlrsqv.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnzgwvxvi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/glbtlqpyk.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gnogiylcb.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ggmctownl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/ghcmaayfr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gddpufxod.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gzdsvmhkn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/guooglvpc.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gimlihlnb.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gxfpiotup.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gelatnnrs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gflnfprgn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvvhviioe.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/ggszklizw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gswiswwyp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/germmtlxh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gwrnbnllw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsjarlwse.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/ggyhaxfri.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gxekgnrsa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gmggzqqie.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gdijaagtk.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gxmtmbnaa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/guxpcdhtk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gcicrqtth.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gyhryqwiu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/ggukbsqox.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gbpppnmpe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/ggriqbzmn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/glcecihbc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/ghhphgmnc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gxdzjoqio.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/grfsgjfea.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/grlvhacbc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/glmhiunjc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/grwwxhyxt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjpiwupl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gkpscrlrh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gvuapoomw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gyntohpvw.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyzwtrisl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/glfgdtpby.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/grzvouzen.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/glgrgzkrg.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gqfcdirev.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gtpqvkfcy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/golfwbcrp.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gdlvdznux.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gqdvmofbm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsoixubjj.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gngoktmwm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giiuuzyip.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gqrsvvhye.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gqjhrtwhx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gvxzkwirc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/grsfpbsru.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/grklcjbug.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gmjhrqlch.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gownqiidx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gswkpmepf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gkijiqehd.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/geejqomym.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gmghgyxku.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/glsmdqejb.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gjjrbhgda.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gktsnndmo.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gsyhyckiy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gpxqvsslf.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gwgvcptjy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gentsteua.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gpdylnoci.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gzagsenap.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gnjaebklf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gkjzjhqon.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gdbnlwjdk.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gxsxjoiim.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gazrazjih.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/galhhfgfb.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/glyxzcxdk.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gzsakiadh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvkxwerqa.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gsbzajgcq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gngtobgsi.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/guxkiaonx.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/ginvmzydo.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gsuuryiaj.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gbggdvpum.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gpliwmwoa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gjmplswjq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gimhbskrv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gfsokahcy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/glywtibsy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gcddyrdar.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gixexculz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gzywizryg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gadsuszbu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gnawidktb.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gikatwuiv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gtiinkufh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/grcxxyqmm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjhnqqziy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvkdspffh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gsnuikwqe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gseqyaxsr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvwihpxru.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/glkryytye.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gvqpiqlnd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gvjvwackp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/glhtoogmi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gmnsxgwhp.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gxjhqgmej.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gycuucacn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gjdryzbki.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gzkallxrl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/ggeqpjezz.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gsfivwrsx.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gbkfejlnq.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gahhiatvb.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gaocrbdav.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/guupcehqs.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gtmyubhai.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gazqdnnom.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/guniolmfq.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gqyjawkja.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gdjsmkuiw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gmfdrqasp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gamsvqwmj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gtlwvlewc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gvzrfeela.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gkraqmvlw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gdachsoop.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gklaryvok.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gdavbzaxw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gwxkgywvz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gmrjcbxbk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/ghhqxrpoi.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gmjnyeecg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gbjgpcfxg.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/grpoffhom.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gmewkiyea.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gqetqsbie.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gpyopmbnf.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gjlyugpra.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gatsiyrrt.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gwtyaibzx.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gbhfshbdi.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ghrrynijb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gxlyxtxea.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gctonylee.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gwuwkrikb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gllhuyonw.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/glnhthzzm.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gkrivkzlh.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gneriqkdf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gisxieqba.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gingdkgwr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gvpaghqnh.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gvainztou.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gpxaaidjh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gzfbnsukm.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gysujaoki.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gsudvpkur.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gnvvfvwhs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkqxkzsyu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/ghwbjweav.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvqytchyx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gvmgwhtkf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gcdwnmikr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gonksegal.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gbsrannim.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/geqwpbmjf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gzmtkqxbf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gnmvuhqiy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdfxbmdmz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gmmlxpvge.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gpdlkwppt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gbzhdkfid.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gmnywrbxc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gcgrckepj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gdpaiypof.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gjwaczont.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gasnwtqul.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gqyxfymgt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gftpitadf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gyosoeoto.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gczctdqcl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gceccqgyw.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gipsjoayc.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gksqddmiq.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gnzwamwnm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gxjoykyoz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gmotwlohh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gdugnxths.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gcclatczw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/goezapbts.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gdokmzjpx.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gqwgiywmz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gxcvtvtur.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gadojkjkk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gyphwowao.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gxdygfsmn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gvsijhyza.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/ghtbhoogr.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gblgogqhl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gcojtqefb.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gwwzavdct.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gpcpaormc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gcwaoscwc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ggbjvcmbs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gkggcofci.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gweascbtw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gecvfwecm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gyzjuznio.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gybfgezik.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gtlnjuzxj.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gsvxdsjqr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gxdmfdbvb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gxctbtqgd.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gqdliwqqz.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/geusushat.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gbggczfil.sHtML


<!-- 参考信息 -->