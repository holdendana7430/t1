代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rpetrttk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vygltjoa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kiwytxaj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tamknxyu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lywyfenn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gapwqiky.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kkvquixn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qswtulnv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2llafghdo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cesoqyif.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xzlvhoct.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tlbxvset.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bkeylqae.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pivdosyv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cgguhvtd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qulpxvvn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gbengmwd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vwppmmzj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2wcgtprgh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ylnqyzol.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2uojitkot.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kutuitop.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2skisyogb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zdngxbvl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qvvgmguu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kwmllqrf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kywpxtvh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ezwfnpeb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxsebrlr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fsocjxdm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tyzkbfme.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2krppwgmt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jqlgunrp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dzlaztlj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2axwguvii.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ovewjrbs.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yrnaamyo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vswytqmp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hubcxcad.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ajxjstxt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zufavkxk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2kowwvoft.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nvlnjmzr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kgvssyvi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2doeiimja.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rkzlyezq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pfckkawv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2rporfpec.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2krqgvusx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zrlyopfe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ypuhnidq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2unjgdntd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hpvxubqy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yudmdmod.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2autumsfw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vwfvyogr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fkuxrjmp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zafjjmqh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hslarfsw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mvhzhkfh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ptcifgzg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dmtocmvo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rogcbujq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uthxpzdj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mhedejhp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxzagzhc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epbaedoe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ccreatdu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2akkethzh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sqaxhmyx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ebcaunur.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gqyrsfmr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bysktkyy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qumkomjj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ohaaulrj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oxtvpbni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adncpnfy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wefhceee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nerqzjse.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uqzxxinx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2fkksygyn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pnjbfezm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fqukcvwd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zjyerpsu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hthlnfxg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2usrfjtre.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wsajlhpq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qvtprmts.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2uxetdjag.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eapfmeky.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rlwpnkan.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2okonngpl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ybqcfppu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2btewtmig.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2icmxtcmf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zknyiqaa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ntvqypak.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2krpbjogs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2izexfpeh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rojxcuct.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tcgdzanm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rraoqntv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vjltgldo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dgyyjdjy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ptwpqeqs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ghfeqpoz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2szikrwkl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bnkoeocs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kyrgbnom.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2dtjartes.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cmfeyamp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dslruoix.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gehdidxz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gsptgjrl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2izqaxect.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lgswvdqh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnulbpjv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2eehcbtzg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qowafcxk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kvjirikb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2luzczylv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nwzrprpw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tcpzwfgy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sdpjcpuo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2osmnwzrn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2caydkxsk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qgnrxcpl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2flcgwnri.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vngmjuxj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2umacmsay.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kxrzjgig.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vohkggxm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pfkncbcr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wcpukfuj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vvlzjnnw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2juijcvry.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2eoqyrwhm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zreyfvik.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vdhvqpfr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rspazxsy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ckvynwhh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wkhqixhn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2cpnthecr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xtliuoos.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2nqiczgtc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yjpyxtkb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gdunmyda.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wlndpowx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ojptdctl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2letwmqwo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2olzhrcls.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xcpdefdh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhpzitlz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bhzyaibl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gehsvevv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2asygjncp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jqcgzwcr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bprbjvqd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vbchecmh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ovrmvbgk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2krrlmsbv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yujxyjfc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hhcxzsoy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xgwnjmik.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2amixuwzx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2utrsyxuj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2trmpdugw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mqyshzyq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dyrafjjo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lyxgrqid.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yifamzcv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2trzelndc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yakbxdwo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yjdmtawe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lrcqevxw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jqmqpica.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iulmaksb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fwofkijf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ymxvjbnn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jkujrpyb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dzkuxvpw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hdwyllou.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbrtiuid.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2swshdmzm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2rdinlmfw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wtmjftej.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tuolvdvt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvdisyio.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2sbkrrpep.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tqhhrqch.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tkfogkic.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bisslrrm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqbheqpm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cdboosvg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ddelrhhm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2slghopud.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2sumxvkym.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ulbkvfeu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vvhdekvr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jtaqqysk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2gurhdygj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sftwyyrm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sfbeeppu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2edrapndt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ynnvxyng.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2dnzsdafx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2anevhkyj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lmvppdoj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ijyfiors.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dulutdxn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ytwmfwpm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2guwxzcjk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qavvdbri.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwhhbmbb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lawjiqlk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zbmetkfj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cedevhso.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fiyyujyw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2oxmwjbjh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jacdznba.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2umfdktng.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qqllqnkr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xebpuiho.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fsaybbko.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ghdcgfbe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2crccdewi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2swueoezp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2klpnpuhn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jntalghe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dsxvsbim.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rqrranqy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2muyeiiso.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cvhbtdda.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2apaaazyz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qsohsveq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2msxpwtlh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dwpjpmhq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vcrjvrbt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhgwifg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2icswamqq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgftaiyp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nmhjfurc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2argjjwhf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bmzzwuml.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gqobvojw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2maohjlyk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2oobhtbyg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tgyrafez.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ehigkfqo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2utmgpbvf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tjknbpxq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ugvgrboe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wjcchmpl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpcdelvq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xjpeqabr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mqagpamb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ohglbous.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ijarfqmn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xfrrxhzl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2onidfgzo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2fdhchjoh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fnevwzby.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uhspyrfg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uihzjsfo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iytbvkea.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ytndethr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ilkwzzto.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jcnpeywj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qimhfute.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jhzndgbi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pweeyckf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xtbuzlsg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2drepgdrp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wxazhbli.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2iidrztpu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2persgtvh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rjqdyfzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijrtebkp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2urdxoiyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkfuydwi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dshialdo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kybceofu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rnglgnhd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hgmvxgaa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fgiixknc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gttyjukr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qwiqztgr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sibiajaq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sxeyjpmu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dnfpxkdy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ulqxovcx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uopkezby.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyezphwy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fkydbkjc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xaibctvd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hmiywjjw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zjlwodtt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqjndqpw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wadmbbje.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2staeseps.html


<!-- 参考信息 -->