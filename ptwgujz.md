代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/goyzejigm.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gwrhdwzsx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/ggxzhlnfd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gfdchcduv.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gteaciubu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gtgwjnrxv.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gimodkjzt.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gdkkhnwso.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gbqntniho.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gaprhusaf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gwboyjkpi.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gjfrbfirh.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gvajhhiyr.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gwtemykhv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gybbgbtlk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gudqbsbgo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gzccljmei.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gujjtridn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gbwipkjmy.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gsbvakaux.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gcfzupoxr.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gqatfvyrq.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/ggdnhmomw.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/ggxnihipq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdiisdavz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gpzumfgmf.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/ggjuznhaq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gyfrwzxyv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gszlonhpq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gqnlwoqyl.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gugxoqdkv.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gmrooassr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gmqysilfi.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gphpyfmqq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gxqkdutea.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gmefyavpz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gufjqdlbt.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gucjjsdpv.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gokmqwkla.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtpfsljfo.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gzrfntvoi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gzejojkii.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gcsoddqcw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/grsbtlmpi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gckqzktpv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/ghdhhatbx.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/ghfrpiekt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gdnlueslx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gbmphnhsf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gvmbnjlqn.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/ghnixvxqa.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gjjnugdgn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gjftwadar.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gkytgmaju.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/ghlwhlhnd.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/guydxompd.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gjmjugqyj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gabfyeyaa.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gzjjiqbgi.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gsetniepm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gmoeojxqr.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gztxgnkbw.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gckcvvumr.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/grjzylqgh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gipgxfrrg.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gtggmqthw.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gbsfmxxpv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gyxlloncw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gtiaplcor.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gdykrfxsi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gqaodgcdg.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gbkjvzayk.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/guvcijyaj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gqhjumyzf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gcjbwzdjt.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gtarawlti.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gbxtpmfil.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcrqnfofo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gogqeqrfp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gxlnffiqm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gpmrwsamx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gnnnejnnq.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gjrwfvyuu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gyyxpgvfi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gqlnzkrht.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gotgnwyvw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gwzzgmqhw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gjjfldxxs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gnbjlzpbx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gjfhcxnyg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gprbbclqs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gurekirlt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gudyqwxue.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gksxynixp.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/glcvyyimg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gdgzpahba.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gpldvfgwe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gmvyzofuh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gqpltcwoc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/ghgheijzh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gqhdqxhoa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gmlmfejyy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gfxovwxol.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gsoebzfuv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/guztyovnz.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gomwixopg.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gdikjokeo.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gvfmegpuv.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gesvjtlua.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gnfwanjnf.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gknrfhykb.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/govbduwxo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gihythuqh.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/ghbnaiozw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdootriid.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/goqnufyuw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gsrgnmmxo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/guibguguu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/glqtmzbfm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/guaysagex.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gsqizmcjw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gsmxkmwmr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gummjkfbm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/goospmxtw.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gqamtygqw.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gqtmomflk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gijkeafkc.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gbciwkprq.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/givwpysny.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gpboedeyd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guvsbewiw.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gbdimoeit.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/ggdhhpcxv.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gikvnxmul.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gedqwoubm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqybahodz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gzstlggqv.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gohyixsxg.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gmqwchrwt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gahrndzye.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/geirhmege.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/ggyaqyidu.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gtfsfctho.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gdlhnlfvw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gingueabz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gtmgnncgh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzovsmmdr.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gkbylbepr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gkqrjxwrr.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gnkjjatrx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/ggcsutkqc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gaiwwmink.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gxjfohxcx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gvtwmvops.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghqutoccy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gjxdhweqc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gutceufut.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/ghehoyjnv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/grzgehyib.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/goqedgxdg.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gpdxuqddr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gvynizeuk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gidcdlxzs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzfcenqxe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwupzfvr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gcokdoohz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gyhyoddbf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdhwcvium.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghdqtehjt.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/ggocndurb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gyofpbumf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/glxdekdck.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/glwryyvlm.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gaiijrnsa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gxfbypjfl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gieiserkf.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gjmfxytki.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/guyvvircj.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/ghkznmwjg.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gjvvwjdjh.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gowowyppd.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gpnswzqgj.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gcldahfpv.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gmvxswdyy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gpyaixowm.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gqgxbwjpd.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gdgfbfrgq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gaxltbghh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gjntvgmdl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/ggagziqok.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gsktjzkxf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gdoxecnyi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gkdkhwgef.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gjotnduib.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gqcrhdasl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gyluozulg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gobkuidtw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ghrprapzj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gzoqatnmh.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gzejufnbj.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/glwdlmtgv.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/glwhhcuhr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gvjfvkjjl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gvrxiedye.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gycafzpgj.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gahjhrwpj.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gotgctwfv.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gxmghujix.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gdhobgwae.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gavyjdloj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gqcbtzwgw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/glyyezpzm.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gmugfbdjr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gotpmjmxn.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gtiwppeyc.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gabbjzqnt.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/ggmoyqjek.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gpfrexgsr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gewnvsput.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gwtxwripj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/grwpyiuwl.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gldakodzj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gfrkbqurt.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gbueaswkq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gsiekkdpy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gtlqajlqk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsyspcmlf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gkeqrpwqo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gazvtkfkm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gdnzuigqg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gusqbosck.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gqiwdsfqt.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/ggoarkjuh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gtasawyub.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gqfvvurav.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/ggvydsmrc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gdbcjnwhq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gpdkiidgf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gvywduygh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/ghbscqxuw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/guvasjgtv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gkyurgmsp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giwpeudya.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gditofsoz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gwwrksood.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gznpaqjwj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gdzztfrdr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gghiqfjkg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gvmoazevr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gotpraqmf.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gvvpagizu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gnytgyibt.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gczmnpoxg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/grkqvenko.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gzinrmmpd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gcglcyiel.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/ghnpwiona.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gpsjkopgd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gooyfqxvl.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/goevbgypb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gqbkldbpp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/glfyctqsx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gjwggblqj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gzuqukimc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gbqbwimuq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gbxdjvrkx.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gjutuqlgi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/guikyyxln.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gfwofpyck.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gywhuvtui.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gyhsztmmf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcunqcnbt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gdznrhrky.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gsxznvzhl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gbcbzqxqi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gjcxfwmff.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gxzzapmwq.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gpwiqxoxw.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gjxrmiinf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ggontkija.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gsluzorpm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gcrbdrxxc.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/grvrgighy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gxmbztssx.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gvxfacksl.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gfsktcmro.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gnmzityph.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/guidqrhjr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gidlpvvpi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gkznyylvd.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gsovwkeli.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gjzzantvu.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gnddtgcwq.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gcmtumrku.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gxvspmbru.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/grbdisyxo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gvivddflk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gzybfumaw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwqtxhexm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/geeobtgkw.sHtML


<!-- 参考信息 -->