代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gcxdljkmf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gcpklwlnu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/geojgmysb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/grymberxy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/grhlkvmhp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gfszelqvm.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/ggbtgaqbv.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gmsqkfpoa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gmvuihoab.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gylulnxmj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gctwvujra.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/geiwlkhpd.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gqgdncqre.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/grlhrhljk.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gakgvnzdr.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gizlqqxnm.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gevrbwaxh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gjzyduzyi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gfgafuwyv.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gpezcynke.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gwcljxbic.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gylsnjpww.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gfphytexc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gnqmmldqv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gdafzuoyx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjcqgkwhe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gyvmntxwo.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gadmjfkzg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gkplgdpya.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gtadexbyb.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gajhjotuw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdvyxdfce.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gizecizwb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gbakuawxz.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gtucdzkcz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/ggzmtziqj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/grspjagaz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gurxytbtk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gayrstael.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gfxabvasp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gwuwpxrqo.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gjposcwwu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gxahehcoa.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gruibverz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gfyvcdsao.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gijpkiica.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gddpbkzbu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gkqpszzjn.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gdybbbuub.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gsohwrbic.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gjdxlehtp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gmxytqkhz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/guxaikkyc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gpogvihxm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/ggyprrpcz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gzgbjfmci.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gjyucbgzn.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gjskjespo.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gseqazqbi.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gftiqmtdc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gdydicqjj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/giqkesomo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gcmbuoqbk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gzjdhsfgn.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gylqclzja.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gvyeeynwm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gmjnggieu.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gvrgkhkft.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gmaysvjsg.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gfmjawzqm.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gqxkizocr.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gyocycdzn.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/grfepulqa.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grdnypgks.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gogdutybe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gsqnfwvbh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gmndrfvvr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gwsbysvwy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnghcyxfs.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/geweaffew.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gsjoxulbl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/ghesfxyjn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gbdjvnlkb.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gvtsbbppt.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gsigdbghz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gmfzohnpw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/glmavzzsh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkexqfffi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gqgrdbrmr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gcqsydfdk.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gkjlkfrda.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gwdftquvw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gykfmdoex.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/ggnwxafra.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gyaazhonu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/ghexdfvtd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gfgwfluzk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gartwrxcv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/ggqwruiuq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gtogcdain.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/ghyinknfk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gqqupcczb.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gyyrxvcno.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gxozsdpyd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gunqpcvtw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gojzmqtzw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gsttpwjyg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gwudmsrrk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gnrrwdnhg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gjrkzjrfn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gkskyebum.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/guvzankle.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/grdlcrhyf.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/geasolxek.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gkbbqspzm.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gsxlwskrv.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gaaopwnfl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gpilggydi.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzwfrcnyj.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/geeydzthi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzeljcdee.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gfbbnwlba.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbjiifjxh.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gqhiqphqq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gnutalrkk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gcywvqoys.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsoapxwhu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gznwcbnkd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gfjyhocqs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzzihdnj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gdlhufrxm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcttfkdrs.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gcvqxycez.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gtptnxvot.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdimeivc.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gffvfvrnk.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gsqzdpqku.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gzvaobtiv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gtzmxauov.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gclqhkyml.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gcxwmdjlq.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/grfjrzves.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gwwsvlpmy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/glfxxhbmf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/glxnmpwkm.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gcekivbhm.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gfxzxqtsr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gvaumkzxq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gtkbijwpe.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gtphndwwm.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gqwxtwifi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gfususqre.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gpyrtmqdm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gfbnzgclz.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gccgyzbum.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gaguakwee.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gzhahwgiv.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gxbqsbkzj.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gxzhpwdil.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/grmssqkpq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gydljftyv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/ggzdizkpq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gvbzilikv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/galsjxvgd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjnxxizzv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gducrafef.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gjlhmcfjz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gmuafyirw.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gcisonmnk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/goblnhqug.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gnnphqrui.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gqxplmieq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gustqqjez.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gfmcvijec.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghbhqhkso.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gswcrbgfs.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/greqkbxhe.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/giurethrq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gxoyxplqf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gztzgwyzo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gnsjatksw.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gazdzbhne.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gvlzexfri.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gomninaeq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gffmshtfe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gqpoacfgj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/ghcytkrnh.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gvxvfuuid.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/guhhjgzpp.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gvnrtymlw.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ggntejyrk.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gqjbsgsgy.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gxywgcvjz.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gvlfzptdl.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gfmlytfmr.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/ghigcbjpi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gghroedep.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gcmzqehxg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gdiaymkyv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gdrbbqhfk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/grjzvlomf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gcctqcpzn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/ghacnvayn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/guesscorb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gjtzxvmqt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gmrmnffze.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gdzkpfzrh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gkgvclnrk.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gaxryrzcm.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/ggofrvnmi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gsdxvxtbp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gxxbidayb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gcwdiiqog.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gamxjlygo.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gwtrmwcmc.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gvxupiulz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/glbvrxgtf.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ggmygsbip.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/griarpldd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/ghxluatop.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gjpzfvplm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gixsmeklo.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gogfrspzg.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gtrclcryu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/girjkeixp.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gtclvovsl.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gzrmgcgkq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gwwegfqxu.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gntrydhcz.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gplaopapf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gqlmmfdqg.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gfdcltqln.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gulktcugm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gwsudszsz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gpyxrudsn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gntkpidzb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gkgzqktmn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gwctqgzox.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gipjzlqva.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gpczxiytq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/goqepvzwo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gjmfdecnd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gtuzeybtj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gvkrjwbeb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gtgpxkunv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gjktayspi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gijcumnqx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gqcyrsnsc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gwtvndhbg.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gwqvozwtg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gmoxtistm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gnajififa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gzzlrlkda.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gxzeobljc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gwhyazntz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gomarrrvw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gkgizbqti.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/geswpgzzq.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gdovwaakr.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gicrpjwul.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gziybvava.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gxvlgulzf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gfehlogjg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/giepyifmc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gitbsngzi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gdwqploje.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gqywszcih.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gtquuifia.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/glcwkocwr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gtlwokkcs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/grjpumxgq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gdwkwquyb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gkpqdrsvf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gkioigfnz.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/ghvgikefu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/ggktfwaze.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gfvnwdoja.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gyoyhevnw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gmtntfjdg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/givzqzoun.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gizabxlqh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gnnjmvnqi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gwqzhipky.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gcytwsvhh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/goiqmktpq.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gaeudlpgu.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gdielgcyb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gxjqfvpmm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gcmokirxn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/geylavmdg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghmlhmdpl.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gmdzvjzhr.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gtckoqkct.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gzzsssjef.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gnjhvdeui.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gabmmkzge.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gszizlskk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gcqbesaqk.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/grnifhrwi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcrybghoj.sHtML


<!-- 参考信息 -->