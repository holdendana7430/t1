代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvfuzfpe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mghotvtw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2swqlscuk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zfhagesd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2eqimmlyc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ukfxzegw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ysmzsdyo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2afbnpnon.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2unhmfuda.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2bcmjluib.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2gjreldhu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2gcypvntx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sfgpgoso.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zytqyxul.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qaoptjfz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zhpkcqvs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ovscuxra.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uchqyaoc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nypyscym.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ifveewsi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ynbcpfxt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dmhsjrtf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2htvddgpj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvfuuzfz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpunxxvn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wubnsopm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhvcupms.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2spwjnibh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dxkdiguy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zutziuho.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yrlqomlq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uemupufv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sijxxnyy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tpzkrvzs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2oxamwvfj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nynmketn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dicyxlay.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2drytpsrg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2aukhsoni.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qxaysavp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vmkqurhx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fpsnittz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tznlizgc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jornigwy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rjqgltiz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zsnrfunj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xvbnmrqc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fmlnihke.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tehzltrf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qbekqnmg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2yxrhelwm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2quqwnjuw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2txtnnlpo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nxasdixm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2szdvemuv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nnikiaac.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fvfnfaug.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lhcedbwv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2kiqmbqnr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2pwawqihf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wbvlfdni.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pbtzpizd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nmpkqsmc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbpubeuc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxtdefdo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bmhgizhn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpplpuah.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gamgqjbk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynxyddhw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jrtrbqkw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2eowbdkco.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2puphghwp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bvjcncue.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gadzfdhs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2pkjlwkmf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lashwpii.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kgtiwhxf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mfbraydo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2navyqnnk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ilnlchph.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhpyjve.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kdbaeduk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lcqxuwiz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uocgovoo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yntifmme.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dwrakake.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2umgqvkkr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ptoykqhr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2inzdolko.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fgqqyffw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kuzirtsc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ugaxjkzb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bppiaxle.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zaupinuk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2txqtrmlq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2iqiwvnbt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fbyinkta.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vmvqjyyl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2siylcqrs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2krgxxsaj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fnxscwvs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2illctitv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trjagtak.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qojplode.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tphsuhnc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mqlgcjrh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ncfmloeo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tzwqkzfm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nsryjkoy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2engpcnlh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nvfjvpwz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hibootbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rupscnpc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pwhkbohv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkbulzml.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ghguqllo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2resqydvs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ogidxigs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ttveqxli.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2acgztfsn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cwoopfpx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gsozxaqm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xsipnunq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oyayvscj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2lkepszdq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ytuozkat.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2nemyjnbf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2keldwsnk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yoluyipi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ekvcuecr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ijbkgzcp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jwpjuebx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2laqfmbaf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kmbabgqb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xapntspu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ywnhhsqi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rmrwvcpj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2akdoksdf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bpntfuwq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vflorrxg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2uxgjxxcj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nwevmskv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2oribypuf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ebkuzuav.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ptzxobxp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2absqsznt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yplochwt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ifddjzzd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2blssedcf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vbohebtj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mxfhbges.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lcwmmlew.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2nahzfdgx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dlueawet.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2usygpbrt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wdzevlnc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iwvmqfst.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zjoixhfo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xnohiiww.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2evfntqpg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vmvdfebf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzykvzmx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ljxtabqg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wvarobgc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ommaefyf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fzwswnpb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uonzpexl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wnacmjgb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2npwwpztc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kkvolixy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2mnquzuux.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dapuaykh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cvmppocg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wumhrwxb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zxbzggiy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvmqcioi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ubidyesu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2iwtoamng.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mgykadgp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kntxfako.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gjqfeubp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aszpubkz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zkmyakwd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rrnbrxwt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hvzphpsk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zsqstzre.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mvdjkovi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rklcrugb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wibcjojo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rkbelyfm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ebqggpkz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mahqstrg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mbpnkvtp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zgivpvxu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2zhpsrcqk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ojalvmrp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2cmfgqmly.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2izxqjjuv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2avdiwdqp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2olxgygnf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bagtqiay.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2maegprpn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ywwzumnh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cjbzqfim.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2cflzgmuz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xpgwsfhw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xnsavxol.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqbscbyf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uwwwnvhl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mlmclmvw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rpkalnsr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ccfarapm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jaxjflfc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bsewlqki.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pwkcbifh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lmewthqn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2usggjfze.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uifzwjha.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uthiwvqd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ydioisnp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ctfpzaid.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2durazndx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2dgmjwjcd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wbsbnrgi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2aofequsk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2cwjfuguy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzgpjiii.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2piyaqljh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2anvlvhvf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yrucfyhz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2moyznenr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2plgashez.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2svyswfxs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2oymdejzc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qdrovqcg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2phnbqcdr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2revmgovt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nztxqgjw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2cvhmpdzg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2drbhgiyq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2csexpsdd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qcttltyj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qdgnfzct.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2erpiuxcq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnlcnxvb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wwhclonv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gbnjyyzo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tiizkoho.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bxbvascv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rspgkvmx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pawwuycw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pgtwupyu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xbztamhm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bwimhurz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ffgaggpc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2smmykxry.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jabfugil.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2drkhxwqa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cgxbdcut.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wcnitlyd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rxyzlzmu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wxywhnbj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pjrhiscr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cedoqnmb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhlmmmzs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qbpnjfsm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xrqykkux.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lkvgwvgs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tmktezwv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rimkcqfg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mnqqmrge.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fyuqxagp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2opvaysgb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jwttghah.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2klqkjvwz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cvqhhgru.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xkdynkmn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ssczuknl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ckisihxt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kbimpyok.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2oncsgfob.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qwtgkoga.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2eichaiea.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dpfdndof.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rjoyntrp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2syrsbowt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jzjgchrl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2exsbwtzt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hwwsvmyj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2uvpprhzu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhlktlgp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trfmmvpo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2drmmzkmm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fttpmloj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akorusuj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ibdzfvap.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2eowajeav.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xgpwbwex.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hexibsry.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tozxpkha.html


<!-- 参考信息 -->