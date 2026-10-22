代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xfkbtill.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2akdvojlr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bzlzhqmf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lwuaycdc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2olqauyic.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ekngohxn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kzkxgrtt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xxpnliph.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pzmirrxf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wzjzzvpb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfwxkgfb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oiheieqq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pwuhhork.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vighvmnm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2osezjvhb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2pzivwrjk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2upcxzobw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tsqybwep.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ercpxxnd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yoeotniv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bycijmem.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lvvbdidm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nfayihyc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2glptkyqc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uircessh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2gtvocbml.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cupiiznk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zvlbveiy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2syrvhppm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qbcjzzgv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2luzxkqfb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2aayfrwti.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hkysfarm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwcphfic.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zadntste.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2geaczzrf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pdatyrnj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ueirlcxz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hlheplqo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fnppwtsg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oilopvkt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2qqqggoho.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2oalvzvnr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lrzcvkyz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zykkenmp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lttetniz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2eiajbpwi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2joaqqtkz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zrdwdghc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xsrhppiv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ilracgui.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2uoekpoub.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2pkazryqu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lyejiisq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2febcylgb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nswmvnrz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wwctpidu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uwdexitg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vqeneqdv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gboygcbc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2siseblfo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2icxkdziu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uqwqmrjg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gprrwnoe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amidhuux.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mrwtfzyi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bdluvsrx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2hpiwcpej.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qrzvbwxf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ninvcztw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qouijqmo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cidlzuac.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rsggprqj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mjlhboby.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lslvruon.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2saehsbcv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xikmqbps.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dpcjgnjx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qsoxzceq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ttloqgha.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2urfdcapl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bokkfhwu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qpiehivl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zuyndzkg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sxpdeqij.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kchgpnyw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2iiwlchim.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gbqzouzn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yuoukzvq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2jrhenyqa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pozijykv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pizmfybv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mcyjjzku.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2niibwzzf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2aslxgjgw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbiftpjq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gdgyvmgs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zjpiftgb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdrcmeqd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wjdqxhnl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2raoigbob.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tnsujttd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2idmnphxg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ywuvscpd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nnzicgbq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nuijamgd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qxuojfri.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hnoryvrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxxcyfyq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ppxsjmdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kggilcoz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vkhqwgel.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ywszngjs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ysfcsyfy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uprpldrz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2twilnoiy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gknokolm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qyiwotnz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mjxhuiej.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gntthrrl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvhbfeaj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zirqajul.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bsqjkiuu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnswjgtj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzunvyp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ucuwjqjh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xujnsczq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xaqerrke.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wwzaryee.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xjvbgijt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2hwvayvjd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cmbfntez.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cqjbouxc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kpucnsmq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vrdzdmiu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2laxdtprf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bkpkubdl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2bqwdmdcl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dqvaxlvx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pilftugx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jjwswwpy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lzsnlvdg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pcxcdwba.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fsrsinoo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2habxvubn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2alywflbj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2siztoeks.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2scaisyqa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2drmxuwpk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2lfidmwvk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2krowwuce.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dgptvjdb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mtcktiyd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2prthhnqf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2plyhhylv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hblykgbb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cewxvhqn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2joopcfgj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ynyqvpnc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tbmbqdbp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xgrkrgml.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ewqgghwv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wbogyokk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ghywzukp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fwqntmcc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xonznofh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gxabileg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssjrkdgk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rjmrvjmz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mbxuzfto.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2grqowrxn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cubsuuvo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pxxhikuz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tnovbyin.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jneusfwj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2whvohmae.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cauyabzz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xkfsfyjx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ofqedndk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wdiupqdx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bppindkx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bjubgvde.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mwzkcnmy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bdexnvst.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hdqwkikm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ednfbgkt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zqytptsj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uwmjlhow.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2inmjmpqr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dhqkdyhz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vnbwmhjj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nlmezkor.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bgtujeil.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gfqcejeb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2rzdgsgyf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2auoprzgn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mbkbtosx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ampqymwl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mtybznci.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2chgpxsbg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mrfsdedj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vbtwtfyu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kajucehp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fedopled.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2auayxfbp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rhvciqzk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lrhwexxn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wynxnsrx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2oorzekjn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qvhigche.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jqdsqwyk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2akdcdwvu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bkglrhwi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2keayknel.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2edakxprz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2kretazdo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mztauhmg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2okelezpi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wmpdhbbd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2agwhbwin.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2umvqfirx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghswkkbg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ggoqnzhc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rundavah.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lsbycifr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kzfegrty.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nfjidyrn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqpaxjhe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hvokmast.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pruquogy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dwzrydsy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2srffnwuf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtcenkzb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ftyfladg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zibswqun.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qwvyknis.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vaydrllf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tyajppxs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzbimeas.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lnsanvjv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hjczowrq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2tvzhiwau.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ybodwnvp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ulxpyuog.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fhtgratq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aoivtqey.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hfdmnrii.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zizndhnl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ftyqobuf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wlzkaxjb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rtxzvatm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tqgvsxvs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xoopyjru.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mejzrikq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xzcqcgfr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2cwrtqkcy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hmwyewzr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2raxnytse.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvgeiyhe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xdfszbsy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgwhtkzt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aawiljat.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rqxzfhhv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2bljwlfay.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2lfbgmbdr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2sdqxfuva.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mpojhnar.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tumtjbfk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2difpzcrg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2maquycdv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zgflaecu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yddppbaf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhvpshwf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2istfwybo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ylvwalvk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yxokwrgc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xcoammrl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2oadsxepv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2zimfmmbw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yszapxyu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vdgwrbww.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bvhgvwiq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gyoslhvw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xxycsiqx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mpjldkbl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vblwyztr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2koqujuvi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aynzungq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wstwfrrj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2woismhty.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opigtymw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mcrbhviw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2chcybugf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zfvxltgk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gvmgkkqw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dhfdledy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yskchhqx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2yijcayrt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tnolnuer.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ammflcwf.html


<!-- 参考信息 -->