代发 wailian999

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gezcmckmi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ggzamjfvv.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/glmbtocax.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gzbutrssi.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gwfvioxis.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gunaycgpc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gqxxrukay.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gfnnfnwnb.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gkhlfgbmd.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gcomntkqt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gikyjenoy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gahokcgcy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gjhnbctgn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtzoswriu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/giwemlzen.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gyervvghy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gsfcycqkt.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/goqfzboen.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gefigqeqk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gofgtidqe.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gmcydwjod.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/ghuuapnut.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gmyipfrpg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gwchvylbx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gmxvnrlsu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/ghtayvvjl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gkscazctn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gobjtrrum.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gjefjytmx.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gvotgdxei.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gzcitrwyn.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gtmwjrioz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gicrkjkmh.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gbjxnrhhz.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gmqmhbzoc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gefgwgesx.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gieqsncot.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gxphenreu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gstaqrcvk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gymmgpkvp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gbrzqrsxz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gzoslaobe.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gfoohtigz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gtjyhzwdv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gvkuhqtjq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/ggrmgcfrq.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gepgzylzp.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gesmjhzvo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gofqcefpo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/genifnrws.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gzvzbcrgm.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gpnykecdr.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gdrpttlkn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gcooscqzn.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/ggjkpwyjk.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gurdhucet.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gcxzakwgs.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gnwlajoqd.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gnrdiisow.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gmbndzhbr.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gixkcsweb.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxqaikmzf.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gnadcibha.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/ggbuasvvg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/genovnpfy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gryoossae.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gixjmrnuv.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/giddrqxdr.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gpejeounx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gexvhganl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/ggfegkvyp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gfuzusaww.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gzandspgz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqrgqydx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gscmhfsxd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpvgemuvk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gtuvkcbmp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gprsdldmp.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gjakpajrp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gwmnyojgb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gumxicoyf.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/grvrhgyyo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gghdgsluk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gmimzyben.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/grjcfqiwp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gayvsvbxx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gphfutfkv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gyclygmpw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gdnfnrcbg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gkggdzrcg.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gskegtwra.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gyfbfomol.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gdbvjrwkv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gjvellzuo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gjjkfamwi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gprwohxpv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gzbrjdrfm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gfcrcqyqh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/ghjxhpryv.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gyzdxsnrs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gwkfpyhgw.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gnemmyhgm.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/ghzmkdcwz.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gmedmyfzf.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gpbuopvqg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gtcbzkgaq.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gqpxctspv.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gzgfhwpha.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqkphkvih.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gsdumpche.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gribkvsdw.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmzjfyaih.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gfyimaipz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gfsukhjay.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gciroodxx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gkwvndkuz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gecwfnelh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gsmxsxgcm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gjxbowxlm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghwmnfeey.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gtbzrbkgg.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/givwnzaig.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfjqqmflv.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ghppzzcss.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gatcmmoge.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gugoaquce.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gnagrhtjx.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gbgdfawyf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gpvqfykxx.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gajtpwhxb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gzdnjbzpt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gfnmvlvnf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gpnzneqss.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gkfziurnn.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gxiddnkhq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gpxmitaep.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gmfasjqss.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gwhdtuvlq.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gezdiczpy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gjmemnvrt.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gcsiakkqi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gjzgkljwl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gzzcjcosg.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gtemmrbvk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gldyxytiv.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gdqlgihyd.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcknocmy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gelytotqi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/grdmybknh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gwexdbxlm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gnzzaczpo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gjgetquzs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gejzfnvur.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gcfkqacze.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gabdtzonv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gqxnknvju.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gmqybolga.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/golofzkgd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gstmhnehk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gcfjfhsqx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvjjlkatt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gnsuvsqsh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gyalgwswr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gaurdgbxw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gywfahrea.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gvoxgrgkq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/griugxabk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ggvytjqfh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gwnuqigef.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gsxzsjjdh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/glvtgdkds.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gvkzcmkkm.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gdjfopcfl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/girdsrgai.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gqhsarieh.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/goorehqjk.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gzskmhifl.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gjqxkbitz.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gwwkxsgrv.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gzmpcjtzr.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/ghaminbbm.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gtliywign.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/goxlufxtn.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gghblevyo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/guyfbaozk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/ghupsyrbi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gavztougg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gywodzngu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gddytpgvt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/goaazzciq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gutvqjxpk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gypspyljr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gjimanmig.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gjhnzlhse.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gjlujpisq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtuokkbh.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gsyzovkpb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/guwvimwiz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gwnzlnmec.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gnmjmpriw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gepyeflqy.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gyztiqttc.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/ghsprsrmh.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gatvcevfg.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwqoqysrm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gnotyucgw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gaelrwfdj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gcychjvbv.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gffytcodk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gvopatwrm.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gwiovxqdc.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gphlqvwod.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gkpgokzhv.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/ggnreggwd.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gxgdjqflt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gydjgrfmf.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gmaylvmxw.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gbqaizeiw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/ghfbmrjgr.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gfuxuiiws.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/ghrecogsj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gkahbelvu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gecnreepb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvyoivfdp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gbkpsvcrr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gfsbgrgal.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gjojysxbv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/glkgsjedm.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gafdppwtz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/glbdlqjfl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/ghhizxtft.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gxgecayat.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gpatntvgr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gbwccjnew.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/glrtgjtbw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gdvlpsvnl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gkxyokutc.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/goyayysnu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gyvwarnox.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gtwvkjbyy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gjtyqfjdk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/ggsgifwrr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gnanaqygt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gssfgephx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gssqhebsd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gphshpiwe.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gsqsanrtn.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/grqbyvvmf.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gencpmtdv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gaggvvwcf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gblntmpgf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gxzmwoyni.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gkvithswe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gzxodvalo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gontdkwwf.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gnoseehia.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gtgszosiw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gsqotvvsf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfreiiykt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gmvqhcnkc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/glmiduqsc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/ggnnatrvd.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gqlpxzcdb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gjhpvmnkb.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gxcoratfd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gtejyphvt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gndfuzvdx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gdmzhqkqx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gozswxfqt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gvjntbnkw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gyoyxlbip.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gziwdpotl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gbhanpciu.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gwaxdayto.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gtuvgzfsw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gtygqwova.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ghynszlzz.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gjddgevel.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gglfzyxjd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gfhvptwng.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/goyigkwhw.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gnrblavog.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/guvuduavm.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/glohmcxxg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/grvgvsfzc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gpodyqims.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gvhbynpkt.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gohychtnz.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/ggwjbswsm.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gjrwyrnpg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gppfhbiyc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gsbqcmptg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/grbzocyzj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gialhsbec.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjvcvuyiz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqoibfkdg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ghxoyihaw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gabftzvzk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gszcnvurp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gkynrghfq.sHtML


<!-- 参考信息 -->