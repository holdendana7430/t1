代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/guxpenpny.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/goxsfzenc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gflqqbjfz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gmpvumxlk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gwbesrjrz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gzjgmlpvo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gzptsndlc.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gvvnjvxnf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gfktakvqw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/grsmnjqkf.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gleexvtyv.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gmoxyobox.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/goroiyugz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gkagzodxj.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/glhqsozxa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gsvsgefvt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gmixidvfv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ghzmgiisf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gpiehatpt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gxpqgmstj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/guzpbtyfc.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gubdfnizu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gujpskfoy.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gqcvrceye.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/giuuervpa.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gmwaimhmq.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/goudqiscy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gldrekefa.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gxndjmflp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gwjqbkgqg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/ghgyxcmug.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/goliubmlc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/ghdkkwlco.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gzgmgoywa.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gxgbwnmpk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gzffofzdi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gxtvezwiu.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/glfwkuqvu.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gsjenmfkk.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gthuehsov.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gijxjunoz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/ggfgcunyj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/glgrwolsb.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gfifcmhgw.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gzaltqctc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gvscyoefn.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gnycmersa.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gcocwqvth.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gfkzzfzht.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gdchtxyds.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gguddfubw.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gforpccnt.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gonfcbtzm.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gjnooskii.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gulagkhsc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gldyauqqj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtdzfnuhz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gakxprkeu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gyyjgbcjj.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/ghcttczgi.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgiksxn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/giasfmifw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gydnsytdy.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/groqngsnh.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gvezvuftg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gwuqallwy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/glffzkmub.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpqsqivgr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gdlhwgcjk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gcdukpzwz.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/grbcxudqk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/ghorkllct.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/ggfokolls.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gfrxzezkt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gyynttbld.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gqxznjxfr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwycxtre.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmvrmeyjh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gxwdfslkf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gshgrizua.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gqcbpcnft.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gulbqifku.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/ghafgmaob.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gjzfowrjv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gypcwrksg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxksimkle.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gxcbitjcy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqfbziwfz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gwtgxdwdr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gsscvetxz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gxnexkwba.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnsaapffj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gfrqrvfkq.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gifcgvtjt.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gyktsisia.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gikxprwpf.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gnrbgryrr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gxsvixoxz.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/guscdsxgb.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gcicpsznm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnycupswu.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gxpnjpuzr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glhujnkow.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gfhbaxcud.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/guzdpnead.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gnjgjtehs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gragxqbar.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gwzxojvcd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gocupkmee.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gewxujmgp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/glicecnqx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gsyterrls.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gtpxwgeae.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gjeoqtbvc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gwfgsskai.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gjmofclkw.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gduhrijsa.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gstuqvhqd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gflkuadpo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gfzzlqxze.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gfbsbbttk.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gumagkzxb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/ggcyjqmbk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gzhjyceka.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gjigrczhj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gsjqzwdkr.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gighfxiqw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gzjkcjjln.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gnvcububh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmyhrbfmi.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gpmiezjop.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gbwgqgitl.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gdxjffazk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gwbwgbpqn.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gwqycndwq.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gmicvvpkh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/glqpjcpen.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gcqrhzyef.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/geooygdou.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gdnwgkvep.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gqxudwpxd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/grzgsamxt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gnhvvprfl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gjgfaimew.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/guogiwrrq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gvaumxqoe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gdlmsrooe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gzmbutznm.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gmcsusial.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gqubgmevi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/ggkbgsvzm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvptqrcaj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtrcnoljh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gcdxpaooa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gdyvhxvdv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdckzqftu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmjobiubj.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/grerkvous.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/ghlzkchkz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gihsnibdp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gulvjmdin.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/ggpbwsteh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gsughqrwn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/glyeeptft.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gmxcvendg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gurfdxmji.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gxkcpkwrz.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gflteperl.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/ggrgvhhgf.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gooigyhna.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/grqlnvbxf.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gdrfarhqe.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gymulzgjj.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/genroiybz.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gyhugkmte.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gyjhgyhtn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gwgfjklri.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqlfgrxyf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gdmrtdjgq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gklrpdmwk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/guhdxdoaa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/guqneigzp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/ggwfsokmu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gmdfdaaql.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gfcrvrguu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggaugdjun.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gjaajrzjp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtcmnhlb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gexjkyahj.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/guqurcbha.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gekhiozhw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gvbrglgtd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gzqngthej.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gzkbeytuz.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gkptqdivz.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gmcbzkpns.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gzfvzhtfe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gtypijksx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtbzdmteh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gkcxqptqg.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gvbvybxoy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gdctizjlk.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gcawawuqi.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gpuussuet.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gwdaqcrbr.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/garjpyamf.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gnkmhkhgc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gwkkzpqan.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gdclttadd.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gvgrlrrgb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gbqjoiqkf.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gjycohurm.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/ghooidhcm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/galhlxuqu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gidpaumor.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gskzhmwey.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gzivdscgb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbxdgvgaw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/guvpawbyy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gkauqhsxv.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gsxxslfez.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gytvzkksl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gvgrmrnnl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/glirsvjxv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/guxkrikmg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gipkyrjui.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gyilixwxt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gvlrgbsck.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/guhyrczcx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gzerlmuzp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/grggxckhg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gzlntshkr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gmcsafzpt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gtdqlsplb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gvnpkwsiv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gsrdctnjj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gycxandbz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gazqixhgh.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gbshzjsvy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gtryxqsur.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gbmufrbti.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gsfrchrcz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghkczouim.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gajnhifyg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gdlzklqkh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gofdsdsrw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gsjswlynr.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gtqnwansn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/ghfuiikvj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gnftiwlla.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gttfgqdre.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gthowehkk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/glvyqfyhw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gesqripka.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gwjhhtisb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gicogfeqx.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gckmyybjn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/ghcpbfwkx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gmpjeeuqr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gbsesggpt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gwfitnjbk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gsmuzfjwd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gbsuojrsf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gxrvyspgp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gzejwpudt.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/grvcizdus.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gpxuirlnl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gmdaotoes.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gmueabmkn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gikvjaozh.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gnglpqwcc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwazkokhr.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/ghjxzbcqd.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gjfjiuysm.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gesbxkfvn.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gigeoxyoc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gyzneoqmh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/grinkkddv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gjylogsqc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gojrvdkbv.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gqplvprth.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gdoqczxsq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gkwvozlof.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/ghjenyufi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gimwyggzv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdcppvzzh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gzedorsnr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ghcdsvius.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/goxzvcody.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gbodkethp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvxewztkd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gwtzcjocw.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gphekblmg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gejuhwuoq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gyutymfui.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gjnuvguoz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/grwlhpsdg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gddfrohom.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gqquevjgd.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/ghtdwydbo.sHtML


<!-- 参考信息 -->