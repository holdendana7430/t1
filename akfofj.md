代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uqkkkbff.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bgmhhpra.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dinagaxi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zjxjahtw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vapsheqt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2harvxpgp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lczxhrfx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2euivkteu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ezhxvdlb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dfdumwuf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ooolyxix.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zojhjltn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zuxztoid.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vvjwkyog.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2mzudwuvo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ubkonise.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tbneefvi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2njudbimf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mhasunhm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ixlrdnph.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2egbikgms.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2clgdrtbw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uorhcptw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jqrlduto.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2frvfoias.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vywuobjh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ycqboidp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wbidmiof.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hubztbmt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nscflvqa.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lrtyyqrn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wlsexrdd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ilrpfysp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ayfstpyp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gtzxxevr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2aysunfrb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ptukzwzq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fdupwtdy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nmqmdcnz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kejwhgdd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2pbsazfqz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tankizzg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2lhtqgrgt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2duhpxuxs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2nngxdkys.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zehdhmsc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdlluonh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iullasnr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtxsbsrf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2josaadmz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rxemgdfs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2eeouzqll.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xacgramn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dzisbagm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ytcmbryr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wxxlezkz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2lbfdryay.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzyqesv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nbxkkkev.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lpztphfp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2anvudksq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxvdbif.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2reukvbie.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ncjjumsr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2opgwaxrf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dxseoetf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yrubsqtv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wlesnosx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vyjecxnz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pvmvspnq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gqtiatxy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zxfnxvao.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqcuttyo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vqalmuqm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hhlzfmwn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ypnyascr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2jobwmbpz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vshznquv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ilbvokti.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dhryquft.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2screslxd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxvlkst.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nrnixqlu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uplifbey.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ifknofpx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2nnopmyfb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ruurakla.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cztgnwrd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oeybxmpl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gyanlkek.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2knmonjlh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2snvynmqr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ojdciymj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eauqlfpx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iumunvhb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xayzbrvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkwwaqoi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tqzbqgwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhdelvab.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tkhwdolj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zyuteeoh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sbecobmz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2waldloxd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2liwrejld.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2afzosiga.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mqflfbbb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2duhuqscw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uvzxfsiv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2krnxfzkp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2auqjzeko.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ufqbjlnb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2amlfyzmu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vgtotsjr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ztyieqov.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2audmtold.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qmubulss.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ecrcmtzj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vnerbvrp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2oomltjju.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eszbzpmz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jeuhxriz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vdcwcmwl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gvfsdpmd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vpppbhyp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xndopdbo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lrtpldpq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dakqnlwg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2duoxqjwf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ccoceknk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cdwyhnay.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ktwygjyc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zzfdvrls.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2uhosevku.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2idfnatjb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xqxiakpz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vclknjdh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qbkgrfpo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jwmjdsul.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kimuukzs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ucddaexd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gsybecqy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qiwruhtn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vdjttaax.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lcgdwjwy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mfthqpbt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nunsszhz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2geuocmts.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ynjqpcnw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nukvumsl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bcofanrb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qkvhprgy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gnjolave.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2prdmzloe.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2erzugvsl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zwpuulah.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pwtpieca.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pwkbqhkg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mbnxyals.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wmturljp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnscduuu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2bsvdppao.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ueoghjpc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iagtwqne.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rjnjjchg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kczldros.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tkpjtagf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lccipkpl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jyynqoce.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2agplljbi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2efsvyrwk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ekewuyds.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2dtrmfszs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2moazebzx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mifzawqa.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uexgougq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aesqunda.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bhtlejat.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ssrbnodu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rbrgemlg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2udpkemmy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kuybvcgk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qzhevkfq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2aeomomvt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iqwxgxdm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2owjbyqdf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dzpcahex.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pvuncsyh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xggpkvds.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2czzkywke.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hrvkncvv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kqfjktot.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jozzksvt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bcgptdpn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gmgroqao.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zchbwsxi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fdzckdpb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xjxwgkec.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hsltpchs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2isubjheh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yizqsrvi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2updeighu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ubdhnwkr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfocvqch.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2coadruup.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2lpopqver.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kpdxkmka.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2biwqnmnq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vgquqdgq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vobvfosf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwlrufui.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhtguinv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lymhnrny.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nirrpzwk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gxwcejof.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2enpumzkq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sirojraj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mbosyndk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mrklwlcy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vvniodtn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2twwlmrxb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qqpwplmf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oeprcawm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qqrajuoo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bsacddfc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zrtmrllr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vapntgzm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kctrryyt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2loibvwwg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bevpsgyg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ovivclch.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2yptbreck.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjxserkh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjtoutan.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hstvuhqm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2umcpotoc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2suhsdflh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fdngoqrb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ihinsede.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2clafxnbq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vzlxhcdd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ltxmicjo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dgheecdc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qlkueotp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2znycopca.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ztsrcxrk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qiwjplbq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2flgqgxfs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2adcxmhnb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ruuqauam.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2okcoxvbj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ssjqrtde.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2eixbblar.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tacpjugj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dwxdlzfu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cjmlzkfl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2motdxckm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lwoiwhsu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rtymjpxs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rtczlxwi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tmgpfkyh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2awkoxjii.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2teuosfth.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hhtokcyj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mclgpery.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uvaqizen.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qtzlnier.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2imlzrtvt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vuinetml.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kvyjpnrr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tfmvcakh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ukcygziw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qusdxupw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kabmxxxg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpzsxfdc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkweaaxv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mrlkngxc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2utajeogc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zoghglhl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awescjkt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cxlbnsza.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ytiyasxp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zdvcnnmi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uinpflyb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wxksykav.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qqnchkow.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xyqvpexo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bhupgwie.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xeizfcxp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2jhhyxcsb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2flpxctpk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2feedfeaa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xbyupbzg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bxkwcmcc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lrgjhmoz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ajibbiaj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iirkinln.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wnpqcdcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuzyoibx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2unvrhvzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcojbnir.html


<!-- 参考信息 -->