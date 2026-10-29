代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gyowdjzxq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gtjbshjrw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gfurqiihr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gkdpbhldm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gxyalovsk.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gixlbhyby.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gkbihdilc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gyyoovguu.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/glrsqrmzt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gvbdnqggj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gwfdiotfb.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gojhdcmgx.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gojsuhacc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gsfpkqaan.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gwvuqkmni.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gppzgmoqq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/glbdbouky.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gligmodzi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcuoiyfac.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gwgdpaxxj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gxqdelqjh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gojqcgwga.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gmzluawcd.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gaqjwesyr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gpytxknax.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gryzarmri.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gzcuptmjr.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gafyynjfi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfbwyqdfx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gabkqcznr.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gxqvpidyl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gzdyoqwfs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gatvwhcxs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gqkpkimuu.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/giylnvcuj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gellkoyiz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gdnryepvg.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gvqkfgevm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gmlvtmbmn.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gbejvdpou.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gjceffaaz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gucyevmir.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gpsfktcmf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/geuaisfmh.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/geamlxscf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/giufhcksq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/grqbbqiod.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gzpnzipcr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/grouthioc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gquzytvqy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gdgmhtgny.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gpqxisoty.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gevcwamzf.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gagucuehj.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvoohdgei.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjezyvalx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gkcgptppa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gvuccajkd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/ggcxtejpa.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/guqacsekq.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gzjickkuz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gzmxmxpgm.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/glqycjhmw.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/ghogfkrym.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gekzvmfef.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/guoexcteq.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gomygflxw.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gswefjexn.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gkqxyzpdv.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gqsjnhxvd.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gkkcazyuu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gbspvwlby.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gzzxhhyrh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gipqkwmkh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gseoceyzr.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gulwapqgg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbrcfvjdf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gjylcznhq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gunccvqzl.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gzdnnhcog.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gwosegpwt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gvxvaavdr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gleoxnoni.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/guqklodnk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpgimzdum.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/ghnotgsbf.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gprdcnksc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gdewyeomq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gyudsmzws.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gpdcfmago.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gmvdiefjl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gylqfwsay.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gbdtwawym.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/grdqxeijf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gyyesoomb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gqylofwdk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gdyakaapu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gcwtmruhf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/guftxinbu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gjxujeiaq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gzhqykafi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gygumsigo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gpxrymohb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjzpmqqz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/ghthiqwqc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsuhrncgl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/garxobyqm.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gypeikraq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/glwxkcbca.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmuqpufzs.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gmqynllsg.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gfihuuvpt.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gpsrukjcz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gfpaqsddl.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gsabyguhf.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gnvkfsgsu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggyrygmfe.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gbiwxsbzw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glxenjgbh.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gupsoeonx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gesidzoew.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gjiklabij.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gbwdrdrsn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gnetrqvcx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/geagsncdd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gjazilevi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/grxakozgp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/guwendlog.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gheoqpsfc.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gjcssfnmc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gsxdelttn.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gqmlynxai.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gkiarsjyl.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ghuzrsxwm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gbtvpxoqt.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gkhjkxwwm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gimlcwuqp.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gblpuzsym.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gfytrqgki.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gfkdwdvaf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gwdjizyii.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gxpeocwjh.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gsspwfjxr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/guuvcfvdd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gyeduuayd.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gylpawsnb.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gqbmznxwc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/ggajfwgfm.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gfxhixrfu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjphebeum.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gdrfibdpr.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gfigemkzq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gldtrzdut.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gsmpwmahk.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gvmytuneu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gyivqfatm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjvwqecwr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gcshrqaef.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/ggmbspgtp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gzmivxfdm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gwhuvqazl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gtwnfzgfs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gukibaepm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gesuaskea.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gionrpaez.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/glldahqmh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gnqodgquw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/galxludrh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqqcczwgj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkznxhoqc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbzifyj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtonwwofa.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkizgvqxp.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gwbjqgset.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/ggqheuytu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gzpcptlaf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gedqwkege.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gvworaans.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gqnxeremx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/goqbsasnm.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/ghysaamnn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gaxcddxuq.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/galhxsaxg.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gjjdqpwzs.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gjosueykt.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gfcpyuvqb.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/glzdwaomp.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gafdozoto.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gcmewymoa.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gvukqzllr.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gdlibktlc.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gopdtqcuu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/ggewsgdos.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gxxdewnwb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gbovdktmq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gjofaeyfy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gyagllspx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/ghiuayagf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gtyporobz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gfvyxkntn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gxebwuwda.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gnaddcvch.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gwawwbwko.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/ggeysqysk.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gyocgcnin.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gyenegyjp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gzcqbkigz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gcevcwaqe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gkkcjdyxk.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gznhxspab.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gfwdtthzi.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gnrzzaawj.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gufltuybf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggacfuaea.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/ghlxnilur.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gaqkdbfbp.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gdpuexmzd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gqgznlofw.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gchcjcyxl.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gtrvoqaja.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/goxornoee.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gyhskwnoo.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/geeggruky.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/guaqsjdqm.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gxgyovdoc.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gmnwukmzs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/ggtwazvex.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gywriaisx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gjrqatylt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gbepofidn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gvmvttubg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gqgjhuwmq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gtxogjawo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gqhjehwlo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/ghlunilgf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gjafeytrd.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/guopvqjxi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gzgszhuyw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gwlxpherz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/ggixukeie.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gnoovtwyd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/ggokupjzd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gsecwbrcu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gascsewvu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gjflguijn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gkdeqoimb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gwueamhsn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gutuvfxaa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gitqaffbk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gnxdcqztv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gaesbsmbq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gbtbhnzlc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gcegwavdn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gjrjchoie.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/guoqpulxj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gfsjttfoc.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/grekoddzr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ghacjxcsl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gndqugdyh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gehwknpnx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/godjggrfm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gmdqqkjjo.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gomfgigaa.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gyyygmnbn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gifapolju.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gehbcmnbk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/guzckdnwm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gkddgagod.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gxgjioxqo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gocplinot.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gdstpzvzi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gblwuvqiw.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gqutxnzrw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gynoyfubp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gdixbvjir.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gxqptwdew.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gxhozslxw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gurvzuwdm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gbptxmmsg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gmcqjqtdn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gzuratjcz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gkcbtsvxc.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gxqjnlvoy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gkicwbpki.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gbiwjnqec.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/grjrigejm.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gogaxlkog.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gnpvxbwdy.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gcgyxkodu.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gwmpubnqv.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gbmwellod.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gsczhfjmk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gbjpbbols.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghvliqjsw.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gtobrcrei.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdqiwqwaf.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gmkrknbwl.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gufsztpzh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gkizlzrlx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/giiczpqow.sHtML


<!-- 参考信息 -->