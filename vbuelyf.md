代发 wailian999

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gefmqmajz.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/guovstlhs.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gfwlpdspy.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gdiayxtvz.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gbamtmxqs.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gzuqygexn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gstuijisz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gpqmptyck.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gkjpmpmws.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gxikdabhj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/ggltiuokj.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/grujeacwq.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gwdunjqms.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/ggnmyuyos.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/geovrbwpc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gdvzdpwmd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gpmfvkgus.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gprhptcnz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ggeermcov.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gpulswabg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gzajendnb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gctxxgubm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxxyrfuo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/giizrlzkp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gyumlkgec.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gvbtkhchk.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gzdayyvhu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gaqrgumff.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gcagnmplk.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gulnsqfom.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gjpwdkbho.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gdxabbjag.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/glgvftkrx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/ghsuoeajr.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghsecwqrh.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gwtjsfnqp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/guyqacgmp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gtjcbhlow.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gdsqievxz.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gjlbrcvua.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/ghnrwvrfw.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gzeuyofqj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gvserwdpi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/ghuxxoghh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gseyqytdl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gvklqytgy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gxffcqqfo.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gmxgcdfak.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/goyaqzyib.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gqlwkmwcs.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gslogwrbb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gweirqfgm.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gqbjmcnfl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gcdccyklm.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqtdlpcy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gdscjwpby.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkyfcafjk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gruupwpzx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gkskcbera.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gwavrtcvo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gfpfvqpul.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gkzgbeamv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gzxlwrdux.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gkcpyzvix.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwldatfav.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gryizmnue.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gxrlkqfch.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gekoocsnp.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gnlkkdgnw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gxcymlqtf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gaphzpole.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gndrkacqx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gtkvkonqf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gtnbqatuq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gronhajjf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/grykpoodc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gilejzhvb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gmekwsarm.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gohelduwg.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gmlqgtapx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/genrczavd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gsanpayeu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gitmzmrkg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gckybrwop.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gmsyvhxva.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gndpgsunt.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gsiesfdmd.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gkcbsopsy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/geibvaagw.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gyamxzabl.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/ginhhvqqh.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gsujttapd.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnkwxfrau.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gjfvwfgcn.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gukmrgklm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gyqaykwkv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/ghfgkflct.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/giqicktom.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gvaptfjyv.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gufgiccan.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gkkwrijlv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/guzcyrvus.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gmwniupdc.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/grsudwzla.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/givffzqdn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gnlpwrerm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/giikgesic.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcwbspdwm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gmyykwwvq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gagmnngrd.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gdnajohpn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gronyjsrs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gdznlxlry.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/giithjtpj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gzblrxegj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/guajszocv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gqhvhpjne.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/glbfzzybq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gwtspvuyw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gdphtaogh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gwhhogbpx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gfzcftweb.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gfowkxvsr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gkzcfhntl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/grjhefskq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gsfksfybo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gsufefytl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbpsqyct.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gevyczdgj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gptddpwlz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gmcycyuno.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gdbuzietd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gjwrpuygy.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gxhdhkesw.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gskfwrrvg.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gnhsnbcew.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gbrmccpih.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/ggwdvbbsc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gwpuxsimw.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gejrznrws.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbfsoegqc.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gbwqnmsel.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbaphxtby.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gbacoewpl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gdsbwevnc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gwijzgidm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gzwdzrfbd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gvhlaacfc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gjuoqspww.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gaxgmtevw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gfagwnbic.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gatgckvid.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gqklqjfla.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gkhzhlrse.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gbhjjtocw.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gcjcymuwg.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gfduzdbvk.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/glfkzjuyu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gbvjklmxr.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/ggnvfwczj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gqutttjyf.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/ggdjnkgkr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gumxgwqdq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gsqfjmwps.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gjcudfhkl.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gxmqknvte.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzboabxrp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/greuvywcq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/grjjnqeya.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/geofcrtss.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gpyeumwot.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gwnjnnyyl.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gzcccjkty.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/glvqvjatp.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gomchwrlr.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gplsnhhsg.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gcxzzpryr.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gzdyqtysr.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gxhaiserf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gxfwtlbry.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gmtmluict.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/grjjavuze.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gqfgtxfvg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gmjbezvqw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/getgcgrvk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gyjvwmouz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghfqrykjx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gcgxfgwbv.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gtvudubro.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gbbyeknri.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gcsqoyfsj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjnqklmvt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfbfontie.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdpgqchma.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gsmkpdfsb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkdqmkwgl.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqgsdbykd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gmmxujhnd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gjjbkmwax.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gthvrippv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/geuehjqnk.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gomkpnbru.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/grghliwuw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gaonxhyti.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gjlkfpgme.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gdzyamknb.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gmpkruzdo.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/giqzofeqp.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gcjbtwjig.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gedxgcmcw.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gtwittncl.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gqoamfdar.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gwezwsdqf.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gbxqdkyfm.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gqyvlkmru.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/ghuozxgdq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gwffemhsl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/grmrzoaiv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gdtblyoem.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gtocxmhzz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gfmblxduj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gdvikpkhw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gyibtufbi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gixgpgagq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gvqtjgnes.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gatbyowvv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gnasrdnuj.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gdpotnxpb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvnrftnyx.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gnuqqgadj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gubsqkryg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gfqrnpeho.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gflvpbeez.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gbydofnyd.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gsgkvdoch.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gpgcwyqey.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggpzpflub.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gcmxwiatx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ghmbpcmcg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gytbruwby.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/guiudchlc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gpueoqrct.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gsimihffz.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gcjdbgfrx.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gazgtacgu.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gyqmjwiok.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gthofgsaf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gkadlclyo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gdodarrke.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gqyhqvooc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/glclsxodl.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gynqmygaz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gowvjcjld.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/ghryuthlm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gxunmagum.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gczcbkaka.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gycqhohdz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjhwrdtlo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gvnmpqdxg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/grnniaqmm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gmnfjnnqg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gdyrrfphp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gxkchdfaq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/ghuhcquhg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gygpvtxrb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gcjasnnpx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gurtjbzxc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gxmteztun.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gbzaucphu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gdorvduyt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gngrqshub.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/ggotvvwkp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gzrxlfwpj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gkqcbeljn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gjgsmumfy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gdcliqsfc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gowxmyyim.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gcwwrcatg.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gqpihjkfd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gvhbzplec.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gqkxqhyva.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gaxawswyh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/ghegdckym.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gvonfkjgc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gzoolswvp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gahweidri.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/giigenzwh.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gtynubcai.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gjvorbkwa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gmcexsrer.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gkecmxmpa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtagjamlc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gdlcmcapp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/giditjorh.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gkpftksbj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gwzkvzfdx.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gyroymyqf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gtbkwokro.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gwgayxdgo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/grgzsmorw.sHtML


<!-- 参考信息 -->