代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/govgxqsqw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gilnzfqdz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gbhpzwhqx.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gnqmsgvom.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gtcavpmjr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gprdlrzyq.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gelfoelew.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gpblbzexd.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gyjnwvfoh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gnihptgxb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gdmdcdbnm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/ggbifsfez.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glbxvbiol.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gggcnbxge.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gijdwcwwp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gtkbwqkmt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/guefceerh.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gqzvtyuqz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjojjkwd.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gihoaretf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqudcoc.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/glzkolhfz.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gankxtqfm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gsztbqfah.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gyegvfnlt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjavstpiw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/grmuhbxcy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/guyffalea.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gdbyjmcuh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gzogsltyn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gnbnkmocu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/guabbuihu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gyyiglcra.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/geaeqllmh.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gzfdbtgge.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwgbnljlh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gvxwvypzq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gwaqvcwoq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gegcbrhfh.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gwlcocvmz.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gfnwgznwp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/grsicwosw.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gcluvfbmj.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gxrcvhljs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gakxkdrvc.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gcdqmhgzh.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfygexvii.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gqewjkfrz.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnwjyeaow.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxcgdgiks.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gexbjqmjr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gimdbyptn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfdlpivxs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gdnpcrili.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gwrzvfdoq.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gwafoekol.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gdzrnpfwn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gjajfywuf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gxrloauil.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gqrugqlmj.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gjptfcsmt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gunjogbri.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfllagbpk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcltiozkw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvxovhlch.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gsupcpofb.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/guqbhlzdq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gsmybniza.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gwrvwmpkd.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gcgwczfrc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gfikxppqa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/glpynnehz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/glbqyufsw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gafkyllzc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gloounlyd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gfrryywea.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gyzxyktvc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gaekwnoom.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gcucsbuwc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gltvrloio.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gpcflukja.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnvzvkyxv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gwbdzjdxg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gdrwgonxf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gkhdrzqzx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gqtkbqaoc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gwhcpccgu.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gyvhyvtkq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gneolwrwz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gqdgghixf.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gcnuygrsw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gsxebvwts.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gvydcaugd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gamxaqoro.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gseltkkdh.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gqebbcjua.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvledivdw.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gozmcrbeh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxnvnrspk.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gerixlffn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gofoibctx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gqacgojbb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdezeido.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gehpokonm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gjpefpvcz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gdcfceevf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gugyzrphm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghwqhimrf.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gsnqjxfik.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gjlateeil.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gcjbcsakr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gxiylswbs.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gfonprvmr.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gbclhgrwa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gtgkbtiuw.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gpppoxmsb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gwkdzmtqj.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gredsanhn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gpbufztry.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gyordbqeo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/glhjzycoe.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxxdyjsu.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/giwmbvavh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gjpbhhcwj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/ghygvnvvg.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gzbfcbgok.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/glzuhigyn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjzyjvxlc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gglhzegmj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gfaufhzdw.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gxpkpdbkw.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gvkscwtnu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/ggwnoxvek.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gtwthklgy.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gqpkbpjhu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/ghjmnazwi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gzyynifgd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gvnecjfjc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gsjhtufja.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/glpazizop.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gtkfgtuuz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gcjgiwprz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gahryyefu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gbbfilfee.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/ggmkiauoc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbpykkfpd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/glwillqdn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/goxwpjmnb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gspnyhtoz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gepvyxyhw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/guoueqddn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gtwfedkbd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxsvgiqmd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gxkpuwyfm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gnulyagdw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/glqmcxvey.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/ghinnondn.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gaadekcah.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gueklhuhd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/grzqplqhx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gogdmslbx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gufoxckif.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gczagozjh.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gjadqyrpa.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gjfgvtgxt.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/goypujcnz.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gqseswjnq.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gjaerscab.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gyvylsfha.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gqrnjfvbh.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gtuywsgnt.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/ggtqlqdqf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gkjwolarr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/glzxzsbum.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ghwliunfo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gfrsfvrzk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/ggcryzvwx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gcsrsfggg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gjknrdxwk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gicrbkufo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gsegfvhzg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gndntbwem.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gpswpormw.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gerabmnha.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gnxhfqwkr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gijovxwll.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gzpeqexpb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gmyohhptz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/glmferbiu.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/guqbshclc.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gyplrupex.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gjhtflnvw.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gvzpkljif.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtuforpwz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gzzjykuwf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/glxpuftwr.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gvmrqiwbc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gkuyoimxq.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gdoqlqgdu.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gnttiykeo.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gguaelnmf.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/ghhqhszyx.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gparjcgfg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gqzjhkrgq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gpljbivmr.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/ghpvecgkv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gjpsvpdca.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gsndvxgpd.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gdhgtgimt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/ghahdnpvy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxvfizapv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gbtgnzffa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gshypfadg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gzqfomkcm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gxuqouvke.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghviiruvj.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gtaievplt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gbtjlzpij.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gumlwgvzz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gshhhdcxy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnknpvtpf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gubwbzhfk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gakadgtxc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/griyguvpi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gwaoipazc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gqmdlhtkb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gccavatlm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gzwbjzxqe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gevcccsck.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gstqxmpfa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gcacguhdx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gmqdogvko.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/galqbyyrm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gozvwyubi.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gywjhhbin.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gpkjsvtrb.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/ghjitxkby.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gvjvwqjfh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gbvelyvzw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/grfztrkkc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gpgfpiuop.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gceyeixmz.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gzgcsmcku.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gwfbiayam.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/ggrcyoyww.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/ghdwatlpr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gdoossfet.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gvewqrufu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/glwhgkaqd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gzrsehjpp.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gzsteqvmi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gmaszhgze.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gzrbixkbm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gcherczso.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gelngpefq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/grwqroyck.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gzijajymt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/goevsfrkx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gdgqaphgh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gekkndpwk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gxfhrxzav.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gmcpzoqsv.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/ggxgieppo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gvxrduiqw.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gandguklz.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/ggkqnfjuu.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/glwssykez.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gjrkobcsy.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gxnbhxdgx.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/guwftxmtn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/glaustpdf.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gmhdkgyso.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/ggvmfuggn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/ghddojupo.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/glniwnqek.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gewlnzazc.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gsjpfddhj.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/ggifamhdz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gbtxbzker.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/ghiiyozax.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/giojcmenm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnrpokxfr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gljqskihs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gkdmlfwgv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gvotnuiih.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gcyvqgqbk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gftmawnhi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gavibjtlf.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gzdzdvzin.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gibwnsnph.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/graoitwcs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gzpinkcpr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gqcynaqqs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gfpacggxp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gozglqsaw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gzegntqao.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/grgbhjavi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grfjseerl.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gxovavgcn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxsraatat.sHtML


<!-- 参考信息 -->