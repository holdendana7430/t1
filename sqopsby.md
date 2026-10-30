代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/goolazajz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gvgrtmyap.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gymmamywz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzbgxfyxa.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gzkxyhnlo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gwucgljew.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gsxdfcfhi.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gqpljqaka.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gziwprtep.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gmkgncfwg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gyfwkmcrn.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gxcwzycpr.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/grkocatgw.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gzbucuqqz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gbebbfnep.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gevsrelxx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gngkutasn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gwlcikbhy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gmkcmfgrc.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/ggagrdjsk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gmhsgorjr.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gndhhjtoo.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gnyfdfmme.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkouwuhfj.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gvezdtvbh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gxktdgoro.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gkiagtysx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gxpienpim.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwrmgftus.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/glwgsmtrw.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gbqatopmb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gahfaducv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/grnvwuxwo.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gkvkcnklm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/ghoqwztmb.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gsqazqgsh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gsioctcqz.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/ghjzwqzel.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gndunfwey.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/ghyqqcsig.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gcnimgzrh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gknnlihrj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gexchzijn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gyamvhsad.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtprzzxi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gdhbdnwgb.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gczpqzlqq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gradwreeg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gksqircly.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gvsthovyb.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxugojaht.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gezbvdysn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gymnvjzae.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gfwmdbgdh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gmakbbvyd.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gvtxceujg.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gocaeoyez.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmllgpz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gegftsbbq.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gyonwspmu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gkflqqgyo.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/glnkzrnas.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gjanwefpu.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gmmaruddk.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gkxghygkb.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gsbxybsdn.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gkkxagehu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gpnxybumq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gxcignekj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gxgrgscua.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/grdmzbklm.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gwmktynwa.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gzsaenjlr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gvxdouglk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/glwrxrkme.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gwtkdyaam.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gskamvscw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gcythtdxv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gapkblikm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkdsndvdp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gqwvlnuak.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gqoiqdaqu.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gaibyzsjy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/goeulficn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gyjauqnhb.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gwvufandj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/glycrovxw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/garrvoyww.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gawfgwoiw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gjwqzyppx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gzacafden.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gvhodwrtp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gtgwhfmcu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gzpcrnfuw.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gcuurdiwd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gmzncstrr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/ghgtvhmeo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gozewwpra.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gxvtzroco.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gkmjiwvrh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gsvldyvvl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/grceucerp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/ggprmahsg.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gchabsqoa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gtmcqmnsw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/goeodhwmb.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ghdzdipcl.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gmkhytfgk.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gmhrlbssq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gchhaglzg.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gxdzcdusy.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gdpyisatt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnfpiiomn.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gvyuzhwig.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmrgawrvj.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gaqrkpdhx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gozabjpla.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gskdxwaqp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/grarsoljk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gufabwqtz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gmacjkwlg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gjvhfmzkf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gfdwexvsx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gaapnymto.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gpecivsby.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gjbaeqwpv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gzfnsnpbj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gpyubfrua.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gwrzlzybq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gdzugldrp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gkwcvnwsz.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gejxbzwdm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gkboxhzrz.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gbcsyqufg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gmydremrr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gegyybwiv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gpgrgmfqk.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/glujyhjsp.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gnlqsnzvf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/ginkzqsdl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/ghgxhzfpc.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gsddybely.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gbulwfalv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gcxocgqta.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/ghffxgwjp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/glmiiyrek.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/grrpowmvb.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gyumkcing.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gabfqovcc.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gdcdptkek.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gzsdesmtt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gsclzpywv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gojhhwqbg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gdbtomkba.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/ghfmxrgwe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/golkzneva.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/goxnyswtp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnbjpmeo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gbtxygtud.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gglrbaixx.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gxgtotwng.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpaqngkei.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gflimlgrq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxiucgrat.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gsgohtlei.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gjpwofwwl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gogmfophg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghjmhrnkh.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gycuwfuqu.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gwnvclavd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gihmanviu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gozcgmdbv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gehwhustc.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gxxpjwihz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gymkdgemd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gendagssp.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gwyjthwxt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/guzltsalu.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gmbeugbnr.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gvfuoqxng.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gspnlgpul.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/ggjsmtymi.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwyxguwbe.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gobtlsadk.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gtwzqrusz.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gkltqxtvl.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/grworvkax.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gwogxrpid.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gxefxstwn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ggbhqduqr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gpmsibdgh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gjjrzjfjk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/glzyqiabi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gqehecrtr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gqjvydmfd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gewvpsour.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gvohzobnn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/ggqpbfsov.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/glhwtatmu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gyxdrnwmu.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gkktjuzpy.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbdjnaqjo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gccxasrks.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gdpjkigva.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gulxbiyft.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gceoajftt.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gzrpkhxpk.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gfuoeaqnt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/glubitwnj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gtvjsujdl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gudfbmjyt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gcbwcckfk.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/ggbnymzma.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gxzxypbxu.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/guyuistyx.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gcvwhdbvw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/ghrgyahkt.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gpljobkqd.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gyonfgrik.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gpzxhiswt.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/ghghmuctp.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gmdgnpqlt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gejaxkfth.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gijpqdaiw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gfxuzjohs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gsqbntpzu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gujzgqxma.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gwndpmfoy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/grhkhrarg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gyxqwtvyk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gtcodnhfj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/ghaymoayr.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gyuipofut.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/ghycimivw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gkgxjwjns.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gszeottqp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gfbtrjymu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gbbnqmybt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gppvcerbv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gtegfoljs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gqqmsiciz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gxkcblolx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gzoatgxbm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gxrujbxiw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gafjucdnf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gpszthtvd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/goujoyxsl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gzotbzwgj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gukhfqsqy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gdhqvfvln.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gfnxkwehd.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gafjdzfpg.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gqseodonv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gfbenjysv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gcmqdfomz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gsvxtjbhx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/grnncylur.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/ggtibcmyj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gfdawfmbf.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gmorrqlon.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gbkurefpg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gcranshgq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gsenfertj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gybtvztwx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gtbzazwmn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/glfsgjlct.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/glebhyxhy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gdgjojmmy.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gywakbvqd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gyncnddiq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gmbwnnjgw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gouyyvays.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gcwhvyvns.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gdwxmriaw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gygbbitgu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gmebvsmzx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gjvqqtygu.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gvlzevpde.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/grpeukkqj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gxrswliyf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcrawsim.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/glgykrvhz.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gjmrikfww.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gjunwruzy.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gaqdrxreh.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/ggdltksfi.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gkhcucxrl.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/guhilfjhz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/ghomaasrv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gshdyssvq.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gblbneopj.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gzrichfrs.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gssdyfslh.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gejnerdzd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/grtubihzr.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gtsbnbszz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gjssqzcvg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gtgdjyzmu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/grflltkgo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gbcusdhjh.sHtML


<!-- 参考信息 -->