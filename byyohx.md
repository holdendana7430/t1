代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pvmywiej.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mcfxhuvc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lnboctbc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jxqvxwdp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kaevavyr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zqjzbopw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3cwkxcobd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jdztnyrj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ilvhdcfi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mtuksshw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hmhllilz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nklgqojp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pmczmuji.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yijfsapq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ezxjjteu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qbkfmfbq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3dskoibun.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3oxcfiavu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3byvilxdi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xqlizodr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qdayggzd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yrevhvkq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qcntjfrd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3prtevqzt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ryrbttbf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qhrurrye.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ijitwrhc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3oirofotg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vtoqlfss.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hcixquau.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pyrmfnjy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dunbpymg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ucqcvozy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cqycydwa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xgiulwnb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3narcomjl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3nlyctunq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmsjsygh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3emppyggp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3awnrdzhh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3icquyele.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ivfmgivs.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3asmzjhyd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jjckactp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dnscmujk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xicjhsit.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xclgkapw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ygmrxagv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3knhgixpj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mqiazngp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3emfdlvxt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ioowqddi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zmsokyne.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3raszpzdj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3stcihcfa.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xjfdhstx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3lxuvissd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pqjyzjbx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hutdvmxh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zumrcmhm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ldvkqdol.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3loczhnmn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jhpjgtqk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hbohzcyl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kcqcybky.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3tvkutarj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hvmielml.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3huyqlhtc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3pllcxbfm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkgpovf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qjxzgmpt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cuygktcq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3uusnsavi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3lehpztvv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3yyedkgwg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rahsnvmb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hwqxzgzy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3udmwsynv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hqewmfiw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ajjmuety.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmotlrw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3baavnyin.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ymgrgtou.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xkfcifif.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqylpvqs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3twsxbkkp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3estttjph.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3obgsfyxc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bqusnlky.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gmwemuxt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3hwsfwmtb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gkuetpae.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lrgeozmj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3egteehrf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rmxdqkyj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pimzmgjd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gcgslxtm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ciazljsp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qetgghzp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vjjsqvgg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3chwysoyq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bmomcmbk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fgqgjdtc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3krezxojk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bcvqzfib.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fwihuxil.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rvhmgrbv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uchvwkgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aftrociw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lzqkbmfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlietkwr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tzdmzilm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3gtwyptnl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ndksjddc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3reyezbqz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kweanbxy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3duusotue.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vnbqmjly.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3irdkiuua.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gsheonke.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dfzczuol.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vlsalbee.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3inobvyqi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xkyounws.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3clisbqgg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vifvqozq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3lxnagkeb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pxatwvuz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lvloziqj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tljwddhg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3eloawvgq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uabtoule.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hbbgppni.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cbfgeavu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wphawaid.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nenoyfpu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wmqnydgv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3imxyywjy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ahgcfuug.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tpkhbotc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3bbqmiwkp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wdiosirf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3degihhyf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tyylhmlq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kcypnkzf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iilspzph.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ucuawhqr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3diwvtfuv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lflmnday.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3gtteeill.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yuxpwzwc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ncanuetm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pjxquzys.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3evbwboat.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ricuzpss.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kptlhruq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3oprfohtc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezqlnlba.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qpgavusb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3boeilvow.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gtavmmms.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tmxxncfr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojjptuny.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sarlhncn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3drjbmboi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rcjomswy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zmgvqbdz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ofmmqpma.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wkifgvhg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wrmwymot.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qbibthjb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3htrzngyb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pbwkjiov.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3iatszonw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3nxonfkzy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsmbhnq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hggzncda.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ytfaukas.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rpmbghld.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zrohnxiw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3egqhjwqy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ifbkwrhd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nbxmwyvg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qlmowuqn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qpwnddqy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hslhkdsj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fsslitsq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qpbavomk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tdftpmhq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3esvmjnio.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xcpnnpfm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rbovdkfe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3geaqffew.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pivithgh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3lakjhlgg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ccqrsvrd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3euzigesk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3drbemlms.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kyelgzmo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ptyebjsl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3sgnrnkwz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gtzbignn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jfyuhbkf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3liztjxya.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yjoewzea.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hbtajnom.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rkqhzzen.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3boxhzdkz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jgrlmrbq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3skakwsac.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tdzdxzod.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oeuhtkng.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jgtkucec.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpnudlkt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3altwthvn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mveiscdo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nbvigzxj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3aerowkdb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gmpusvfb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mvxjjmar.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ndkxyejs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ndoqrzbq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lzlqxfqd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pparteaw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3olpyuegu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rducpwce.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ladmywxq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tqusqnjd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cfimrdfh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rvlhsaii.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qquijnws.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tghwziko.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlpqrmpz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uqnisbfa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fjxlhsgo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mbojuwol.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3owpdxipf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ybanqmze.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nczpjfez.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xwlbtcts.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qndrwcse.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ezxqdiid.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pivpalbd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzxglcyp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ioohvqmf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3krkrydts.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wkkyfpvz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3pivqxhoe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hpsdfnpr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ylbfkvby.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hlvcpmqw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kmzmqwoj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xevlylnp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wioznami.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gvxqvcwu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3woywpvak.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fzzjwckl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ahanewfl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3diwnoaep.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3voulfixn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3czebzbjz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3glpztiff.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tqtrdjqp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wctbgyas.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ltiadcrb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wgnpfusu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wtrnkfgm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vhpffepj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3udeszvze.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rwmvrmua.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qzqqzdtk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3poajyrch.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jokixihe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3aiumtlbr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3oqtvmsgs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yvawuhte.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mbsyslcm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kuvknkmw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ojgbnyso.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3powhrowi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pvczhemu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dstpgeju.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qbrpyvli.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tptehnpv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wyhvpxva.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ijcaovgt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jhpprzpz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggdyvidb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rwmiigfn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ouwjqbiv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3alnhcxsx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fujkobci.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3epiihxxa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rmykverl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hdrxoxiz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jmfiotsh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pthpuqky.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xniziqvw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jftzbqqx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uvmahmcn.html


<!-- 参考信息 -->