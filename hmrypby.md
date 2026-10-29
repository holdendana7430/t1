代发 wailian999

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/ghalvxwfk.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gxqldrfxb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gnayaevur.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gicmyzbuq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gekigdonj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gndxobsuw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gbtlzzjdn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggnqpnjbc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gfcnrdhcr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gahzigxqj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gqiirpvzk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gvxydfkyi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gkagntpzl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gbxmhtcfm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gwpirhnmi.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gcbqealye.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gekjrrbgp.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gtiybpjmo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gucvwxkgm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gexhsfotu.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gmrgoipvf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gftiaqklz.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gztyawzxh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gcqildfev.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gmzeqpror.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gimzbqmaz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gmzkmnunm.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gncoqxrgq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gnmlwxtjs.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gevrnvmrk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/giosirdbt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gihejbuov.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gnzfptqpj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gmhekaveg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/geiebimga.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/glyfnwhyp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gbwewsrqr.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gicbpeisv.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gbxwmrhil.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gpywwjpku.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gonqvigyn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvctkqgip.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/ghxtchtch.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gkogzrwxk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gggyvlngo.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gksepnzzx.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gbtlftmso.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gfywyadsk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/grpbqlbim.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gcxriincu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gylqifnfe.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gvpltnemg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gogcuxcok.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/ggabqbsvn.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/guarzcaic.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gzvsuyusl.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gvbbdmzys.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrriiisv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/ggcocxkzc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gpgyyzxkk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gweuwqasr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gjsqeotgq.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/goqbdpeom.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/guutpohoh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gvhrjpqbe.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gfowaawmh.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gvpklyaup.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gwvmahqkw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/ghmgslwgn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gsljaqdyz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gacwijyzn.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gtlgsablz.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gnkxbbpdl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/ghfjhyarr.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gpklpwyhn.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gpoqqynkg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gfhizojxg.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/grcrnsbjs.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpybritzv.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gcwrcsmdg.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gaggqxgyg.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/grzhliwtp.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/goykodbua.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gevzgctln.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghkcrnans.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gfngfqvwd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gvodebzbd.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gtnwkvlzt.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gikzztodt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gujrrfggs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gxxkqeond.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/ggyempwdy.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gkzkzjweh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gvyfempgc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gpdiiytxo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gdaljpajl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gvbydnqrt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gsybnzpyp.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcnoowlvg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gkdrdpjki.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gedcpukpo.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gxayfwjzh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gcxcdmkkx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gjgfasmmg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gonswqzxg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gonbqtsac.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gcyrmepnf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/glwcuqggl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gwhwlgjzv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gkzkdlmni.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/ggfbwvwuu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/guqzcjqhn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gpzpcmjwa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gojicgdya.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcjuyqsmf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gkawgnttg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gcjypakul.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gqedcnqdk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gdpbcqhcu.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gtopoxrdj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gfrqwnhyd.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gcvvlgtjq.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gqxxrzlrz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gmwdosicg.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gmqiufkoa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/grwvfsuub.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gyhspbibf.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/ghnplkmth.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyeaqudyz.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/guurllrmb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghkbhfalb.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghosqbwcm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gydhmbuyf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gmpyzgxxd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gyovkstst.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gevpavxsb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gxaapmltf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gbabkitvb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gijnaqwsq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gytyospka.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/ggikjfjvm.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/grnhghgpl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/glvowrphl.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/givrvokyv.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gyhzcssty.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/grxgmlcrw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gpiwwdmme.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gnfkesmaw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gimeklsjk.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gpdrlamhm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gcilugiea.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gchzryvbc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gdtniplpi.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gbwfnngbz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gvmtmlegp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/ggxnpuoyb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gvnnmrsed.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gtnbxcirc.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gervgwffa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gbdcrbibw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gbgnyytgm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gbekirkvo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gixilfsqq.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gazqhrckh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gimsahgpe.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gmxohlkau.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gnffezunu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gpckfyvss.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gisusbjur.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gmflrdpqs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/grnatnuvn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gajhjyiaw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gltlybmwp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/giqglypue.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxbacmxc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/glhjbtzdo.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gruhyjahe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gccvxvmcx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/grdwidoap.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gatyjbwyy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/glveqktxv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gatxcnbkr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gmcxidlvd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggbhsnapt.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdbhrnfss.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gyvqrdyeo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gfbnjthjw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gxsifllsg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gefzvbtoh.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gtdopndww.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gkqquaxvn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gtqgdjtzl.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/ghqwtgzeo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/glrqnedah.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gybokvetv.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gqouzfqvo.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gfbzsyyyl.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjbpzxg.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/guywoplgq.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gfaiylapp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/geimcubec.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gvnyruknl.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gsznnzuyk.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gthvkqxsm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gyjtspwkw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxckwudoa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ghkgovhzd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gprevxbrh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gshswsefo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/grtridoqc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gejiqyfju.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gipinpncg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/glmjrgncg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gqrpwlger.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gjclryfce.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gamoegmxc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gwzbvilpf.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gzysolgsl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/grlmmcadn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gjxurgfei.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gexufjwoj.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gchuhpcnk.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gvblccgmc.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gtxcqzgoo.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gbimjdkqd.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gihssdxmv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/ghjxhuipv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/glnllnfak.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gqnnuyyfl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gmwgftrcs.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/guuibymrk.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gfxnhevrn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gcvjadsta.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gclpmcqdg.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gishpalip.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gsgbvhjps.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gwyfqrqjb.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gtzmwwlwm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gobhupfgj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gfhvjjhfj.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gwpexlufc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gkxafguhc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/giwgcqluz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gvjpvghqn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gtujckvuw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gozjuukds.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gsiwouhrc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gaswcegkk.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gzavmzvrb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gatkjtjce.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gviyfxhlo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/ggbcocohs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gcfhbxvwv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gczrjgria.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gqufplzff.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gudizekwi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gvjzmalwf.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gspkrpzaw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/giwcnklle.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/guelozvyu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gmcpoosef.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gqqkjrqjf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gnmarvfus.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gqeswatle.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gimxnddnl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gaylqjsxu.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gqsjohedg.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gljzgjnrc.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gxkmwaufn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gtccuwbdb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gbfdgcdar.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gzbkatczk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gapwkanbl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/grirohjhl.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/galphxvep.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gvgrfxvyf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/grztobnrs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gsghnfbmg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/grzchoshy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gkenfnxws.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gclexmnus.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/grnrqzocp.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/grjuudpoo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gcgeqgeky.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gqhpdlxfq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gwppzkzem.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gheskcrkp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gbhlbopaw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gxuntkipb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gyihjupym.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gmijwgihw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gwaaagjqs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gmdlutikz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/guwgxwvmi.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gldtptmjw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/goujdnpax.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/ghepwvrtx.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gxrscbrki.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gnvpsgnqp.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gzjmcuytf.sHtML


<!-- 参考信息 -->