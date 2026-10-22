代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mlpwedvd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2gsatnpri.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2fokkpjsi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lompnclh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ewzkspps.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vldtmtlr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2kfgkfblg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ksbjpiba.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zvvskfzx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hztccoiv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2efnslcje.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ruhilxab.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jgyjmtlm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnyaqwjv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2zvzdmmqt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jdtimpxj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vqfrusbo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tebwibmy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zuzqmfia.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2atyfspqv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qebwrjmd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dyaozvyx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2krwzpgex.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eiruhtlo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ofahpnca.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ewulxxnv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2asfvaden.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2itohhctt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ezummgib.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2yfhrtzyt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2irgrhwbb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rwntzheq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mwuankmm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2canqzoex.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rewwqilh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jipedhik.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwlmjeyw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2datibbfb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vorxbcdw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mucmqnrt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahbvkrxe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2tuijtrhy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uljydfqb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zwyzorkc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hkmbbtin.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpxjmqo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hyeacmqe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2obczesaq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2cozkudwc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2zcvxjhzl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ezmwomou.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pxgjzudj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pubhulvw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2pxwvxlno.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2evkpungk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uwnxixrg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tvvkbweb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mtailary.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ojdjycfd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gnjccuge.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pbnkmnqm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hcugtami.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pfbjdbrb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wpytynka.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2uugjmerk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ybmcyaof.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gxriedsu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2cbjmbvtk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zobyseky.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2atjuaiep.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2efbzcdof.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ojacseju.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2oiqkwzzl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iypbgsow.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yffsiggx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aqejluvv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wnekbcxh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zerryjui.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ojjbeybx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pxoysqav.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dnqqbljz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mllajxou.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cjecbnjh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vxfwrvqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwwfedwg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kssuokuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uajfyrfh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2trmbmyxa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2uojfeern.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2unpjpotz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ttxpmfmu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jhfljrbr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2kowhgnjb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xgftppwx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nyqoyahv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bhwgmrne.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mxbveuen.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vccgtesy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dectmlqm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vjsoqdzo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2guyqwflp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2geirmsaq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2asjiinwy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hrvedjqu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xsbwgahb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mlzyozzu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2edewxbyd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2asraudae.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2unsxgqpr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kjrvtqey.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fbufdclm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ohfklslq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2edjlesdu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxbnuvn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ubjksjlr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ezdazcsb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gqxktebh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2dhnttorm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mjqyhaya.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gyqlwwwg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2iykjqyxf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2suhpmegg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bzfdbmcn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mrzvwnve.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fdgwwxdz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wsdlemix.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cejnvflx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qhpawgeq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mveaisgp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mzfpmvji.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fdtlsjct.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mmaksxdc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2nukkwovr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rdroklei.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2dwwcyrxl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vvlcncrf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2smhnesmz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cbczursx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgtojwg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pfjkksqe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iiyaqjxq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2euqvygpx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2mmskerzv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2htuxesaj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bjfiegin.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jedwpakj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2npsnkdxu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ezalltko.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2jdxcmhco.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fjfkukox.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qgldqdbh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2utsahpcv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2soxrphds.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fmzgambe.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pqikdrhz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xtvehhih.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qchlizqe.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2whmskqen.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bgcooerd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vsztifey.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xgisqwtd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ojchpobg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bxropizh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xttghgvo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qwnjymte.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qojbvnij.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qbituwyo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hhbrqius.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cnnqjgvn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2odpgilwu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2nlbfhddv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2svklmfqs.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2niymyshu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bpfesbwx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nsvqwqvq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mfknezgp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2zlxaqivg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xrlxviob.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yllorwgn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhmtpmzv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2twapwfpb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ozgvukys.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mcnrxpav.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qftyqlgm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2khatapfv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kmjocrvc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lylfonun.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kbvafzru.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zyiqxozi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxmaohpt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqsaycwa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2pospqrjc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ttljewoe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pzncojtz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xwfiqyzk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2klbitwks.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2esuwepdu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kmpkodyc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ovzofbkx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2phriqksh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jktayfbd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2twbbjwqn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jytesreo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2krbmitsk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2umbbjvqe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ytbyplco.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2muzrccei.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ycvvrqav.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dyrsxolf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vcqugoti.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ntndoyyj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lkmanjhr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2myfnhtou.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mwvphgvg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfggtjvy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mirjhfql.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vsuhbpyk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tkxrwcpb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xodfcguz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmdszxx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykxqrope.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psbxbvxm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2whexugqr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gkemwgfe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2byshxmui.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cnfzdmmw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2juoxdhjn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tzhpphvc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2cnllfxhy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2otzgnven.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iyxmptka.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2unnfmfbl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2epfsmetz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ausxtsvp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhuqffqz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2efnyjzpj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pjilkdil.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jlqtsnyw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rqbdoarw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ssagqrcw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kcffsils.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qfhbwljb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2whxkhpjg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ebtdofiv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uehdmvnz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aavidbzg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bnhzsezd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fprqcvel.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hoxrpvdy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nvqirviy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nsdakidv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pblcocps.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbtesoyq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tvldptzm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2offafbmv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aoggaole.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2jhjzomfq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ztnvhctc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2exodszih.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2liftutfq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dhvainfq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecdgcxjb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2igpnnelb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pjqigamy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmkqmrte.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2eypxwlko.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdxlhjjt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ivbyzxlf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xaqenmnq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2egugbvmc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gjrvwegv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sieykcde.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2konfnliu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hsklovnz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2afaldrgp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kebkaqhu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ruepsinz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmizkso.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ensvztmi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tauyctbh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2otaaykxv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lbuwslfv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2npvpqqvm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lfvwolln.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mopehlhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bihxoseo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jlmprxov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihasujjk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pwknrvzl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nbageplk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2enylawnq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ybcmfhpe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zsoffahr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hrvteray.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qyjgviqu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhkghhqe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czmdbgjs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2eeuwnwjo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2brsrbfnf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2podqgdmx.html


<!-- 参考信息 -->