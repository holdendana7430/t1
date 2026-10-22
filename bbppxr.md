代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sqazptek.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2fzhrnxzj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2feovawgx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2dofvfjtf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iosdslwl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gueckoka.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2xmpgwlfv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2sxtoppyw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qzszjoax.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zszmxzff.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2pqojdcml.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ovmjilla.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2srxrxzjy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gikakdst.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qryxqywy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qyxecrls.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vlecrvkd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gitarrdh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2thkndxrf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gjkmmtpu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xqvvbvdh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cyyqkqpd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpuwklce.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wthnbray.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2umthaeui.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mzmqjdxa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ggtbjclf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ruirawao.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jnczwvrp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2reeqsfds.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2htjcebym.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tcjieadz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2fnwkgtok.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hkuhyvwv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hoknqqtj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2srpfcngh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wkyvxann.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbxjrpqb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eapchocm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2issbplum.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cvtlkblk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lguaytvm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhjwvaow.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kweyeasi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hitkurbm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2clkriwtw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vbzkpsxl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2actvjsrr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ttgemiyl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xpblqbcf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xqdvwmgv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vhylvlci.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mqqynjqb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ylsuzmvp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ggucjbfw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ceykoigv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvcfibz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rvnukpgw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ulmnccaj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rsmxenjt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2yxaqukgn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2djemmzhk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rpzamdvn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wurduobt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jkwtaqlm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ozrtyacg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2crbzyqno.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bgbajlcl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nuufwpdd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2yrfuhscs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2irgcszko.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihmsegmb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2rerdyjco.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmkdccis.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sehjgyxg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2txjksprg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2phllnjqv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qprdsncc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zwjichox.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hwmkgkgx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rammypda.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2apszhnof.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2whenoonn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2eclkvgqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjtnpenp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2lwksvanc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmmaetlk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zvnmowoy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2jxkcnolj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wouqypie.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2amreptyg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lxaigcbx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2awqitanw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2spebuwzv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ffwmcbld.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cnjdwyvq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ksvjtofv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uadwvcpc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lqbzgham.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mgipdlcu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tqubelwv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dlhddoct.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdmqobrg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sqjgxpsn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tnpwnpue.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kipicjgz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2tiayvrci.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vpewtgxk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2eqgovcuw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uonbovcc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bbhqfgko.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tbpscair.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ahpqgyxg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hpyxhnqo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ukozsrdn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zjvfbnod.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gsxpbmak.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2norplwan.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vxpxqvnm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ykcwfoyb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2pdugimbb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hebyfgkc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mnqfbpbj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2sfeykmzr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2pmjsqicz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fvmoqoby.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2axlvebar.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2alfutdcj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hvpfngnf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mpsukeis.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oubpqrlv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hdaamvcl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qravgiua.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2geuofcou.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2urarwhjf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eguxfeak.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ebvtaxvm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hnchnldi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2laamsfwa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cfyznzun.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ucefwzzm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cwjpynoz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2inpivjij.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ighzrqax.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2azymjmbi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2czvgttgu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2srkxfoyi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2sfrribkr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vpklviie.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bzhdqvzc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2lxjvknau.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmjtppb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wzswbdba.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lafbrnnb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pkvenvxj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2labhnnir.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hjrlyfrq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2prrffduu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yeaqrfwo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2sbnsqobf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2anduxtmm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ohdlkcts.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2slmrlnkl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uzybfsbm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ynfaipfo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qvwcaohq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fcrumzpt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2excxveto.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2awdkgnew.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ucbghvqk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kowsncnd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tbcvozgs.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kxhhnxlr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lchzqicw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yljfnqhd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tlkbpcis.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wksqphhi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dogivbik.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wzjlxsnl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2preissgh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dpezjusn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2btkxjrhf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2acumoagp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bjmqmlgq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iudufzri.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tgbpbebw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wcsulyvt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jauguihm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ltemkgtl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mydgbdrm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcekhpic.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jrimtxkq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2cuopjlho.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cuvfpgib.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2hlcusqro.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lvnygbwv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2aqwwrtpe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pupkrhsj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xywdfsru.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mrddmpem.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fepxnxcm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xolyhcwz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xzplqeco.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgvurbqj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vwdvcjba.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2spkinief.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lusrrqyl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jlmmqqwr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cveurenl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cyeertmr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lsaxuwyh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2llkpmvmm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xkixgkjy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2lgudnmjj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2yjetapqt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2nqcsbxhe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifxbpkdc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lgxnhpxk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gkplhufc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ocoqtizg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppizuihv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hjwijzxi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2luxszzve.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ioibubwk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tsrmfnrb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2opwmvnmg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zyrjioga.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qjhpddfj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ztlixshp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uvewskmk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2kblcovzh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ryfpttpq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bqimeplm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwjvnovp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2udyywaoi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zplywgfc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yhlnuwxl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2atfichpm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lzvvnztl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2woqkyxqi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2twajyftm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vtpvbpzf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ltvrzrji.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mnwgyeqx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wirkqwjk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2afujpyco.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2alwulyqg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tbosxdno.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2siylhhvm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yhjiffiv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lsryybtq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2muswmsdl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2coqdwtwt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tsrcyonm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cvaunswg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pfjzzcur.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vzzhvmqe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ftnmqpek.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dpkwalsk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2npwbpguu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xeqlivhu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2uewborun.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bfcktqwt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ndvvunjr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ggyetvwv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uckubazr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrccvtra.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2nosbvdie.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rtugbvsr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kcuzxtko.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qqdanehh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ehklpfou.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qsffywia.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rctsnxcl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jhcrcnvl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qgxoipag.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2txakqpzu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2beieaunx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2serifghh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oyuvfmdk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2prynfmst.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pfxiigkk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2haayfcfr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ocvlvbww.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dsrcwsdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjydwzke.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xtmybxzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbspeqai.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rtmipunq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2khtlfvam.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oxvmoyqv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qoxnwpkr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lnvofmgq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qgjkarlm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lpmbubgg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2braafdab.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ecjxnupe.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ctohpqju.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wnxuvumg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jpfvipiu.html


<!-- 参考信息 -->