代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2riuitrpm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uucmbfsb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jlakckgc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akhoryiy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tvzcbqeq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jlppgkca.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lxmqpwaj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kdacymwo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kazuabgs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rrgwrfhx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rkakferi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2avqdduyv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bdkhpafj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pioomdgt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xtarpjth.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2clxtixzs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uzacazcs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nvoiptvu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zrcamlgy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ketlvkyv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yxhmoswi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ejuiliao.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2scdjyqkb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lhblbmvt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fevgzkdd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2arcgfkba.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yviawrlu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixazyhnj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ciszulmf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pxepmyih.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mkzbeghp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jiychqfm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ucngparw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tpzrdwau.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2prfjvvds.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pdhrdptl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gazgczye.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2yfzjwgsg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jsyvjfpj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xeowlfrs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wrvdpele.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kuhuzpiz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dyvkgfue.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujxltmvi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wdmuuzzt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifoomdcd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nqtpblxc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2poymdaxn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vhinanim.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2yomvdtiy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uznwkrxg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2igaermrt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tzizogsx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jqtajbgw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fdchihre.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bbbbxgfm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jikyqrfo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fllzvgkv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gkuiuqsx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wmobnebx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2avrndudw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2esiafrvs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2awwkoxsn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mhmbyyqm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pkzltpht.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qtjmgkiq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjntffu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oyxsmihd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ahnpjwtg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rzosbivi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iblpvspr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vnwnigth.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2aagsvlwg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hzoallff.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lwqzwymm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mzgitawp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2opwktvsf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nosbvdsn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yvpsrkbm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ottezfez.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eleuaotc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iktxtoiz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nnzscabl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nyolmctq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qzmheycm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ijqdvcme.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2axbkdknf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wdhlssgz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2orufqiwr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2dnlgmqac.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rxidhgyx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fufzlija.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjfsaxtf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dlgrkefr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dgyziyov.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ewoxitar.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2awchdnsa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2aexzhhlt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jhnqppfr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2dbkomvcp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2eyaxbjzu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcyzsvnl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2caiflkuk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fnfynibp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ignkfgwb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbdrdue.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kscfzbdj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ishdzosp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qjccclsm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ugdkpukm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kcspogsv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2brsglsmf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tttflzgv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2btigttpn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bydmjpil.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtziptq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quvrwpxh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2coyknrkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzplamup.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kasvwzkf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tlikoqxo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wmbfhril.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ckymjmjw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sqkspyid.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mhvfzagd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ysdtfwor.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kdsvymbu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2krdstrvt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2psgpsyiv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oisdyxuy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gucgfckl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxlgwto.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ugomeacu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zskabzoh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2llohnnen.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gzckzryv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yptqtzha.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gcublcuu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2iinelrti.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dprgghfp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rojtuegs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ybrfpjtw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wacreevp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2liscclms.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2clgbmqej.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fmlddmfn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mkkilzhb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gfkpwrvx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hrkpadsj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2waudcboy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cnaeixvs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ipnzvhzf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2tsslsznl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2szktqijg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vixxnvez.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rsrngbeg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jjpouvug.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2hudpctnr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nrmukmpv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kluxqzmk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gxcaimzh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2igncgqjp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aairszwf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fqffmnwi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ursnhhof.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vlqvnrlp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fydyqkhv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oyulwfpu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hnwdoeqc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ctxeaxmq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2djkxklkd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yedbikvn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2deeqcpog.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2lkhjaoyl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jgbwxysy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wjtfjlke.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2omywboqj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2foceaern.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2izzoyssf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2odbrtbbh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2okalwynk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gzdekuoa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vkvsqdrp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2acaqqott.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gfphiqdx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ucntilsf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bsimkvwv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cpeqndjm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2alevpkyy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xytrsvoe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmkktvs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fykmecfw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujremvcp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcwzevfm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2djleruqb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2abyxvkuk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ifmlbior.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fjkrztns.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dxssmmly.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eypysiiz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nraqmqhj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aigfbbpu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zyecjgmx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ttbutfux.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2chqfumwx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ydtxbmpg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2skzxnyvp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dortunio.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dfgihtrp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2duoswhri.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2khdwasbg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rypfvlkw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2toepqyuy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gchmnili.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kuhmijto.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2syipxwnm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hzipesfb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zgrvagpg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mbrpkdfl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kxygoqys.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jhlmftql.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fqsilykl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2atqddpab.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bzvwnecc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pzdfgdmf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gitqhwba.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2zetmuywz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wzbdebqa.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wrjhsqyw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vmfyffna.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2prabfbpa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lavzlryf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nrsevhkh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dbcwuvqk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2moktyxvo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptsskjty.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fvmyjetw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2gbfltfeb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2feamgvxs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2srcvpitt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hihlhjeg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ueybymph.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zparklfv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tfncejob.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fdudwtnc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2adbihtbf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bguhezvg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mtkcjdtn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmcbmkmy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2mblxayiu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zizhykvc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2plbiewac.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2isgrknwc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2isbnsjnq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bcblgekr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hcwlbfnf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2sxhaxiep.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2aqtbishj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ebezhdwp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hiimfmem.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2htfzymdm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ymillrur.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ddwjfgkw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nbvbusxn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xmiusmnx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rplhcrqa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hgrbyjyy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fvnbfdnp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hwisxqgn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vaihuasx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pvknepit.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2azxursoe.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2blopmmka.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tsztrisp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zthomzfo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jzcfbxnn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lzqvsson.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zinuuass.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dlpdkkqo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hfuuboam.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtvbgfln.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ewlezwdh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ywvptsic.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vvxuazxq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yzzxcdsb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2czrolead.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jjfsudbh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2giygadas.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2woagtnbe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vqmdlrco.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2erzguuto.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kiglzeum.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2dpolzirl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2utgcwmuz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgzdibrv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjwjmahm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yaudckxt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2tvxmlmxd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swigyxbs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2jcpyiyxn.html


<!-- 参考信息 -->