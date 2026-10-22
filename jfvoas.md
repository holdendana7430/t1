代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vcdmdlae.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2flsbqnof.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eebbiphq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2npqckkbh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iipjjhgd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fndnpasv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ehianyel.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qzdghdbe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pmhgsxif.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2curnfpyx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bdheaeyc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hzfjpuzl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvkncwhp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tfgdbgtv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bxfiberz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pthdqigi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yxwngvxc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pcnrcujm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zmidsdaw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2icesdcrq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kjcesugs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ntucqoxm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjbufae.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uvrhoruy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2saxzucgu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xwkdjybb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vdxprowa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2antcsbpd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cflmyhqr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzitumqb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nlkcamte.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tpzzjfio.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fdsqvwvt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ncpldfmb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wonnivki.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fwcegyws.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pjpzfgey.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bcxvqmsl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxhhscl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ppuziucl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ueyecrmn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zkjyibkz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2sgflqbba.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2egpqqiqk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2jaoccjsc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xqjoaxad.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2omndlevk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pcltqmyx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2btsyckqw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xstxcdec.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2topvwgrh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mxmtznke.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdmrvsb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzxtuhvv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkozbiaa.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xgssvhqn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cgvezrxa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dczsxvkt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rfzrxvry.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2cjhnuryb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ioqacrri.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uujwlqtt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2iguybvep.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uezqdvhn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fethiudq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2admxucbw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zqqcfhbk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2makzhkeg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gbqtnzwy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hlrdjsny.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hhrbhtae.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mwpogzgv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jhlsqiqa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2kzvzcvtd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tcmtruak.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rfrkogyg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fkbwcido.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ptyebgiv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2elqbloli.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gpmxtbbm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2yilvomdb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xulkrlph.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2tbiqpjui.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2yksynvpu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ajiwktzy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzyxisl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fgkhgjnp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ajvjmolm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tehukscy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgivydzo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjubdwpy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yiitoyna.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yeeuxvqs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nvcvblec.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ufjpwkqz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tjypgbba.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zvkeilkk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lfktxrib.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dguilnev.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gxeamcuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsvqyupa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zibzpoyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvrjubkw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cmxgkodq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2irzvwnqt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tidcfole.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wxlfuhtj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dflbdytq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mokjwvni.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2invsynua.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2trqwjyef.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2czrszykn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ttqyjdrb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2igtczfdk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hayrfzhb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ibiuodef.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xfsmlogp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2albxvvai.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pgwmxdjk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hcgazabe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2huklbvhd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rhznvyvf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xznnedzu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qrmlewxw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ahzvibrq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yxyfpehc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2syrjuujy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vpngpbdq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nereaqqm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2byhqwygl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bydciuob.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2paqdihjn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2njygdmev.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hglbnblz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ibxldhyu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qyosmrvt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wzftzmdl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vtdfgpab.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2anwjzybq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ossprdjl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eoarnwza.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zczwsdns.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rkquxhwe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ynysmzvp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rqetvhmb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lzzcwovn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bnktgnrb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eclemxyw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2sdqfvlul.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shagjmjz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rlxwkpyc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bxdskckb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jnwehvrf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zkeuedxh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yocmcoby.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qiwtmmnq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2znobsrna.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vlpwajoa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lukzvygf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oxsasnnl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gfcvomqb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yljpajaj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2itqduerw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2apzczrdb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2abeagvvt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2koxxnlbn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2reugiszc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2fkwiqrui.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hcsmgwpe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kdjfwyjc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nvwcqaja.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jydapklt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lmuzjmhk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jrncsvoe.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2femmdunu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2noojgmoe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cizrjmub.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ypjdefry.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2huotxpok.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lhpocele.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lzpojwwt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gjghtiht.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2kvrnmqtv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qkvujstg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2efreepfg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rtuvmiaq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2skjdhsrz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rghwdxmw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bpufygax.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fiimovwy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vxoasyti.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2meeotidj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rqywjsro.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lqnbsymt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vyxjufaf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zufajogh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qsdjicrw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ibfcuxfb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qevotwcd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2phgxplof.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rsbaohdd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rowalnin.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2etpskuol.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2onyufwxk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rkwongvu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wisooxne.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hoyjjaka.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2csjwptyb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qczvlnmh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2irjqfdpj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2izowuuan.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dzhsmkee.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2clyplsrw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zhlsoojl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fddcwqto.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2odytraor.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ztxjicnw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2unalnkhv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2eswexgdx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zxtzmtne.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vshmkukx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rlpdtqah.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2usoiipkm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tsmcphxj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akpwwcib.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yljtgckf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2aamrqgmx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cefweove.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ketqyers.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2epkiizet.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2earvbmok.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqkuuhbp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2peugkrzm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cdsrztsv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2lbmlygbw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqjalou.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sucvdnbp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2lmjxpaom.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2notwvfqr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qebfghuc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hfnzyznr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mvcuzdpe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2egjdwbuu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dbadifye.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2afywyaoa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oekzmbfb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bjutpwbz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uyyrvtal.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qgxcipsf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2tcdrafys.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lvnpsjte.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ibucmyzr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pueimeot.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wmffkpnj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nurrkkfs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mxqcgoec.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2exvkwrhy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tnkywyba.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ebwkditn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjgimmk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sdinjxex.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lpegzdfw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hkikjmkp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwnwgmzs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2notnrvhb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tsbaaiih.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hyghzzkj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xbcyujzd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yahuhalc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kcswatwf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rcwbvrgp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vrwmsqvc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2pciueojy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2cjstcunl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2kcafeyqz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mrovpgte.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hpqbsphc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wutbzcxt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vmwxwqol.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nheqrpcd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fftlzqcs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mnbrsjxk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xifmocwt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hfziuryy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2obvsqepe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lkgtmqsm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2onqghcjg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ghtavyui.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wucewrgs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jltbousd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tjzunmqw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fllpdgyz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kkcsoecl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ctgxnlnx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kgnximvs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ucgqjngu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yucdtcdv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2djagjxpn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cjdmvywj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2opfwbnas.html


<!-- 参考信息 -->