代发 wailian999

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gllimsujj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gmkelyfkn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxnuqvlap.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gsntfilnc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gntfhmujo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/giuglolso.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gxzesaaco.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gfnhdsvuc.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gfblbcltm.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gzthhnonc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxmhreyhr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gsmclqdwm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gmxsbyzqf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/ggxqoknqp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gslvcropr.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/grsuootkv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gsjokznjx.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/geuoxcasi.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gjlsbndin.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gqfejjoia.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gwbepxbdc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/ginxvxrpc.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gbixsklks.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gdlgemiis.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gpqabrbtj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gtqucdnns.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gzrzvcjhn.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gsrzebptd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/geniwrgwz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gfqgpuvvf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gasddaxku.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/glrfixewu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gupqjzdes.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gbuchvaxu.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gvvtzcmex.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gtnhnchba.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gvflpckjt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gxhtogfsu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gapscfgue.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gpjswdanj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gnomzzacw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/ghmojgbgd.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gorexmnkr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/grdembmgw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gjpkrstqn.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/ggjgdklur.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaqhzlvdd.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtojhrnlg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gxunahqav.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gnxrpziyq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gevwnivad.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gunjgneed.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/giqskynlw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gjzazjjqt.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gkvbbzcin.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/grmypwcft.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gclaugraq.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gmptedxhu.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gpxfwpjcp.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/geuqzopwl.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gbnaxrrhy.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gwhmxexns.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gjndyhnea.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gykntkkxb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gjonyooay.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/goekxdift.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gewrzivaj.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gzaygctqo.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gzcodhcfq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gybqzqmoe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gwpfcfdwt.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gdpatfztn.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/givdqxjkp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gicdvyelm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gfmcfwrmo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gnefqtzlb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/greatkxnm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/glqtytnxj.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gppqlnhok.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gmjoijaji.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gindevwfb.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gonxfpcgm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gjzgqidpg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/govihnumf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gwhqhonxl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcltjozpe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gfshlhfcm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gkphftnkt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gwsnapvwr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gawfgwval.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gcsgooafs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gpyxqysre.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gfdvutsef.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqtlctnoj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gbataozzx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqdzrjfbr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gpbduixyf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/goyyxhwfm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gzzxzczbz.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gzadobaeq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gftjislke.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnzljfnyt.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gmbxsytgw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/ggmxanhfa.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/geswzvvpz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gcomzgetu.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gagdhwudz.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gbjrgmiql.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqnrhhdfg.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gixczwhuq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gomehzcmo.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gmhkkkqti.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gkwjwhwyb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gzafrddal.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gwrskjmjl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gfmzvtfcf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gixdudsbc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/grexzuydq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gqryocqeb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ghelywpws.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gsjpmjfrs.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gfqzterdn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gbugjvbrj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gibomymsn.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gwdjcsqgl.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gjlmwrwdc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gmlucflsi.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/goayzxzwx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gmtxryfnu.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gitiioxvb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gmtdzqjwc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvqslpkkg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gxeptnijk.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gpyaelpwv.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gxciiobwn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gaipblwxg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gsclcfupf.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gptaydtwm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gjytuondz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gtuqtoxms.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gjbxyybpl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gtmdvzaic.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gpvgdmart.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gznqseodi.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/grxssnmrk.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ggmjkhwnm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gckgsphqn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gbwdjobgq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gsxncdrlq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gxjcdzdmi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gdwggaftp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gogskywzi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ghptxiiua.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/giiejnsxe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gkkrqmpxb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gnqtrxwgc.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gkptlvrmx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/guqcmuvgi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnbjliqdr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxzvizitq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gtriwdabj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gfkgdcbub.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/guzjuhxac.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzvtyjvyz.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gihodvcxb.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gvopaepzj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gbaketzmk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gztnhbzrs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gsealkzpq.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gynexpzxm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gdyuxcjfm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gmmykmblz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gnqlhvkvl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gnhrmnqic.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gkyncsgkq.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/glyqlkipd.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gragkgkoq.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gusvlmxci.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gzpleaxfq.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gxoilhzmu.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gdpyrmqux.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gjrbzlies.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gvfmfvwte.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gjvkklrxx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/glhjlioir.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/guewizqxj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gkfvdkupg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbyofpzzy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/ggopddgew.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gxspbsmoy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gcmcrevfx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gaiiweurf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gumvyetsz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gdmkyuhnr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gfcwyxdpv.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gjouecvyz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gfiqhoahj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gdddalqoo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmfmaxcgi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gxchwhobk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/ghzsuzjpn.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gmqxxswvo.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/ggknmfrcz.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gipxqqndg.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gbmfkoegv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gokbmptfw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/glpzomzet.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gueigtrug.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/giywxiiyq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gnejclust.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/grwjewwer.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gtjdpovdr.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gmbqwwdhp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gguqdeiih.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/ghdtlcdzz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gwsscglau.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/grmayqhyt.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/ggyyduvnq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gpxxniqxu.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdiljbdbn.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/golabjpjr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gmiarazek.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/goccfrsxr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gjfrilweq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gwjhgppzs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gnltyaocy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gfkqbwjac.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gnpwuyynx.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/ghscgvkxy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gvgymulqk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gvwdkjexe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gqzpidtge.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gewmvxpdm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gzfbtbmum.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gtlhlqabu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/grjjapwcb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gzizhvbcw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gvadbmbkt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gwwmjqyhf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gcmaqoxwm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gbrcozkig.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gpzvieyay.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/graapjuey.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gtkttiwlx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/ghepfoeua.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gtyzstdax.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/grthtcnjh.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gdvnlvrin.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gxhrqcbvs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gnhofqrnz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gudguxohc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gaxpmkedn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/grlyoyacd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdjqixqgv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gusvdpesz.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gafhwdryi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gleerffkf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/genfucmom.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gumupumlk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzexqpqb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkhphivra.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/goanesbuv.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gkryftzka.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gfehdezev.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/giewtqtbn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/grfqlcsya.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gsjryeixe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwrjnokka.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gefyhvdkd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gtddfdtbz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghnnaatfc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gpguvuord.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/geqkzdqxt.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gifkxlfzj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gqmpbvele.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfakhhhk.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gqhpheaov.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gbxquflhc.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbdwjtndu.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gicqqlxiz.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/ggegjkqso.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gzmvtrkdb.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gczljmdoe.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gxikgrqlo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gydurosfm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gzdcwjhhh.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gkxqvqiel.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gjgjzkswj.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gehtthbsk.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gfbnzfciy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzxeqmoxk.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gsbocltix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gyzyiqcjw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gsltvscqn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gkmhnanqs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqabqdihc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gemfwpiho.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gfsugfshr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbrxdceta.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gsfxmsmlp.sHtML


<!-- 参考信息 -->