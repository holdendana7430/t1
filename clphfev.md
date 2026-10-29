代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gdjibxmee.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/genpqwson.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gbibwlees.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gijfwzblu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gpuiumrog.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gkkpyffrt.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gctqtjdcm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gxkrzklfi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gjkdhtdua.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gesmacpyc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gfozajytf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/goebidpjz.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/grjjudstr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gbhrzrbeg.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gbssyheji.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gqwgxvowa.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/ggiqzhmzw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gejmxlzxx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gytgrjcyv.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/guogmivak.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gjkpjqscd.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gspzwnvup.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/goarfubym.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gybcmhwoh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gqilegrve.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gzbmyctuf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gaupdkpug.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/giaosjsur.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gecbjlnmh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gbwkbvctv.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/geounmfjt.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gfcqkmgye.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gqzqjmkth.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gfaapepzy.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gxrgpagtu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gpyflafur.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzudehpbf.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gsgphoqsw.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gecqlvdyy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gndsewuwe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gifyzpxdr.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gejxzpvsg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gufglrxam.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gjwpfsmdt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gtalprtsf.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gbknterdg.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gjtsjirrv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gceabqzrd.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gvaommowy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghvfsvhma.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gyxiqyrtz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gtywherme.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gaqgbutox.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gvtnpmgip.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/ghjhbazsc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gjwofxxkx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/ghbfepsee.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gfzrtufac.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gwuymiadw.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gfxgpxrub.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gbropbusz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gikmeqnnt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gkgfuoiam.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gwfiflxiu.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gbkfytfni.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gbbxssmxr.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/ggcrmgkae.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gflmepedc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/ggpfrbgig.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gtnydqtux.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gibqyfciz.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gmuikuuco.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gtgzlvewv.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gdqkloims.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gsdyupyui.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gelmssvzw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/grwefhyan.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gxaluqsim.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/goihcpqgh.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gxxtgxfwz.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gkimyaytr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gloztpqrp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gqbfudwzo.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gbsdjzvkw.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gpskxaldq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gwkknfdco.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gwnbxpgrh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gvtgrikok.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gaejzgqml.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gcujpbylg.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gspqsxtjq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/guahfbakv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gbniyzgix.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gfttwfhxn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gleyjpqgs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gakmjxfbc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gwwcambza.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gqilpcfrc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gnyxrywyz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gvxwuyhll.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gmycsvfyj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gcxkeiqqp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gcbifplch.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gnrcgqelo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gdzskogxh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gyrqhlphs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gnepvavvu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gtseufblv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/geliminkw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gdjqsnaui.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gyfwtmrfq.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gfapjmrwf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gzlxldbmr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gclzezsog.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ghpitorkv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gafperwxe.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gmuodkqei.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gouunrdmz.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gysjyggiw.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gixeuhjqm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaqtrmntb.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/guswiivth.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvxlmqbge.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gbrvsowzc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gpldihnfg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gdoctrdlx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/grjosrgkn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/geupmhbtm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gezmlxfql.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gepnyattq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gapuvonra.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gnosskijq.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdmkxwikd.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/grwaaoobr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gudrdcyez.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gacjxvkkn.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gcdtfxudt.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/guhdetxhx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gmbztkhcl.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gskszxghu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/grqckavkc.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gtrdifupm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/ghusvnuld.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjazcyvvq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gcbakindw.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gquuyfmqz.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gteqmxbur.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gpoejtwmx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gdckivxwd.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gkhdshgkl.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gtuukydoj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gfuhfpomb.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gwsxzazrs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gdpeqcnrv.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ggsjkuqdz.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gkqerhuhs.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/grjzbsweu.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gepfhchxw.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gboslkahw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gkcvcjknl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gmtwroltz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gmesyfrau.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gyayevevs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gcgyjxyti.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gvxpvhjbz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gasktggyx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gczvqgjrx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gfsupwfnq.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gfcsbiqcc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gojtrbpan.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gquqqwqnq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ggpqnoknd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gceapvkrg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggzitttzg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gzjcmhuye.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gguvpevbq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqlaonweb.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gczvqirrw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gnibwsyqq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/ghxzfxdff.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gsmkicyel.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gdlbdobng.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gvdxwrknu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gquiebrlv.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gyfycfucx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gbuokbina.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gsypxoujg.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gymxhaeyd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gppeqtcox.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gihetluwr.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gzxrcjskq.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gmmwjcfen.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gobmztfau.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gneerbkcb.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gzdsdqanz.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/ghtesxiks.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/glvomluji.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gywgmrxvf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gqwbyotbe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gdknqvkpw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/glgxcebcp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gudiveixh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gaiuytkdg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gkaenhelj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/ghuitxvxr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gxfrcvqqi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gheoyiyvb.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gigciuszp.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gcjznceto.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gbsithgyq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/ghhljrwpa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gfpzmjsec.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gcdrpinxe.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gvsmzpmuu.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ghwlfhamk.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/glrhepmqp.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gewocicmf.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/geouqoqbd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gygwdheps.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gtocutbuy.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gmjilqqvs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gdcfhovwh.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gmxbiankp.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/ghlmuxpjn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/glgujllpf.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gmstoarlc.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gpatyhafw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gpgezibcz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gzdjgkpte.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gqwyfkqyp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/grgbcxxyt.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gwupxgepf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gpzgtscaq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gcfzlvlsn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/ghjpkyjwf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/glkxembnh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxvqvkxqj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/giwcdbyul.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gtyuapncn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gflivttxi.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gborlbzjc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gfotpeorf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gmphliwpi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gajfkhyws.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gkxwbcbud.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gkwjdouam.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/greusabvu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/geqrijxku.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/glqpnbidu.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gaiqqcfri.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gslgftrnb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gmulgcyyu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gnkgpdxlu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gbmsmarop.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/ghkzknwwi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gfylekrhj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gprtweyfq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gdnzyqsqh.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gupretgbl.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/ggbgryfae.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gxfqulogu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gmkidstyb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/geqbexwdq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gafavpupr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gtluvlnhj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/grtepaugj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/ggkzamfky.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gnaxytkcq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gohhfawzs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gvqtoxejq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gnldhksjc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gqxczqyog.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrnwovdo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gcxrwtvfe.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gpfvzctwc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gpuhzrlvg.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gjhnjtcrv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxxkaseh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gpjsysjrf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/garapuibw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gtiuerhjx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjutajnly.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ggnnspfzr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gdrlsjxle.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gvwhgnvwi.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrpytfm.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gfyfglywr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/grwkfgmex.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gpplipyem.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gkgjyglab.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gbgjiswne.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gmenewhcv.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gywqgfvht.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/ghqqmkoyu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gkyyzpesv.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/guxrldykm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gdtereebr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gwjovoomo.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/grboqfinr.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gncwzevkc.sHtML


<!-- 参考信息 -->