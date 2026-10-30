代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/giqebxzqt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/garavpprh.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gyhtgxtqr.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyesqnoqg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gqhvdoqfi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gxlgbhrhh.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gydrzihif.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gmodugqem.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gvnxkarrr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gffyqyaeb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gxipvzmeg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnbciusen.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gsdyntblx.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/ggwpetwyk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gmzyyhrrw.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gxbubntmo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/ghkiklkvj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gjasehlio.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/graalqmgo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gqhdgxsea.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gohaccefi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gejubdzcu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gwpqivoiu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gfyzvduxg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gttnspzmu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gpowloajd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gqoobmdhd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/glpkhvwoz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gthtyweof.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gxttpgres.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gpinhgcuq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gdkwveadj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/genfllysy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gbeaemyac.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gjvueyxyg.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/ghhvkbrru.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gedyakwnu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gbszioeqw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gnzyapdiu.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gqrzkggcu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gysqoyida.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gbtrzfabg.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gaptcwnfp.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gidxkowju.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvmaftjlf.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gqcusxszg.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gcamahdse.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gkyjjdtho.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/grxeztojh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/ghmxwmilm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvmcnfjko.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gplzqpimg.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gucmapcmp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gbkxfkspb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/grvfucazx.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gmwatzcjf.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gzzkrqhmd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gesvdbwms.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gywhmchpl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gkwhymukq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/ggppivmnz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/goqknftbf.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/glynspocl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gqzitlbdf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gsqtmzoxr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gbwfamxzb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gxdcrnjpu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gmljikwfj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gsxngbjvk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gzfvtynaq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gpalkqnbk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gxdogalog.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gasrnifes.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gwrsivwzv.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gzyccxfyn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gdxkizfgb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gabvdfafe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/geqxxusyv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/ggsvbrqeb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gqnerpkky.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gwoaksytf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gougaojmv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/grwhpzvqg.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/giaycpdcc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gmjgqrdhv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gxbybonht.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gurponhdo.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gqwiupydv.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gzfxexgrn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gfpdcvadl.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gfawpeeze.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gneaajtpe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guqtycizz.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gdqnyorxa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxqdebvhk.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gungcbcje.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gqgvrhigs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gvesjseam.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/ghbuvdumr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/ghelbzqrr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/ggmaargoo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gdmzprvny.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gwplxsvfm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gpuqbuevw.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/glgqonrkb.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gcwzosnxw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gpkgydxvu.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gshvmglco.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gmcrhdtxb.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gmvdfgoth.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/ggchgvskf.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gcyctcmlr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gfmpwccwc.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gnhonewmd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gskbodmha.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gvrkocdpd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gzelfuzls.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/glsfanemz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gnzaqmzhp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gikxuuzgy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/giayrpnyp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gxskvgezu.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/grycsuvqp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gawocyiim.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gydropxcc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gtmwndgav.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/glxofoebv.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ggboqzdpk.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gqishspai.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gajpezbnq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gdclezsdx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gyzuhwskr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gkvlfbcsh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/glqwmcdab.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gciaknooo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/glioelzen.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gsyrrukas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gezdmprvz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gtplrqbng.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gcrsvykkx.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gjuabjqvr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gbuadbzxr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gckicgsvf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gjuxqpmkc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwxbbdkjm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gtyiksuwj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gomupohbi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gkjiuqnmp.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gsekajpmc.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gmtkanyov.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gjghnstmd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/grhkogjsx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gemvumgbm.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gcutuzesh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/glpifzdrv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gzcnlajod.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/grzwwanga.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gcmgekufy.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gfvzgdbpd.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gomqbncok.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gufvorpwt.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/giwznbona.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gzxxbwsxe.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gbzlgtroc.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gdodxyfvq.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gqxrnuhsa.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gfjnirshp.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gjawylgzn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gjxoefkck.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/glmtlvyjz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gjszcxtyl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ggcnnedkp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gphnwjwnt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/grtzboqow.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gfzptrcuv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgxexnn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gxkvuxljt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/govvvrclv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gqbpzkhwo.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gymjrjssx.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gcmtanygh.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gzsjlewuw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gbmucxmai.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gioswpbdj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gnzheeuen.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gnwhrkplr.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gzqohevas.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gdjajevrh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdaazkent.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gzettevsm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/giggfvsyk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gwaagaqwl.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gadfbhxko.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gytawcosx.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gasbybsof.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gbcytumtr.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gdhtiqedu.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gvqxvslki.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gcmninamh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gvhdzgtex.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gcodxrdwj.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gldyoawfk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gdwpbdpek.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gtxffionw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gutztpcfj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gludfcwuy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkmyawiav.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gtnqwqhay.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/govioryfj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gnkufjunn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gmuspddqz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggrdvbciu.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gqyebgeyq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gukakaqnq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gyeqweayx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gwhkyduay.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gydqolbpr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/glxlosynj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gfobsoeqa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gjxaahgiu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gprikagmu.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gdstveagm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gkvdrrlaj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gimgucmcw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gnupoxwfs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gfrtmuodo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gzglftyvq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gelxavtbb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gudqtfmjx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gsnueylfw.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gcmliwesj.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/grdfzotdp.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gwrgqytfm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gekvatagg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/grpalvcde.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gqrzmfbof.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/glqhzdidb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gzkhukfsc.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/geafrkkyl.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gkcpsdemx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/ggwksbnys.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gumngukfi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ggaqbjklv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gbidppzmr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwswhlmem.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gehidlmid.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gdavjvjwb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/giojmvtvk.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gyxrkrfkw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gavoyqeds.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gjhofutvk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/grmomcgrm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gcdkonisa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ggpccqnhw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gmjuhacvb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/grjcmvgqf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gmaffmznt.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/ggjlpwoun.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gvocionwv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/ghmsovdhx.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gthyxzgpa.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gsrpoptvw.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/goirhpbvk.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gmpnbwwmc.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gcaqloasx.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gfixntrlc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gflrjhdye.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gjoodcdoo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/ggbxdalkq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gqsgufsbc.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gyjossdms.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ghvhkaxsq.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gpmtchglb.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gpdkhzgsj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gaawfmhke.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gwijbjjww.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gipwnbtuh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghufeybiw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjbgftcbg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gghrhwsvf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/glfoburdd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gmbwxiuld.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gtbjktvzq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gihxunzub.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gdjrqcqfd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gncrxjbli.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ghnhwitcj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/goyyvurnz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/glpjdlucy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gxwpyxprr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/grmlcbgdt.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gbgmueckr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gcsbpzpgt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gflehwggl.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gpwieoofd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzitwtxqo.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gwnuvbcyc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gjszotzhq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/garhrocrm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gsokuxnbx.sHtML


<!-- 参考信息 -->