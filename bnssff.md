代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cifsrbok.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2uqgcrbyr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zrxkvydm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xceqwang.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sypfvtwr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hyjijkmp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xjcieenr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lalcxllw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2shnmkcaa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2imrgqwoi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ggwulmxd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rbmxhfcw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tedenxxy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zpsgjhcy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kmwunghs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2rtarxmxy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2sqaegtuy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2grqpbhew.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwjkyodz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vleztkjv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vjwnlghd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2slowfdpb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2lskmmguf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2blreahwz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ojpjxbtx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2skgjruvi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2twgozujc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ydywhgma.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2svwoqknu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xjbabkzq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hnayuquj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfzzfdzw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ioemyuaa.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dryqrehe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hbbeugif.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lsltehlp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdgianwy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kagmqurw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjhxracf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gbueimec.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2owdqblxv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2iblufnuk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cwxlndgo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dskpngjc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rnvjaego.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ylfovmvv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2unwplrqc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hkskhbcn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bwmnobze.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ayyxuhwa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ghhxrjpo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2bgnlrdxz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ekjcxkgw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2tknbwztv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lyfwgdog.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gwriodhk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2souhrinm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rlxuorbj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xgheephv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xisnjfjo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bqqryivi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dumpdnui.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vdejuuna.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2oqimokiv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ngfxjjta.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jfnkuqvr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zlqdptgy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nmlgwpaq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2luaoqoyw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqgxoutp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nnwaqyat.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dpcnnima.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cxtpnezn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tbdtqopz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rauylgjx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tkljnjhl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uxcqdkfa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zlqtbtuu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qvmnxrcl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2thilmfpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkbyskkn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2clnzwbtk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjywemgt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2argoiecw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2cteaxkpg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2sdeazjww.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hlrsigtm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nrkhdxbd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lbiebovj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rghijcnv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2axggpdfs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qotlntkm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pfmbfyti.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ouckxsjy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rvxzzbfa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qpifwzof.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2conpfjyz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gerpdydx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2dqlxzavz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2icxavuyu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xphuhjgv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rfzlasmn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2oezzkafm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iperdafu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2csuzoazi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mfxcekck.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qjsfeelp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vrxdzbgg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yzrmfrhk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vfjvwwjr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2buirobet.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kqimouay.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2olodtfbx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jxnvorcg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hsmsguyn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mjamjuyb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qlpmzutp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nwbwsidm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rhvnwcbs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mcbavfvl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qxhdkdoz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2abadhpht.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2adlalcia.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dlnnxiks.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ksbbiiky.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2uqypifih.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xptpvglz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yanksuvi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qznvoifc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kmnwsygl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qriflkys.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zogqgipl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hmofgmpv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yppsqysh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbolxgcs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2avahlmrf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uubhrkaj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2poulgplx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hlrqrwwf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhdvbjbe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2edhegyco.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qqfiqyiv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2egyfqhtj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xbdlkyar.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ftqcziyp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ccblohxc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kujtxazb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2leyfefpf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ghusbcft.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hoaaypaz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2erjlirsc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cnlqzuyt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2goizmbvy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ewaufbnx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cmnujjsp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2nbebbetq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxcjqnpj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2frcrzaow.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2svtuonou.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jberourq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xgtmjpoa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rdjdvvnz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gqnszkyl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lenwfcnx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2adaysaws.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dedjwrua.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xdqitqex.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2poxqpwom.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xvroimut.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ajaaveow.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2msbtewub.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kpklkpyb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tmkdjqns.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2chxanxaa.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qzkergzo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tyzbqogw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aktlnixt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qlbiikyp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2irkcjonp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vwxwoajx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sjmskeom.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gmitpbbf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xqprxvwz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qwtwsfhb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gywwdapu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2awlssmlg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2crnqdlyd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ygnclgbt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xmiuyigu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nrykmmka.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bwvulsns.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dkcnlify.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2chuenazd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hnvvpqge.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kksdgstq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yoezilgk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkqsfoea.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2splxjdbr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2miyquhul.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lwayzoou.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vqgwbltu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2boffftkh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2smvzloxe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qvgtfzbb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zdskxeiw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2utctjuli.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2iiszilnb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tetsapng.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jjfwbkmp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yocbidjd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2riqwbyvb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2efkanxnb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2cseownwi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wyibmmyj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qzvxqshu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xdqtsqad.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jwbbychm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nuzutair.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yqbjljig.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2znuwxftw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mfiquwfd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dwbjnrbr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nysmsevg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2auksrunn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2iqdwvttd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dklcajva.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2odltdhme.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nvuciqrj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jwmlkltc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hfycaaue.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnjpnmeq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2psxzrtnf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mqvbblrt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gzhiwkcv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dcxigmqd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2iwqyejpr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2uctrizjr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kvtkjzex.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bnihrwsf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qaogujzd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gqngapmk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vcpzfynd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iwdupdoh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hulspaxl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tmacwixd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hdjrcwfp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2imeguvxr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lkqblpxq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hbmypjee.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kzlrbawr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vzjlmcds.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nzkpgnff.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2liczjbhp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2sywdmqpp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pctekvsp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zbjyvkim.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2nhxawtcc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zfzpmplc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucufnrkb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2oyamcvqs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxoamztq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fdjvuytp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cptdoxnd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tfukaddf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uzsfeoos.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ltfbhubh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xgnnshnz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hqpokklx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xwncoirm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fyiprqhu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sckycrwh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dgnpnude.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fqoisakm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzroeswg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pvqiptda.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2unmrkbjv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2afqfrbbo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fvadxlwh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vnujznlv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bogfnzhp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fugeekst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlguvjqv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2bdfedpvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evintkmb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mkbgcblr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2gjqfvydh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vyenqaxw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2juecihcx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2djwjeefm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nlbqbxnk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2gzxrxyis.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2arvosutz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fgdynluj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbeeujgo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ayrryjmw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xnymvjsf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ovfknplc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zedvnclh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtjhlfl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ecykbhvq.html


<!-- 参考信息 -->