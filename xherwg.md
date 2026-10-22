代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjmokjn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2eujlirww.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rpuozbij.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ynfpdgvs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2alugqnty.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2uyynpspa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2adxqzkdf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2skvxuaux.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uivpxbni.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zfxlngqq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vjimszzg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tgvjzuxu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2uunaicew.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2txspqmag.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2igrmnsto.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dszfxxni.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wahhlpye.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ydyabuzt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bbygyltt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2cvkidwvf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uwrdmabx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2tcwkccrz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2enugiqug.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2chvxssty.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wdvjofaf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bqemcdsg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tqmtmnhs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lbnbaevq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rakuxcmh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ygbkxpvg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zznchxlq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tztcfrup.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hyxkvvsc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpynehps.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfoqyxnr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lkctkkjv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhstmaru.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnqgiszc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjykdhcc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2umincyxd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tnpdipjs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vlzkchmn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lqrhoyqi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2uhtfdmms.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xnxpnxcf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ubyqomir.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dysvluqg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kpvtchiv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2eibyoezb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wvdmvkwy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iooxkuka.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jngevbwv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mjxqqofi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zivtjizj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ujktjhko.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rihtiqku.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2apubzkrd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nlhoyjra.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2coxwrcqx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xriimlia.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pvnzzazn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bpxotwfe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yrmjjodo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fmggckhz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xgtrmlxi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gsltncjs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2oqskfway.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2aahteqix.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kkrjtnpl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ukiidzfq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ohgolgja.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mazjqffn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hffaoeoa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dsslodkk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bhqhmycx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2meqbigmx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pzpczimx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ytezjqqz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ckdfqjos.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fcqcydih.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2osdhywzw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2brobnjeo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2duzskgig.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2okufprqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjryfxwu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2vzqgednb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iimprkua.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2szznasik.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sltufxkc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xniavlzb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ilzulmnw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dwxtiulo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fiejqlcu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dyzjffuu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2uuaxpryw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2btqgnpoc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gqbwxurl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ohuaqkuv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iwetkyug.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gevfcurs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fkvazbwq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xuqjznsb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nqlfklhf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jtwvplds.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2inchugyg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ihahvymr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pwjohmfi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oqhvdhqc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nlyffrcc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wkqtsngb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kwwmbald.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ewrowzhi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tbqkaqbc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rypcxqzf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2quniituc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xcheibnz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jplfpzqk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ghoyplck.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xlmnqcig.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2crmvmhvw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2klzmneyc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zizhvgzc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yaioitzc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hupyvtks.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ijhlxanh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2riuxarkd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pcwfgccy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vlmwtqph.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ftmqvqiy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lxkepxia.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oqrvzecb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2srqhxuwr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2azallagf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ponegfjy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hvkbnarx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dnatkfxy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dqugjcmt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jmtwcfvv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vgokmfrh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hiuqqmsx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2exnrhaoo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kvynnhnw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rojkwwnm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2twapdixx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bquoxfvp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jmrollsd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lxkxcdxc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2oeeknwwu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gsrxtkoz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2oqjntflz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pmsmtavu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ayfbptcw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gqdhbiqt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bqcvpqqs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2smhwdgfh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tzdgbqbn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2pjmasaxf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yujcjazj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tzosuonc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gsfcxauq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvyyswcr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2omukgajt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2coqnzewi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cfllkqst.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jrpkcbui.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wysqdesh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wlgexgcw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xcfhofvh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ekynjmgg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2imsdgswf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xytahdpi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yjhxoomy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mhblqqam.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kekpipys.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2elcxoiat.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2trhthdgu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2iyffqjyv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ispizbus.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hvengvxu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pawzoayw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2racjirek.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xxdsnsvs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ilnmzfgp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wgabbhiu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fciibtyv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rokcyhgl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pjraokfc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qbqvevbs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kdysqsvl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2thgfeyfp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dedkpwls.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cibpyhmf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2owyopvcf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2acrwosit.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tkywwoff.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2smuvaoez.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ckrhxhxb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vevrvnph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rgsjnmvs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmbdkglj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lksvmvkp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jgkkuxdj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nooatnju.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2swnribom.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ydfowajw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2uheqqdfe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gmepuslq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hdttdqnb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ycghwqqh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kzrdiauk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jektvwke.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ohjfkoog.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ajxgpvmr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vzoxuhpi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2tsesygji.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rabcjcto.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmczczbl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2anwmrfqd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hghcpfbx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvuacxyk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzrgzuve.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cgiswsfz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2myxrhukr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pphauyko.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yvllocjf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2owrxxwet.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kxdfnmnn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gjeptbee.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2onyeirus.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mioaczwg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fufpwkve.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xxkcrzge.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2snoxkwjg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwzlsonr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ewjgjpla.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqakkoak.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2sijyvfzr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2srecjwrd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sischlyf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2walhzwcj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kxlgmttd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jdymsisk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wzqfsuwm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2crtedcmh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bkiwrccw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wbvcmpzy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gaqtfjcc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wjmqvmgj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2mgzqmihg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gjgsseuc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wuovfgnr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fdudnooi.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mmrvxxlp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gopljcaa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zxrswsjk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xfnsdlxi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wjijptjt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2nwhbvsdy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gkudgjlf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ihimlowv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dqlxtiah.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ayvzgxho.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2drydhqyy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mopynkur.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbftlyxf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zatcerhv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ispfxuhw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fxsilxkl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mxhfrzec.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xkwazake.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mkljzaqz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rnannvyk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nwskmsqr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ssucudwp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2animbgkf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gdubrkpx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2orcrjrle.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkjvqevg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hzfzxhbu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sespcevl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2thqvhhco.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2deurvsgb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gronizpn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vjtkdygo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xmdakfrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdrlzxkm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hyyqnbzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfptjjzb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2robsltfo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bykpdwco.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qvxorvjt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gibgtwxv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kuasenif.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2odfwicpc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uhaqsdyw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aboujqgm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hztncyjm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kguqmytl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hjxhediq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2htenabfd.html


<!-- 参考信息 -->