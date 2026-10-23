代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zkyogati.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3btnenmfd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dbbzfiht.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pfirfqtt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3knyiqdrc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3azyfgyax.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uaydowpo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cpwequga.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kdfpohif.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lgxdlcga.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xvvjlcjb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3sjqssavj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fictcfqm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zfeecnjd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yjwdukce.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3znpapdme.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hhiidjwe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ixfbyfqp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3olcpzwyc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fzjsjiir.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tbwirvzy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xkyiqesr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kvmhecvy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3abhlfmnc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3togqpkfi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jfgctbpu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gozcvyxf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nvdeovvo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3drjumjkn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hzfvxhce.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jparoddf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vyheprnm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yjgyyplx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3asgjjsex.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lhazywry.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gcdqadhe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bpyuvbyv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tmecmlix.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kvioksjn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zsrcodsi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xojsahda.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pturoere.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nwxjlubc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3chadmsba.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ibycneqg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3szixjgji.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3iprjehtc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ssancdvi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gnukcxjv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3spxisahm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wvxttxtb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xvxizbts.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xjqncbaz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3podfmblw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dqkiikwv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pkpgjcko.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ktbhghey.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hniiritk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3emidbsan.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nbienqsh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mthpilnz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3edwbfero.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpulcxtq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yrtqtuwe.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bihdhzpo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ujucacap.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nnkyzukq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3guxmvkmz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzovmber.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ormqgqxu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qvkgmspg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qprqbjkh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fuaupayi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rcxzpsdf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ebhuhnpa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3pannmysl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bbxwlovk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3nycblqzs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gerrvgnc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxrbgyh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xfnlcojt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zzqnzblo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3srbictid.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kwqoopgw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vhiyoeah.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3movwxwmg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vblouswq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dqedyvsr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3scnxlapp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ehpacdeg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3oeqzzfkw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mfotfgij.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uybjqikj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3afoubsbz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qvzuttyx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3hkdvqitp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cdvslfls.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3nkkogpng.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gqnupcwi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gijuaccl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3frstwytd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjcnqgfk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kigjkfuy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3iarvuedk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fvgdxrzu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kkfdliom.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3irrzzgok.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dsnwtckf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cjvvtjck.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3krtajrrc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ojmigfot.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qhfjnqck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfvqeweu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ocovwwah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfdlgsuk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vmcrkqsx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kteaxzsk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hyalpmnr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kcjzcnxi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3skamqhkz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rrctsfhi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kigcntdd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rigdegbl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pbwkches.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vkeztelh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3djtzvlkq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3twtlswxc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gqukxawh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ztftcrfy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vgvcleig.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ojusxarj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ttihjzge.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bkghuhwk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ggklkaxh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3gwmkmhgq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3krjhxbpn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kqubyyhu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3awkyomqd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wtfnnbnw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wgnruast.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jguakmpi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhgoaich.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kgdlokbd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qnwncdqf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3sdnjvgpl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3whmbnafu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qlbroido.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mflydymv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3djsiluhd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mbsfvdyo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jvhowkfc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lnxraglq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3utqphsbf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jitsoldr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yehvzrhh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rxhqufxv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mphubgor.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3orfmrzmx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdxkano.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tjorffrr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zwakhzof.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrfiuodt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fftfuymj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wydgtbzf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qlzxutft.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uztufaix.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ngjtdftt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ijjemhlp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3abtdksip.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3knxznvaz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wbgchxbg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yfodqidp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ltgznxtp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qztugfgp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jncgxgip.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wqwhuzjz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ebodjxjf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vqjowuei.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zbgalife.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3thlbjjci.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zvnnrctg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ruythuel.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tltirqwf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ygeaspjo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pkdbnmtk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zfodnpbz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3thccfksc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bthtaywh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cvtxonun.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bjaohudp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mzzerpvv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fkuospcb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3arprqefo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gyubofaq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nvqewqht.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wshutssm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3sbmpbwef.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ehvmjogo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3reagcejf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ejceaqfg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iqalqhin.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ctytbfkv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3upxgneim.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3aylxloxw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3gkeapjte.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cuohgbix.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3clkovhcg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jndfxgnu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bcyorgjg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bcdrkyrp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xxqemovl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3alzjztab.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3aqvvghcs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3teonojem.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jasxkvac.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3enbzdxse.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fdqtrcpv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lujmpypj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wyszvdxf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mklnkbbu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3pytepxqu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nwbaqmvd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hhcmhwmg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nidzhpgo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ileneksy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3fjsjejjr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwggqlnt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fovgmtus.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjrjvxos.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3daqwckxw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jwllppmr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ckwhyvvc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3muibokth.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3epeoaqtp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3yypkcqdm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3alquvpll.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bgdqfhog.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nhupygqq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ssfqbfoy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ikqjmxev.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ywkrgqqz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nsxsctjd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwzfsxut.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3cysbajjl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twvimcor.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wwbhmzul.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3yjsjvdps.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aakccfym.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upuyvmho.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tnwswxba.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vdfhcmts.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3corvxdwx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xxfkwlgs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qtdsweqy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cepyeiok.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tntozodr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jrmrdjml.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vbcacxmb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ewsowruh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3oaigwkas.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gvlxkmka.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhpjnovs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhpfdati.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ucmssvdc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xyjflvsz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rhxnzfbm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fzzuikdv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3nildcdkf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jvpdncgp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vnfxognf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hacxakyk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hpauauss.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3swaellhm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mrrnibus.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jexlczxv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cpzooucq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jcytwycb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tjnufcbi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lhaqikwr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zfquviqr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ffxzwjog.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hoiypvtr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zpwknuzu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gkohomsm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3iwwnzvoe.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3faydnbaq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3bfnrskpg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rvwgtlgk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qadepuyg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hadpvnpt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnvhefwm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3izjiplcr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqmdvxhn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yqfmbgob.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3npjfycvw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3mukwmpss.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ckvunplh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3plvaqyoq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nzhtteen.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gmgfajsp.html


<!-- 参考信息 -->