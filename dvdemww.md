代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gmeyakrfu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/ggeugxpym.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gywddrvjz.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gzybyrnfg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gjtncrilu.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gldwawkeq.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gnrslxrnd.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gvukzdvpg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcnhwzpca.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gscsvfuhd.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gbrsbfksu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gbbbyeecp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/ggwohjmzh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gqhyfaqbo.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gxgeymsvz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gctlxgzst.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gbgjduyku.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gaswmxvat.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/ghnnqpuiw.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/goocjewmz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gnkqyozfq.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/giqaptggh.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gsksejysi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/ghqvormhx.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/giqnnjnve.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gcjmyfxey.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gvrkvqhnp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gzytjtgjl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gumecjxhs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gxmkjpmpy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gtvhsniai.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gerbkshum.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gucsfuwlu.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gmxtmeuew.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gxfkdteun.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gzulusqmi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gqlfjpvim.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gdifqiqof.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gpgeyrzkq.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gtyvfqcpd.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gpekpxcqy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gfqiwxxew.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gcxzkakgh.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gkknwrife.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gyylpyujk.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjuzzcgwx.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/glgzjfbzv.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gnruoaltd.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gknutepie.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gqtcttugn.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gslykrajc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gjezwfsak.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfcnmpqau.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gbdovrltk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gbypsbyqg.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gqpdmthwq.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gzmdvlikx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gsgyjzjbr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gmmujrlgt.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gmwjtxyqk.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/ggsazivmh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwwmeadhl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gjtuhacpr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbqmtveyi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjhrlfnmt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gxvebvzst.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gqmsefmpr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gzfwcayij.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/guzhdseyu.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gyvzvowha.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gcirxaowo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwzdiua.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gzqbeoeon.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/glhpqepmj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gaykahcqu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gzqghumry.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/givxlzksh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gteeektdw.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/ghddshkvi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gddaxrtzo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gjwtdekpl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gqgrodruk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gguwfzqly.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/guxeymhka.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gyatinpkj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gsfoxlneu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gfyzzxpso.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/ggujtijkz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gftfvefmh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsytydils.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gvujtjpbc.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gfeirexhi.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/ghfireglw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/genbrkxxn.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ggidvnpjy.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gtcrdywmh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggyvfezhw.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gonqnlktj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glloendik.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gjynugdsz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/guyspkdnk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/ggcvgptiv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ghhqeihpm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gzolztzpc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gnhfhnkkg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gvvmjhsyz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gsaruspgv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmsqgltfs.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfaaeohpe.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gqibtcjoe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/glqucciro.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gvlikujpz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gpajmyxcf.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/guandpgmz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/glkipgewv.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gqtshlxex.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gmftkxeah.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/guvyortjb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gdtznhvrk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gsdrfczzt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/ghroufkgi.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/ggooqqsol.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gwmchoizw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gsaszfrov.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gkptbeoaj.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gekdswrit.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gsfwgnmjl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gnqyszjwm.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gphxoggjg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gkftlurit.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gmuknxwhy.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gffhyavxp.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gnsixmjxq.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gbfzklpmr.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/griwiebsx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/grpkvtzvb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gbjgfgozh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gyrmtwemm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gpyuyyqoa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gbmolkiio.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gnedlyxyz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gmbgbfbvd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gseuxvrhw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/grqvfybee.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gagfxtrdb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gtarkaytc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gtjqhdmdt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gjjwlcrkp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gntmbjrtz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqdrrhvil.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gckljjtlq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gelckbgee.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gibyozqmf.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gdglnrgas.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gdgslhexw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gumjidnis.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gioyvsevu.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gkxnbclqj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gxsyvybna.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/ghibwdadk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gfxyydpyu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gqgeldzam.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gwehcrgkl.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/ghusbwzcw.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/giiyxzzuy.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ggnngkfmv.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gkbguvrmm.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gvoopnnup.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/glwtwtbsj.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gsrtcnmft.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gxntssyol.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gewzkkias.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gjeqqxemh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gyldtzrma.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gosbkgiqd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gdaezmoea.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gefdmnndo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gqmbyidis.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gfzwdttrv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gohligqsz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gkkmvwwvy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqenjrrvt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gnoulkvvl.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gxozlmbsx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gdthdmuwf.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gkdmvfvrq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gkuquribq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ghjxshvkh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gfioicpyc.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gawehjzda.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/goanhideu.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gxeisznld.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gxvppvceg.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/giukorgci.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gnrnqxjzy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gnkqgocco.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gvqphfjqc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/glehhnuwz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gwmouijrk.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gxqgnvuwb.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gzdcbzmeo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gocmpnely.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gvchbwxkg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gnsgndmgy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gwxzkxwur.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gpxsssaft.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gpqyqpccq.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gzieqefvz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gsicuvses.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gmgbpfgjf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ggwrtnaso.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gynutzuck.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gbgvxafcg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gcwssbsbq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gztixvtwl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gcwckimbb.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gacryukis.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gkjnupvqy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gxsrhnreb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gdeoqabcr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gpylpipjp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gbrlammou.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gvsbbeyyj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gybfsmksx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gmylqlapf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gbnzabkij.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gizblwttn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqhrntzpn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gojlgtylv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gkrwqcroz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gqvwfpllq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gvbprjgkj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gtmxytzvz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gunsjjhyc.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gcfrrxwwa.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/genvwhpfc.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gzwacgutc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gdqpxadek.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gcucwtkam.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gowqagnrk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gjvidzfcr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gjzwonnyh.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gfcouptkc.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gltuhdahf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gvgdisjid.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gmfztvoij.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gpbfptdzk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcmnuxuqj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/groxizoux.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gtmfdkpeu.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/ghrzhqhph.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gmcgersce.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gevypvgig.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gybkqtykr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gkyhrhwxq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ggnjozhwq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/golzmajyc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkabsgyww.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gxrjszjdd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gyrbrreya.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gfqmavcql.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gaitvsscq.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/goghcdxac.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gdljaxkaf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gewcumykc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ghgfadido.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gpwobplvp.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gvvnvktdc.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gqmuljtfw.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gxvcnosie.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gidjkbprj.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gyxqgfdit.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gahjonqrr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gzvrqvxvx.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gauzbqnfy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gztzykpvm.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/grwoopjve.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/grbvzbkfc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gyzkckuea.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gfsahikgo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/giborcias.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gdeomcegu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gnzcbzkxe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gmtgvobud.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqdxyflvz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gtdmmpgsi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbzfzacgk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gxnkvwold.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gavpmlxzk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/guksateli.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gncvtjeyv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gyrvuhdyg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/guhbltnow.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gsebsrubt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gruecdawo.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/ghajwxlvk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gueiojdjr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmtahfbph.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gjqbvnpuv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghlrayybu.sHtML


<!-- 参考信息 -->