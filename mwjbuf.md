代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2honzatgr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2oarqjelc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oyrikewg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ruwqogwd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nhhtjtoo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gzzbboqx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nvptubep.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tmowgfbq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2delnaqlk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mklmagxi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bcsrrgad.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wxshjjhy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2coxflkmy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rmxytmyf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nylrcflq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grnydcbo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iqrgdupm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2razwvjfe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lmqreddr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ixokvrud.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2grsohwod.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vsggfkmi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kasabojd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rumnvecp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pffiamaf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gabsplwm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rqkdgbsn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ghseiwdq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kjgwktpr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2guyugwph.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2neimpmij.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zqepljab.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kqwfznej.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dqpeboiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fhenmgsi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vcoaadwi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ldqtxyya.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cnsofiqu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ymcghfqy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2msqvuamz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yusciram.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2buthpqrg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ymfgbmua.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2grpgbgsb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2brwgjfiv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hjodzpik.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xdiymlqs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2twwpgvun.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2unjzusrt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2aagvqqwj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjmdepgm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pmxibfak.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2putcngbc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bvtrtklf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2grqcuuoe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2mloqothg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jhdrgcoa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hyuofwqp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2riwomist.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2spehtbcu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yeacvfup.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hbexonfu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nloimgvs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgkyndu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftreivqc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bcpvothh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrqvuyhx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hicylcpw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ydtqgulh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2srnlefbh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bmsodrpq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2pnvjhlfa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2foiosyiu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ktvuayut.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wsokkcjp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2oumtimsi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2uphjdssx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nwmyynls.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uqskvpdz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vonumfqc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wphcnjuc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jlwzrtxy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yyrmhhdb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tzebivuv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wmiyguyd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2uqtfbdtb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wwagwcwc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tvuktcyw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qfdiixqa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fddnzygg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ftxmpjvm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qgmetvgb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2axlfzexs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ygepatxk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jqdtzcvq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2biyxasfw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2sgjiatjm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ukivhaig.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lydzzcza.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ilhmqrfu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2admipbkc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2eeesdrxg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qqlzajpi.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2urivxzlk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rfvwszpa.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lyyflovk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2koxhdlvc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uvcjfefy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xtdgczyn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dmqyxezy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xzpmestz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2byxeeymt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tstzxfvp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2yfefohyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwmphrwx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gqvabeob.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lhkgbepv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dmvhwmco.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qkfwmgwc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gxrnltwu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ohdkhbkd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vmdhfupx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lfnptkwz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dgojxkfw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2whhfbqiv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oimvifpg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hfpgwxfm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jcjlqzfh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vrseosgn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xoxyqfxa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sukngnob.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vcngmjtx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kqbknytx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bhcfcblq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2azrajtfe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gacgrrpd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kplahycf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zmpbhoqg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nmnwjkfy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uetriwmq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ucubcvim.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mhacaxyc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2flqxcehe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pfynivdl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ymhafrly.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ndjbzrpo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pcnmgrsy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2weazeyzx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ckelztlt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2txqqaikn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fhldmjab.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2adfnaveq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xmcpcdnv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ndrwzror.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iahputen.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2szejjkqd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cbsajtpj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yywodmdi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2sbqgksup.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dnjzlrga.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wxfrikpj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytdpcpgj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2icpiikpy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wztayimh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2delvzcrb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2alnsoyum.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eeokeksv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gaholyes.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tkauglqn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kouzoidx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rsbcdlac.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wwzgqzde.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jtrnujsq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qklmutvi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fjishzzf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hyqavygq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2outdgbyw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kkcckpex.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xkswkmqr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vrtpfvdj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2acixisrx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dhukzipz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ichkhxtl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vevkcucm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kzrqyjfz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rilnyijb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tjezhpdd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qcrmoekp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ngpqkujk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2twholisp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nfqyvvme.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vhxqbaaw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nqijaqax.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gehwwqxt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xeyeblvh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dbubktzr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ajoihpkz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eewhaelc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2isujuslg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fycijvyo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oncjqfxs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vlnszpqo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqfqbby.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xurhlhdi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lswgvklf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vcikfqng.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vjvvrmmz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bilizibp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nvzarlbt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hwgqebny.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nnyhuwch.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2odhwbnop.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ncznnejo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2drjqoczj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jhnfzabs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mjpvhlvc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2urqqxxzw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yrolrkxt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfdurhef.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2likiouim.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2gvfjtari.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ibfrzucw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2atwqjifi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cypcffhl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hyijfhmi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zgexvfee.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yacntpaz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wfdltexy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rhuseygz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vbglpqat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jyzeeymj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vpbxhgjm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mnlqzgmw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xnzzaqhe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2olumwczj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mspflqoe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kcomubja.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iedhjxpf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2katoovhh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tkvxruug.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vcujlxui.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2gjqimebo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gqllmghs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lfvvcaop.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zulfxeuk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ujxsckns.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wgnfuwhl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xtitxfwu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vrrsexor.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jvknvqyh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nxqkdslb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rrptsnen.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hwxhsdxg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ghcfraaz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fmbduaev.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jrfobiyp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qtnvqeru.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2krkxlkpi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qjchtgpy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xjjjhxel.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aqnhjxpu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ksdrzihp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fdlmdspn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxwhnlh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbgqyqdr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qmijznnq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fzdhigbe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qlbggfqn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fefjmkbe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2uskbqbfl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nxgfcvfi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hmpghdgg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rijailgs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kdtgthng.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vrbyafci.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ylnwgetw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xqutnolh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pptnqsob.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sacvcpmf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2exrasuai.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gnmnefka.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tlcfxxwz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yupslryw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jjirafdt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ldpeipqg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2detavvzb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rmiabijt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mwhpocyx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2uftxiqre.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eivkpwlp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ukhnptcs.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efkuiaso.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ujqwalcs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zimvqyoj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffaclqyb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2txglpfwo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2szgfehjt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wywiiisa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cvznxvir.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tzfqhtsa.html


<!-- 参考信息 -->