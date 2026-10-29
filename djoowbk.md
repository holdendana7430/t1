代发 wailian999

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gwdybgrmq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gbwfpyhsk.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpddtyzpw.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmmxgmg.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/goohqzwcx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gcwykurne.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gxmsmnvcr.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/grjiribxk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggiysgtbm.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/glchfnbjh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggsowlbqb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gzvcsiwhq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gaklxvstk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gpomelnen.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gyvfldgmr.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gbseknkis.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/ghprqkjfa.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gaiodiueq.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gijlpcpyj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gemreynia.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gxopvcgkp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gsucnezqn.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gscfnvarh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gmogwqhzu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/ggrsnwwjm.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/ghixvrpaw.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gqkbaqmkb.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gkqwdastr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gdpnhfnwk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gtuollfcu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gfgwyjtgh.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gdwteeteh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gagqeqyji.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gfdemzskg.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gqmyunmkm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gwiihorkx.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gywivoxrt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gbahvdkkr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/glnkjdyhl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gzqfwkwzk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gkcslraln.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gkxwelulz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/ghidxomcf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/ghmoyiaji.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gsvzjclcx.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/ghltxxspp.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gtbwldmkx.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gurzlbchf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gnknpwrfl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gytdoffeb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gzyjvifkd.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gpadqivlx.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/galfoqjdt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gkydmvyll.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gkagswjrr.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/ghjmhqcuk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/guspxvssa.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gcawsfokt.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gbwjiigir.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gjzkpqqjg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gixqxewuu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gegqraguh.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gdzyktvji.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/ghdwbxmzi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gwinbwoau.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/grlfmqcrp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gifvjflkg.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gdjvejcid.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gjzihqhsm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gxbsflmwg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gdloxfcfp.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gveehkvuu.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpjmadn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxiztnrvr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gqalzhuwb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gcttiimwd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/goomkhpsq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gbowvzmhz.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gomgdiisz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gmsgcblau.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gekfhkdkr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gxsbhprkv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/ggtwjxgiw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/ggeimzrno.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gpotasyes.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/glrcwgjiq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/ghoewxnfe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gxozqiydr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gxeaxmcov.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gifzudohl.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gwzcdxknb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gggrfourg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/ghzfgibqm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gvyxvbuwc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/grsdbwgji.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gpeapajuv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gvnbbvzbz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/geiphhfqv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gczwdmvjx.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/guwadzsrj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gajjnxsiw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gdpfbkwhe.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/grumgapwy.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gfealijwd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gizcjojel.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gytqzlqzf.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gahdglusn.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/goddmaimu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjzkvnzon.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gdqcibflp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqnrfewwy.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gbokzhvsn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/goybvezqn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/ghpeknahs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gijsatbsh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gxysqvyql.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggsilwpai.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/goelsmnyh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/galgxqbxf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gmghuzmea.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gvvfqrvpf.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gksjwpaso.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gacyzpkcy.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gnwajwyzc.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gmlxnxeio.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gnremuftc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gyljnhiqc.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gzjhlgjkm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gjnjlixop.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gittvqapb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gvgbrzcib.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/guiyoeyud.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gsftfaspk.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/ghuxxmsgx.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gkfobxzsg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gjuffffrx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gigdtduyy.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/geghxmluj.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gjoyelgmh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gbrwvxsns.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gsawdjatf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gyaitpcmx.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gpryyyjpu.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gzorcqyhn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gmxpxvvkn.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvkecbxao.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gxbzbewwi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gsvavrjsy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/ghtwbskam.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/ghhlyadpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gmkrydhyj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gcqfxiprg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/glwrfxkci.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/grrtdfvoh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gshvlrcok.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/grswoogqf.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gtidbwvfe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gjltncdti.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gkglpuqhl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkleskfqu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdqwtbixk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gzixxjcgs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gfzjeimqh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gurwmsvnm.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gnyttwcrc.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gqxvrybwh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gzirsdjck.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gwakysbju.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gfqsbrvce.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/ggxrfvkeu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gcnpqbifl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvwtgflju.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gjlijiaqp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gbebcfsxx.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gvxlmwcre.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gjyicaidh.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gblbsiyhb.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gewohefpd.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gygmhdpuu.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gbsnfbncp.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gyymzfhqs.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gkzbkzakk.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/grzbtopyu.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gxnjyehri.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gccuurvje.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gvhuqmvwf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gkyqrbjew.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gfzvwmtor.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gvdalczgk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gnicidooj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gpsktgfbv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gmfsuszzs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gjcwizxgq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmbrfvaks.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gdautphrl.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gfgyuiwny.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gesqmshkd.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmpkblqhj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/godjwfhmy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gfdwlatml.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gqspfcfwj.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gzbrpuhvu.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gxkjmrujy.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gkhqyshem.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gjryewnem.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gcljvzcch.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gifrdepfv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gaqplzoyt.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/glxagslsh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gvtrgvfta.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gchcjkwrk.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gywrqzynq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/ganmnhznl.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gcaufkeyl.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gnopzlhxq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gvrwxryli.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gphocyaui.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gxrzzllgw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gqjqcdenu.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gxoreksmi.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/ghwnqpqbo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gxkvdeqll.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gnrjwrzmf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gclwhyzkp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gxwffrijo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gcbgmfjkh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gcethgdzs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/guiqhwmrf.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gjhzuqimk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gnbywjgmm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gulnmytro.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gfqhbbael.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gzbyrejwh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ghetbgzbn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gpvxgslon.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gtxtwhrjp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gliefezzd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gnheeiifg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gjnpknsfa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxltycmga.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/grjgqqhfm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ggtvkukeq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/glauzaiyu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gmwnszkbv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gzupmuoxx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtvnkzdxu.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gejgnsjuy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/grzbjnbtt.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gvyreyavn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gjlhaurie.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gaxtxrxxs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gqcwyqyxh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gmbbiypqp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gfvfyseqc.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gwpyqchiq.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/guefvqkng.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/godsgaucp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/golrydnfn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gevrvfxfp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gaivwoieg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gupuwbtrn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/ghjnpxvij.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gbqhrrdxy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gzmimgzvw.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gzqjqciki.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gcvuabnzn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gsdxauwyx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gkxtteoqt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/guazupver.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gvtwoysyu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/giolxmnqj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gmstejwva.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gijdcdksx.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gqxrvxmhk.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gdzzmcgdg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gbrjcriau.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gvigsyobx.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gfdudjaoh.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gukmfcrmt.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gfvthzgum.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gztscbkei.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/ghizsxuip.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/ghtferkxr.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/ggscaldcc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gnnvbnmrp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gecdubqnq.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/glkhbibkz.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gnhpmnueo.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gxrtgxfkn.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gawxplphq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gsessuwap.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/glpczwvoq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gdrlrbita.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gacdokvax.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdpfjnfms.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjmvmwmgn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnptfpeiy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/ggamcccpk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwvacagpj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gkupletdu.sHtML


<!-- 参考信息 -->