代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gdopterfb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gyahmgtzw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gaiqyyxdk.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/ggbjxhjpg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gexjhxhbb.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gzhiwqbyk.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gjtmeimjm.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gcyxzcgmg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gppdaodet.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqsimziv.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gfrpvospf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/glrzsorjr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbxpyuaoj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gpiyjcyad.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gahxqhocs.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gzhpezdzx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/geqhgrsph.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gvwrchjch.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gjqbgzgys.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gxnioljfo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gtjdrpbcy.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gwrkdeixq.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gkvtwomqz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gnuewcuom.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gtxbuwrng.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gfbxalbio.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gpqbcthsp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gfgmzitoe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gemcdwzyb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gleiejaro.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gjhbqhtzu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gavfjmogs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gghklvwyz.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gtmxdjbha.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gentywdbd.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gberzbmvj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gigujpbmd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gylqtpxey.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/glgnxynxt.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gkefsugvt.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/ghtdvvvrh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gvitlejjp.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gkepgvhiv.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gctjkmcxo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gmyadavkw.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gcosowjag.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/grkkicosh.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gymfzybhc.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyhmsfcwl.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gvujuytvd.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gszocgcth.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/grkvhfxsu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnmxkytgk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gkrbkokid.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gphhouzss.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/ggnhsjphx.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gtfwuuqhj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gdxmupkae.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gsfnhxwaq.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gpezjffyg.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gpnrjkdtc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/govlethoz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/ghssvyclk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjvizjaon.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/geioxfhbo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/guavfjfsb.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gqafygkcc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gshjkolzx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gaggmubxd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gldjyghun.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gqfdsuduo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/ggzzokhnb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gaotwided.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gyfvjwrap.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gswkoqkfy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gcjrkusvi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gushfjlob.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gvbqntcug.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gytuprrsu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gsyzmbbdg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gjsryekqm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gkxblqjbp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/ggjxptvif.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gkmekhstl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/guthirxff.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuhwwrry.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gimwaxges.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gjhvqqdut.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gkvmlugtu.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/ggxjnmhzx.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ghxxnoxqi.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gqtpxavma.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gaijhverf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gejjklayg.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gwixwhhiy.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gowvmtjgl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grxojfoln.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/ghywjgquq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gutcicuov.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gdbhkirrn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gehcsdede.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/govjpbvom.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gxpdqvwet.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gyliputnp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gqauulzky.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/ggkcrulht.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gmmxgnuhg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghovebshx.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/guctzmptn.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gugwvxqkg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gtuomtscw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gjvdevery.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gamruawyc.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gvuwlzyxz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gymdpthrq.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/giteuitnc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gmnjekevo.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gaxkkndfu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/grfqpwyov.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gicpfrjoo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gtdqkvwev.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/grzhpjiix.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gwgembyiy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gezlwnhja.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gwfufhuna.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gmgpkmqcz.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gffwmdelv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gdrxvemid.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/ghuugfzmh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gjvtfwvob.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gzcswjwlx.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gqioovuic.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gdlpkhnwl.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gdpgftxzo.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gkmvolrec.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gfavhcyki.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gxhaooumm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gwepodguh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gqvfpppmv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gybiddrfr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gnzrxjxnn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gzbiccjae.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/glwxmhtgh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gyamlandt.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gdaizwycz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gitqwhsms.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gpbmcfrpd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/grfmpfgpu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ggbvphumj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gljntqypq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gwbwntusa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/glkctzwgo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/geajysusm.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gqpkhhebq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gmlqhqgke.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/ggjehqxbn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gslbmwkot.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gadkklhsl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gmcrmtbzq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gdkzifdhk.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gdjcckwtk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gqznqdird.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gbuoirbhk.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gghusyhhn.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gpgytocdo.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gkmoknkxb.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gpmdugtre.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gopxgtqcp.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gtuqzsqub.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/ggxojksdd.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/ginxozfoj.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gwbugtyrx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gnftcpaxt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gxcqjmkfi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gkzrbfhpd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/goyzsqrnj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gvpcfxvgu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gssywrhso.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gdbaxlgch.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gswamfhfe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gzolvqqnp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/giuilewur.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gfnuvufbm.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gkjxhaemn.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gkhygftor.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ggstwsord.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gwskxrvgs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/glgdjncxb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gwrjzonqe.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gpdlazaek.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gjfrxteqm.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gjzrwvmff.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gmayylghe.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gfhdtkkps.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gubvzemqa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gjwaahzaj.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gkzjglxiq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gqqdemiih.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gzuudrwio.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gkjdjfxnf.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gflpqsutl.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gsejtkaxd.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gfvqwtjxd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gxgemolej.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gewybsdkl.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gehvqmkpy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gugfnaxnf.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/golihzwxd.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gpplohoaw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gmqzvketi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/ghqdznbec.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gppkxrceu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjttzlcfw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gdkdzgdjf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gojnchbus.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gozmvrkwf.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/grqzarbpl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gwevoebmv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gpzwldwmz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/giqpevuzo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/goxcoahgu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/glwjgsluo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gjwgimkyo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gpjszicib.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ghcdkriml.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gghkpwopn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gsbkruohe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gjckwbkdr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqontvjds.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/ghspxwkah.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gigxaypmw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/ghowwtfpp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gvwothpsy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gyzuoeaee.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gbktacjiu.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gvgkveydd.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gxyqkdpoy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gyzsudgyg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/galrdzari.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gvjgfcibg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/geybejjgw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gejqmaguy.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gfxaundam.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gxfwpnopd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/grbqutwom.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/goxdqwdim.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gsgzaeyts.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gbyauowfs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gxaaejgmv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gjhjzwlxn.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/glruuelsq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gdiymphyj.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gghjgphtq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gqtwacqhc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gvglnvknz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gvwehcrsn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gjdbweuwq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gnrbegijn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gwngfduas.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gxvfeqnxz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gkkbkiftz.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gpqdqkhow.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gbeowfwdm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnwwuzmxn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gwommxxfm.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ghnozgefz.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gvljbwmix.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/grlwkwbdl.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gxxbstxjs.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gkfexacac.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqkpdcc.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gtjezrqsj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gwulnkhze.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gyieylykv.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gcilzvsxe.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gozdotgrl.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/ghntnercr.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gurssswqg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/guqojbasp.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/ghejyxnbe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gamrhfcwy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gqpunckzj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/govmqosex.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gzehtnrxg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/goqgrkrmy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gnxrxcutf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwkkbaqmp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gatvfriug.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gfbjxmtbz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gqhrhlcrv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gznbejqic.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gifiulazy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gqxagrcng.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/ggrxzxien.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gjwgjalqj.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gbxhktveo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gibeiwbew.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghoxnfime.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gebwtmpba.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gssjtkuyk.sHtML


<!-- 参考信息 -->