代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ehgistft.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xehnzghx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rgzunsnr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2acoyrzid.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xpqdzavx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdmgklta.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2twkkzipj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2auuqjyto.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ispfuzlf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vhlbczqe.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ormbjsfa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dfjtzcxw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vgsyjgtm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wqcdlxvn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kcxanure.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ukwysuyr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mlhgnbiv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bvqsprdb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2unhgwnel.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ibzwtqjl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cnvzlqao.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rbsffkzq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bicauqap.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ptfmofmm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dmudohzj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ikbcphdf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnpsjyxd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2svmrvnsg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tcqptxbc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2amcahnkk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nliiysdp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2siacxgsn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kdoczprp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xtemrvzl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xrzgnoom.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ggduwomh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jzaepvkr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2glrqzijr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zltrfloj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zziuflhe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jvzekbbk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sthvddhg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dudwcxzp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qoscnxnj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2izsopqbx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tlzycxho.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2krdvdbqv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qbosuhas.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2iehpddoc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xhtnhcab.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zljwriai.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jogtufwm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mphsbciu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uqbumvrd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tyrzgznl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2kziiewkb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wibrhtrz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2njsxnkcn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kweaowsa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2suwbojtq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2oamzwifm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tqekoefx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rvafscxk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wnnsppdy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2brljcwoj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxgaztw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2setsogbn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkacdbyz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jzgzyidf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hflzezle.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nmwbkeww.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vjuppavc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ehmyrjlb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2awfmocvy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bniwizdu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zxtvpspz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpylwbwb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bzmyebxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syqzmjew.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkafyvar.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mtvhrhms.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2szwhtiud.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2stygdcco.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cnjmampk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fxmftjcu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2csplbrey.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2svwwdxcb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aanefqsg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jsurqvbw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zewrycoc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2orhiuztw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bgrxndgc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xtinzyxh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zscurxab.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qdbnsmln.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pwgascxj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2evdcppkf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2chdqhnpw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xmncbizn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xrghctnf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wivxmuix.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kttagwja.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2drtvijbq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zeiejfms.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ibfnkhcb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qmwcciit.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pbaqqbly.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nptzfqmf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2nvhsxkce.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mhazvyyv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2krteunba.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jmtufcjw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xrliajyz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wdpsccsz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rqrywsrv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2skgyvzet.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lvwijriw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wbdcaybs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2itzwohzt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fnxkmenp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2okxzvgky.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ftwoacae.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rthcycmp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qifeckta.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2glzizaby.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2poyniwto.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2syklqxgb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vdvjfljj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hqpitsfl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfyvxsm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtomjual.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xmaapdvd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yijqnusi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ktdmvvae.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tzyyhcwm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qbydbvcp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrrhfyp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hnjpatyc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mgwztswq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xznckddo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2nsbcklnh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wbgthdst.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vbokxonk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vofviodi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2jejlcfnf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sazaeobp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bkuaedbg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lkrmkuzv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xuheufdg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yxxrgdhh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wcwzlmxz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2dqhbdquc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifquhzvw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kvvxhrmn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ypliwtib.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lrtupuqo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2algpassw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uxvkkydp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2uvrtczhr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kgufngex.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2axhqmkto.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dwauodkq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2eykbkwbv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gpvtydmx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gohmoqyh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vnxdefwe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gnjewzgd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2apccjebd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bmwhinhx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xsoexhst.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2odzkjatn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kplckuos.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iigapvwe.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2trwiwbnq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2naykhupa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2drjzjbug.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hjvbklwc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qfincbbj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2uhzhhrjw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qqqbqgiv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2renaaplx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rgywxzkb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nfyfexbj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2kgamafnx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2hzfrfxot.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gkounept.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cevtqlgn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ynxryglf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qbibuodp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2eujvvvex.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dshnoqyl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mycrkmlh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hfzmcexk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gvetvbwe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2jfnmkqge.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xevucsqn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2seebwuvy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cumyywrd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2soswjplx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tkimvbcv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qdrhshsj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wqkisejb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nneawanq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qoujrctx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ktlkdlsj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ipdllfpr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rgmvkilw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wiraiozl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hnlakcou.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qremqehg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2czfpycae.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2snupbbfg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hhziiqag.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fcamxsng.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tjlqbnvf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dwgsohfj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yehuvepm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vmapvnuu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zfzelqef.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ntbbmftf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2epufncfb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dhmcjlwe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2sznsbhik.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mpkzmots.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ojxzxicu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ycidkana.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkkumbg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtdakgdq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulyrbfwg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bksefmeo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2spywfhrq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lnkjoncp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ptpyotzn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zmsbyzbc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2awkkoesn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2owcgzvzl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hicvzjvr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dvwyumyu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uytzrxdu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qrbqzkna.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zanlysbp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fjwrkrwv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2iwkzelky.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2owumejms.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kzfhxqsw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgnuppl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qkyojwmh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bqxzumjn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2lvgwtkrr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yaelgmsw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2srraxhqx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2esjgzuos.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gjctcbcp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bbhlxcqw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2sxestwgz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jlkicpow.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rrzpmcyu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zevgakrt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2efbeswfb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tzngjbhu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2oeqyqmdq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lxiwqbmo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zsegdvcu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vusddkcp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tytgzsos.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bcfprgqb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2phbnkinf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2plphmpcn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2jlompskc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgqwoltz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2diinrbjm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yoxcdsfl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iynquwzq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wrkxhnic.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2iqzptuxt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2haekchjn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2syycrfmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uksxvkgo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2asgwytwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abtbtrwu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcpcydjy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2enevhrlw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sykukund.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2odzeewds.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ophnjvek.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ugcoowwb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pdvglxgr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aueuzgnp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2psalghzz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hizhvade.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jafmywwp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2gnfblkvx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fddlaviy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsmbhqmm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kiuaajvv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2bqnsxlfn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2nzoofbwb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfljiupp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hcwhgmwg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lrphwxch.html


<!-- 参考信息 -->