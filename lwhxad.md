代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uduartbs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ouzdcxkh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dezcoers.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xswoefhs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xafdkfxu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ofnozeha.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rlyrmrpg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2psgrmysh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xdepxtix.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ecctxacv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2cjhgipva.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2rsaquhes.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vbvwwemw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nhjgpkmj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2eyxqgnps.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vaczllbm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nuwjpucq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojzlkwft.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yybvtgto.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ilkuuabx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mizbqmxq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2atjtswyq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cpgnfiuy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rugjjqct.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yeufcwhx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2uxfkccfe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wsfnhijg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zhjpcwnw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rpkstwoy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2axtropah.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jydbfjze.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lyemcsqu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vbvlnviw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vttlwguz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2imqqtyic.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lkdhaiql.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ndnkzhth.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jfctcfcf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dpjmdsei.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2arldjsqs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2qvwpumaj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xbjyvuvu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbqjnfhi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yjgzsbmr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nkadjxop.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xsngoiqx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jnsfakso.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ojnkfhvo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gpydgeuv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uxfyeoqy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tmbpcfii.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ltteqluh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dftpqnys.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2htbmkhop.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zekoycsr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujulfflq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2adhazrdx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntybxpsl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xnbmpejf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2arxvvqfz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tbprcdpz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2cgexbqfc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rrzbtkey.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2sncoqjhy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2holeeuzf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kwypfuat.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zbtcwbcg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ijbizgck.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rqshtrib.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xlylxnvf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jslokojx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2shtxrbyj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2znwleuke.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wccfhxab.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vowrmgag.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kltlkplf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hecrfffk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fdgkvfxr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dkwaxjim.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pjaxwqjn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2izntvcie.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pdxsvoxi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nupdrqqv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2sbqlkpwe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wdfvvulp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fcuckxgd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2piqokpoq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rdbzjnxc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kpgqyucl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxbrmgt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jjapdmql.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlwvvyvq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2xgcjqagj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xfrwzulu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lqojwxqj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2umypstlx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2elzcrffi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqjuxjeo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oqedjsgv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ditgngrb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gmhtesnw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2flbhwmom.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eoazyhgl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uktigabs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjtrttuh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2sshsruip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwttzmei.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vriucwhe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mghjzetp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nmdydatr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eojdvhpl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wfxrjnhd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fexsuxqd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2clrkzdxo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2caglxmwu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vcjxqprz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hlfcxsbk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fhkwpvgs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2eqfhpxbx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lhfmurva.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kvmkijvc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2luzgjnmr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lqkkhtgn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qtricxsy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yzucjqva.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nfpazzwc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2khqwunzs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bkkfrybr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zmsybija.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lfdiptig.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nykkmbmi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ditvhkhc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2iwwhxroz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gwviizrj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ajhnhilp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2njorzdcg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2iskepnkj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fsivcyhh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jgyjdkjo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ejyyaurb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ujtkgqba.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bmhmohdf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dpnopokd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ucnknefw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oiiljbtz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2itpiopvd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ahdinvug.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yjeptjbz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xvgdhmaa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2evtxnylu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2capqjoyk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wbhxkynu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cicbvtlv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gqqqfojh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xqorxebu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hbeakauk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cfyjtqzd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qamsjmsh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zlsjhbwj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iemdmgzf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nrnqtgjg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qbejlwzi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vfahvymc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wamnboyc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2akrrelkj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eewkntvv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2caoqdfva.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewsqwfxs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vooxgnwg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ctkdjjhn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tweksdpo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pjvynojy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2odcamdol.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2szqfwgxk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ghsgsklk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2usmjrvbg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ifiktfla.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qravgwwv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2eylxmqkz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kjwinbue.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kfllurjw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bhlgxeqi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ghgsores.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yzryrvzp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gidxplya.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xhlobfiw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2afbevzbh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vlsfrqjk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rultjxuz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kawtrish.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2aisxauaw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2htqxtxfv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kxsvrqkx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2edehctnh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ksebjtdl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nsncyowb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2afmzdxmh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mffzalln.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jvmrbgiz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dcknpouw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2czbpulgr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2falvfwrk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xkrvionq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ydctsoox.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qhflsqui.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2avdvxrde.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bzvieuun.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wclolcer.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2uuwymwda.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nqotxqkt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2txyyhiuv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gnmiaste.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nrjekzrg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jwsvvhrj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2frhqxqge.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2idsldmne.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tifmzqqy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kxjjmdeg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2scuwmpra.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jfqqmtwo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tjufhnck.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sbuwpwsg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rxrumjfc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lkrkkwct.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jrgoilwv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2cagryrcq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ntupixoc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rrxdkxpg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wytoduxc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2spudnarv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rwdcrtmf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hhgddkwp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wrashrqv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jwzlpwah.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ukoyxiiv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bxgiqmpp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2skxgojye.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gyppnsfq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jjvvlbuh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbjexjl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxlpgkwa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnadajm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pmvkyyuz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2omjdsqpu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fxckzumn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2agxcvcjj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ytegaiju.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lxzdluwp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qirdrenl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jrizbaia.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xgzjgnvs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vgpfqvcp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nmtrxjia.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2tbjlsnzf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dsocxmzi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2txzsamdq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ziozpasj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2difftxof.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xfojncyw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2iobavqot.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vubsyxuu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wasfgtwu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qwhxxrut.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhzcver.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lljgowfd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2arhhujrt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2muvtmnvl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2livytmnm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pmmbyqmf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wtwzrpaw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2opyqqbvx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gqitucrt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yvyablxo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iundwnbt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rohrhfcd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2prdvawji.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2gkajbtau.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ecekdcfy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xbtqlkck.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2flyiaqin.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mryjaopv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvofgidr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wwzzcsnf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuqwoydz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2eoyvznff.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ublezrrs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsikolbi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vlatztkd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ijagbdbj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mmlvmndd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gbxoywbx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rirdxcok.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vfpgkbhn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2joasuewb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gzoisfgc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2urdwrpqe.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2epbrfjus.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hopvlqnx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qlsoztgz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pskgbcow.html


<!-- 参考信息 -->