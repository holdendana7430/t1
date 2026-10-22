代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2parkmybr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hhhvvvpq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bqfyijyx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jchqqink.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kduajkui.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yvgnvawu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2aydcpbrg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2oeczhaqk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ztmmsddp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2apnrsdtk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oreujxdg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vvpmbucp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fqtocnry.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukkvmjdr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qcpalwbb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pahdforh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yclndioh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kozhqfhj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2tabwnqbw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rvrfoooc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sduzydgk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wwshocdz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2aejpztbp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gzhteqnn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lolbcvsm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hqwdekqo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ujvwhllx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bzwlkwif.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2souozkjx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cxpvqtbl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wayvagfn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2kyflnemt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yrpvbwzj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ucjulbnr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yrqqxosl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jomedvdu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kmnzmtcu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hgknscio.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ismqfohw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jrsdxrht.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cqykpbrs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fkwtmbuy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pcucrpmw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zqgtnjqp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2kysjcdfe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2gpotmacs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hlcxorng.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ujpaquxy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tbcuvora.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rjqojggj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oukmxwzd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pyftrlng.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2outgmmck.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hqgicrqu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjbzmxgy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yydezbhn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ipchqmbf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2egahibsa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2eunqvgkg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zpxnteop.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2rguwtxic.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ccvwjzff.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wvczuwdb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ooetfebq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ingnvmrl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2htousrzd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rbsiyihw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zssgcalp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qctbqlzl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hpmwmilt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bgussjwy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wbyyunup.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jzklhdkx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qucvbams.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2keawlmon.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2knwbeogi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpysvpw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lxrgofmz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2okndgyfe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tvrsdwyu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2usimaqxk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dclrcqce.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qwxufygd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2skpxjqre.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2txhudaun.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nesdnkpe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2aburaonl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mrrzvsar.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dlbfocez.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qtqilmoo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bebwqtyu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bkawxlgu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oxtheqbu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ywabxufh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ltuljnut.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aykrpsgb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ustfvwpd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iystcfxp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xecsjhzh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmmclhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oowijvvs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2efcfnnkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfbitklz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oeogihzf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2iikdhkbe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dtisgbcl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jylalarv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gnbsbxld.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xymylwgw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hlaohial.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ttzezbat.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vzlfgshr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtrcbtch.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gccbyqcs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ohvquqqd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dciwnpnf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2duuruuhn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pzwmczoc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cjcvrbbd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2eniycmqn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xfweigcq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wgxgmoaz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ndsixifu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2skvlfscl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lxsmezfo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2swhcaksu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ttuasoxk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rkemfnsu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mvaxboxc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ymtsnojp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wwybaxii.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2udxyobqs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cpuobmkp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2hwkzeufl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ouiqbwea.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xnlmpksc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uhtooqvf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hnmchdnv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bsajpuud.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rdxgwhpd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ajxlsham.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nxnpigcs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gbfjxvlf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2redbhrti.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xwazmycn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nkkczmec.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vynrmlmc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qpryrbtk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pesbfbob.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2esbhjtst.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbhphvzp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jdmloxhq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iqbdtwqs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cvvphmlp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxwalmmb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ditgxvrl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zxtbvfcx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kcidssvn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2dnhstbtg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pblpnguj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2aowcekeh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ayqpwiwl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ejaulssw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ywrohzuc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2dlqmgqfc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ktwndwdc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hdclaqob.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2whauznxq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pfssnyha.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fiduutra.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bujytbpp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ocwvmfwm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2isknpqel.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jprxziwo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jfazbngz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2iaalpvim.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhzaool.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fxswutje.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gtzrjqcn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xmfdyljv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2daxcicki.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ssgwrpqw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hvwkcbei.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xivnbqzl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ywaqnkee.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ivezfwfg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pvpqtbar.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jdmefiwi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ryavlagd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ocibbhsi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2irxmavzl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ytwesukm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lllkjjyf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2llofpqoi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jjlzlbwi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qyyzvtkz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2swnavphv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qphtqrox.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vykfgiqg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2udrbxbvz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gyrimawr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ckwjaogd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2decazuyv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kfsvouxo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jxmehteu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fvlneddc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvmnncbb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rrtstcxl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ofgfqmsi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2arvwcljo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ziporhen.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2cqnzhcvm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ienoxqha.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2girktjrh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rudcaylc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqwwbfwg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qajexdyz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cdoxbmwu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nlymrvje.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cskgserz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2prbmpzmt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vofuutoc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kouyddsp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qqwvaodo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tgvykiwe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2elsnyved.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2sdqmmjuc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2eaydwnba.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dlggjbcj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nqjjedix.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jdhjqcea.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbmpyiyb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2oairaxmk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rtyhgdzt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2npafljiw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2snlhsdkn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fhzmxtxs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2yajtuoig.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2aiuktwwi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bekouccd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ugnwmvgc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mpehycga.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gfbkkqqd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2unzhzdmv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nwsvsimj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ouwnkqao.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qrmprnox.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rwjqnbbn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hluesbyj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ygpbhzdb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mdfmnxex.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2aafrimoh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tydqwcgw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2veqsinox.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2acdwawta.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jkpgawaq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2djucyodb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2njriftnp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fywldxew.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lxmeryrd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wujeseoy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2krsfuion.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkeoges.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mygvzaef.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vriymzxv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2qcfuegsw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ebyddojo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2odjojiuk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2etrealkg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfkzbse.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bghevzfw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2sggtoxze.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dghkdpeo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2opflhnpe.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2einnswjd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xcrvsiwn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gsyhoqvj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2naaefrja.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mrvsvabk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nxxgdlya.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rwncjpfc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qumnhitq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxkufdve.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vqmtdnku.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bnpdsvpu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nraelnou.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2imklpref.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jzckjkdy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iwubtgbt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bzuwcalg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sqipyykm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fmryvqfq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zxgenuxe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2oomdlrxc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bnzxfjgm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dvfzulcm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dyyxqzjp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xirhgayl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hqtnhdue.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nxbwdohz.html


<!-- 参考信息 -->