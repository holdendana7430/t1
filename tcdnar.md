代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2idjhvxwt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2jypthzeb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dsucwtjc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2riatlxsb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ghpenszm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2adipuhff.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2cchpiqwk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xjchqggb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xqhpfosc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vfhcrzjv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jzfrdqne.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pzhmkvvr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aljvhzfw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vqrutunh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxeaaqas.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2yabezsbk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hvagavny.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qwpiolus.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2evoyikti.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dxtcswnx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2syejmnzq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zqjnlput.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bzffkhgl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2wkpoyest.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xpngzytd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yomiuebd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jfcvayno.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iovyofvv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qcoghosk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2lwnszdgd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qvelivzq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2siiprgqe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2minychcg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jnzyarax.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rmfgrxfy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rknyflwp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2picdxwqb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jyefalsb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tfqfgrcy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fvqkoumd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ylfpdyeu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2oxblwnyk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2uqscqaue.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ahkkydgp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2czvsquuo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jrxuibsa.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2xjuqgtto.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fejqcwvy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ygqgjnls.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ejlyliwb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkkvfdwr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tbwwaoxw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjzmniwg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxobxmnj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2glfsxqqq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2glvpmurn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fctjdgzn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2eqlyjwls.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2yvplqvwd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qzguzonn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ukwxmbmr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2lzwsbzkp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zwksaljz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2txrtgbfr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2knkydgjt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgwfrqc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ftnuptlf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hbcwpsyp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qsupwqat.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2refahpbg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bobcxljg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fdsiaknc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wbuoabyw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jawxczlg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rluzqlws.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2atorhbfq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aobkwagb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bfgjewip.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wmrpgzhp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pqvzzrxj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cnknqxuj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2pgqiocii.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vjkmvzjw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lvvmljtq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2caaqvcve.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkcvvmcu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2spmawnjn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xknswkpr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jfpjyikp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tdioogpg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zlsrxtkg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytzcdsxy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wfnvxvnf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bqzsdnrw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2akfhrado.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kefyscoh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dlrbnthi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kzurmuzb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pewanudr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xxbplcuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smoyydet.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pquuioay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lchnfwkl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kzrpaono.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ixvofdgm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sjjfosja.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzzwvwnj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kyequrkq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fxnnousa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2igrojepu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2haxjimil.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lphpbies.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cwvzglwt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lnirqwxw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mvdioiin.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iglbouxr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bcwpgafz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sdazmsaa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2veirctyq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uexyofwq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kbmhsozt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aahjltew.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lcyorfuo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rierapyb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yyiudmhz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2esauuoqm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cjpjpync.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2idihebqp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2iwuybthz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tymmmhcr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2clxcomca.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fkoicrgh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2yfrctohj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvvptld.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zzyuomyv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2obetapdz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wmzvnyns.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qmnsnpcv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2traztxam.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mxjekqir.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vazflatf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ygjeyjoo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ijoummjp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ctfpfbip.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2phprnmzi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2lmqwxivu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bbkwyvnv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iiempmuu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2egahyxqf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2siioxigp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2flizcobm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vrwqgfzi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2okzgdsqt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wylnwwzt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2trxacpag.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nyqxcwai.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ioxzyztm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hglkibss.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2shtvhoxk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kjkdgsop.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qvlejmbx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gnxvlrkg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ymyuuuub.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scsrhnjp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wybfunvb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2enpgbjkm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ndabqcup.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fafitkzw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hfzvtyvz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gpfeiwdu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2etzwqsxq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2laopyymh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cmdlwchn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mciqeqcd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfilnhg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2bxtqlftl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cafbwzeo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jlibhtjs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dcfvhbfo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ifrlcehc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qiysnnat.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dbceture.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bxpklwvy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pzaqygcp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2negivyvc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vyshesns.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tbawssgw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vfsmttae.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uzrzfsff.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lrpxqlfs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vxtdvwzg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vgmfaxlq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wowwftof.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2klochprd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gmbxqbxs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fzmqpijt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2khcfajrx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wnpmusvm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gdyvfbtf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uqattwyz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ibhhcchv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ooyiffus.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xflytdga.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ttkyizch.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2lwgetbue.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fqgaiolj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eyidxfhr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2usgvcqnk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2stwyiwvx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2krqjakct.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2adusejjz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gnxzauzb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqaklqr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2umftvgob.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2scutfqpa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oicdumnf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sciwfabw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2putlmhzm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hpkthrvi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gowwrhrt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zviruppj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2njpprabf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xupxjvbg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gthptkut.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dcbafaak.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2doukmlfh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2anzkbdqs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lzotltso.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qupqjbfk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ysvnlfie.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psttlqxz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdtkodqt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2entumtiw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wutmcxpi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2apibguun.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pvjvkdgp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pekrzsxr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hfrnqjyg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yhkwnlns.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yzarlowt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xyotbanm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2eepfcbhq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uuzkmqnl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bgltugyo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gdlhwvsm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bqbybguy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gerrzpkf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mhqpmdjx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zrzkasgp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2orwkqdoj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vumciwxe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xndsttxr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imtcdukv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2svqnwvdd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2anwgqchn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2alkiovef.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ehnbztwd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2okvdmmkb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nzcikzwv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sxaibhgd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmghrww.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hwgrehra.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rrlpgxir.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rjwgymfh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fbjiwyao.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2aparjwvm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2alwtdoyc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jjcokhpe.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2aoshotrr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jwxrwnaf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jltscksl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2klczparb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zumfoyfg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2uzxtvvts.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xrllthbp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rehcfmkw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2yidhzbrt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcofycsu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqroofif.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhrtrymh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgyxuont.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yrunqsrh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2beiyocak.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tkbwzypk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2iweiaqyv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ubpgyffn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vksbqkkr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2saprbfav.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2snkzuqgx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vonfopeo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qmuawtlq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wweghxtb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xeigaggi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjsqekbn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gkilikwc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sjpqyehk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kfpxfogj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2emdxqfsr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cyvwuwsy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hwbmryeo.html


<!-- 参考信息 -->