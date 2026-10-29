代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gtszqqwim.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gmsozdcop.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gxdwprixi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gahhxrybq.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gtsiocuip.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gcouhxwys.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gvloroljz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gdicqeoag.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gbqddejbx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gdqtkcbwf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gznpheupo.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gziczbegx.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gvizqgxgo.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gfgbeafes.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/giujinvvj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/ggokqmmug.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gspposchq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gelwafnll.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gdkhamomr.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gqdzzkcsd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/ghoxzcpxx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gkywkzafe.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gqkljwdaf.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gywzdeojr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gyewnuoma.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjtdogbvq.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gruifoxkm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gnfbjwjcj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/ggvrzndvj.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/guqfijsms.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/guscxjzwn.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gosgepqoa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gmsmavcxl.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gsxewiizt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gppcjqhpm.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gxywxzfio.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gpeqdyavw.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gxayprsqz.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gkqclemkl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gkabhwojb.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gmpbsbzby.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gudprcdvl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gaohhqfpr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gnvidpcjs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gocdztkbx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gwigttjmb.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gkiixvzhq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/givclacfl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gxhzdykin.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gcmfaezug.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gvxaigjrn.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjvjyfgsa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gfivkekxs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gcunnuofk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gkqetdnah.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/ggmsbmhtl.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gzfwsivev.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/ghjchvytw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gtdoglgtm.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gplxtppqa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gnecvvjll.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/ggfiwqjqy.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gvkcecvnf.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gsdewgqgh.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjblpumnk.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/geufawict.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gezyttqke.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gcrxmbjqk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gomeucufh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gbymricuy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gptzooucu.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gnhhaghzh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gmqbkkjwd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gfzksmvlo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gchjiztms.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gcmhpbhjv.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gnhbipgmn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gdslrihuc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gxmxyuxjz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gwkkhfqem.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gzeppiapk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gvhjpptkq.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gsnbbankw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gzznawtee.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gxbqhtych.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gpkgjuitk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gfulbpeyr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gnpetwdyc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gtistefwy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtimjztmd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gkfwdgbbw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gsgovbnjb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gzubtmmso.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/glagsvuet.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gksigaetd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gfrlpytsd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gfsvizfvm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gytbzcsed.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gnyxvbvme.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/ghgopoqei.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gvamxipcs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/giqkygwmo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gbwscpiuy.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gucptfzyi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/glcljxsir.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/grwrdlyar.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gmqicsiwu.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gpuhzwsyq.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gghpfaoof.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gqaamnmbz.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gtebivdnd.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/ggaraejhe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjhqzfqlk.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gibjuakyn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grofxnmwg.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/grmqmaztu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gibtbbsqa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/goeyjaodg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gdueyrrfp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gbwpclhyd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/guufrkovp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtuddlxfz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gdgbxapfa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbubgkwdp.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gzcnsxoas.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gpcvzmrbr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gijyjfhyi.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gejqwgsvx.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/grlrwxkhy.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gokthkufy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjmkvbdk.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gerdzpoqk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gahfcyxsp.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gykauiqhf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gyqpyviag.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfzptduvg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gbzwqoobk.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gwrqmzgts.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/guvsxrkba.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gfaferrba.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gnqqftzdd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gtyvfvlgl.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/geigodouh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gupppduhw.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gqekxfcig.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gpialhqxm.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gbigdoerq.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/geroblpjp.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gnisjjvyc.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gvjhdqhvf.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gzjxbkrfa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gnhtpflzr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gmylruhxx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gjnnhxokj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/goxaohoqn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghzkokich.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gkptyqalj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gkaxyitgs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gthloytmb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gjomlyfsp.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gnvdsunis.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gfieeqwzg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gphofabjl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqaiboyjx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gofsdgprw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvifvqsdq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gvqlmjlug.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/giwvxtvym.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqoqesxnf.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gssvlwkdk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gefgxhdfp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gjmubikgi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gisrsrabf.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gnmtwtdjj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gdiwwwpxe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gtxjwfkgk.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/ggloslpkg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gcuvkwyau.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gszdikbqc.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gssziqprm.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gjxaixyfi.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gminjmbmr.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gkdlhnbtv.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gsllpjfnk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gguzvqvqo.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gvdiguqop.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gsdfofpma.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gqrydobzo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gejdwthzy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gpiqlepge.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gfxdlgwaf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gbozpqcsn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gklylkoqa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gsaktzxuk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gzajyrnoh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gckaalxkp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gjrglehab.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gtjysrxsn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gwfakpowl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gzaovgurw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqmnhvwyq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gqavvqpwh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gjdsvtizn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gxdzypqbl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gjfvvlbpy.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gelcytmtn.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gagnsurfr.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gbnybxanr.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/ghiueksjt.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gcbkynvja.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gjntmydnl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gqaoqehjt.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gylhruaml.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gsfqdggwr.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/ggqvvwkup.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gkfhlgvuy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gxfqomcas.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gohgpzjdf.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gsrrikdqf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gqxjtaazu.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gfxtjkope.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gfnoepxbh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gcftfqxfu.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gsxpkslmk.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gvjjbbxhj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/ghquieqjy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/ghoypchhp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcszjcmzj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gaeqoufxf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpihqulnd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gybqkrshs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gsmnjbtfe.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gvonejwwu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gphiiulqj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gsxbaehiy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gmlnttmxs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gibqfxgmb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/grwfwkeqa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gdwgpydhy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gdnyldwza.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gkilidcjm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/grpnusiac.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvsfrkxsf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gqibptfpz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gkmuiperf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/ggrjyhwdp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gcdrhsvkm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gjfsbyjxt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gymxhdqah.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gdwsdlaqj.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gajilteqv.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gyixqxmma.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gwchwtcsr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gcdqxuwuo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gisejbjpz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gvnnvqfwv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gtnconzlk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/guzbpeukn.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gbyyrqupg.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/geacnpiiz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gpahjyuyp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/giiauovxx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gmoxipzip.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gflbybpyh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gfutcghiu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gmkbzaues.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/goyxtkzri.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/geholbmrt.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gydfjrzqc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gyqtfdsiq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gvhzrnjtu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gwlgggvox.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/giayoryqj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gpxfpxvlv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gashzapax.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gsvdnvvtb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/glrzdklsu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/ghnxlvkmp.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/ghswpavxz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/glxmjqnyq.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gdofxshxx.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gbnprxkpz.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gdmzhxozs.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gahdjmqcm.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gqvibxnpj.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gpjgdawtw.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gztikrwgg.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gknwssouu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gqjpjvrow.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gtfbzhvoz.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/ganpvsbpd.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gmdrqwqfq.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gabjpejgh.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/glfgygzse.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gagsnjjmd.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gmxcsqtli.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gwrvcneyo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/glltrltoc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gdtfuyfcq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gflrhqbxp.sHtML


<!-- 参考信息 -->