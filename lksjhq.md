代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsawmwht.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ylpjvist.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2osbkxmiu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ggkygozs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qjhvgnpq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kkopzato.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2oxqcnfsm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2iitkorzt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nobbovkh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zvarclws.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cgovqunx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yobtchyd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ggzjnbhd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gbuizhuz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lqycsfpc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hkpcrnlr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jwvogxps.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dpdvbhgf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dulwlbaj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gvsrbodf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mqmvsjoc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vpejfjpm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjueyhna.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mmkjwkiu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qcsldjlf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ptiwqnii.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gsszakww.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qwuwsldk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bumqltur.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2olothxbb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2okmjpkat.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lanvtwlk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rhzbuvul.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lztucvis.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rgqwqwuz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2isqymkyw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ilclnjzb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfrbaahe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ullqidpm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pommsawo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ugixelut.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2tajbqojn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zevmjrrm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jornqdjs.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kiquczck.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yzgjomei.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2aeglrixx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2joqyvnqr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wthafzeb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pryyhjeq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lsrsvnrc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrwpvkay.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vvyevaex.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kqxehhqm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nwsftowg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yhixqjqi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujiknwhc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wgdmcysa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2uxflncmw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2iqapfpvj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2drbmxnpx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ibdijekz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wjuehkol.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zyxduplk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zuqanmub.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2klalkwle.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2nodcuhfo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vuymintw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hkqjamzf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkjkxvci.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2cycqytdy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lddtryot.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2spmiauks.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzjiyshs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tfweoxhw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lfrgguev.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ysamwrwe.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uwkcvise.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dtguwxbb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dthbhdtn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2njegaosi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yunwpmlu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2smmlinjf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2utbxfqeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvjpjdea.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pskbocbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwfdfzsl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfspkpjn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ejwlynet.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nshmfsii.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2afyqvzil.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uwwlipve.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qpnduwts.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hlfoniev.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2eniivdoc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sbjqqihq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2aqzbpcmd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ttpkxxgo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zqbuapow.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2frrvcnvi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2slniearb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aoowyjpc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2enayekze.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xwyxtjkq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2eqacshdg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xqgnfsak.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2weqqeruc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qsnznyce.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mqohrswz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2awbhufkw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bgjuijoi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yptaymih.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ajbgzkmg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2evdtadvh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bzdlmcqm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2humpbque.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rieutvzq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2doftmdha.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2taecccpb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lehomyys.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xzetpwzz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rgxnbesx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nutjzmwb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wvddtuqu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bartteok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2aundrmso.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ylzffnvb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lzycvbrs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kwmoiuhx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dgkmxlrr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nkgkbpkb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yntvcimr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rcypenvg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtgnabsk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ztncssll.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uhnvqtac.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2witgskko.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2etmlanwv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2psrklenc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zkkaypql.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gmvqxkvv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2iomwgyhe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yxspbsyj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ufzufkqu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ggsofdpe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rrhzxcny.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2foihlmmj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2eppsafpu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2bixhyget.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2veytzuja.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jpyhedkb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2occdmosj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wflvscyu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vfhaaiux.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2upnetzpz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cukgzmrc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2culpbeih.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hqzyxitc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wxijgive.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qluftouf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2njkwbndh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hdjmguks.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fagabpty.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2doxecrfe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2owjncnee.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2sayhtcya.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bhhpwhsm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ebkxdzsl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kqidgqsj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bukuaofp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2apwhqixj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ayednhrt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tdaobxav.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dhlicnmu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2butnecdo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dxkmqosj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hdykfqmx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ekdybpmn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vrhbfvtl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wgbvtvrq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jvqekeyq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cpfiwodb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mkrmlzlz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hxvocwsh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jjvqwbom.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fhjcvvmc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xdhxzwse.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gcxlbwsx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pbqlbwfn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yewbkjmo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cbydrkli.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zldgvrde.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kciomvuq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ddzhuszi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ntfhwngw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vywwifxh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2byskvaaj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebkmkvyj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vxmoqgcv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fvgauwys.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jgbffsph.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2alagfjpo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2kbhnonbg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewdvddxt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hleoqilf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2bvuqkuav.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qrlsqyee.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mbzpgpyv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vrjaxfuw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wecmuhzs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2eqvpqugy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dmyfsnus.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcisedb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zoxdzkpv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kshyctoo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jhzksmgt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ulauqaxg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2kehsawlw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2okstpahj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgnhzcms.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkrpnmtb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bpckfhrn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vbdmsols.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bxavjgmh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2rympbaem.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2akxgfrnc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2klstosed.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lgnelpqm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mgkbnlfu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qvehhpep.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2geoyqowt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bsjlpyhd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hsddkdmv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmylcehk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tgxhkawg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlmuuoia.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hgkyfrey.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dotiiwlr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2seohnkvk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gguwnijn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lenkwxig.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2alkwzjth.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rzudmctk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gzsdjlsx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kzeexuuk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xewdarlw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mxmhjoyg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2duraxvrk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cabxfnul.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2uombzpdt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ihclokmc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nveivbaj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xyilofoc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qfcaxyve.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ljoxlkwe.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wlmjpmmw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vnvwirtj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qeqrreoc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2irrsxcgp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bwyvapuu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wmljconb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kjjjrdmm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2igbcixts.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2oeiylwjo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqmdxjxv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mybdrtdm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iylfyfqq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dediumqd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xthkmtup.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2aojbpuce.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wimgfmeh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qrdtmlzt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dacnsymx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ngrbnbfp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lvlbsaaj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xeusfeap.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzboilch.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gnnhysec.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bhudhdkm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qkitgnsq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pafnzgmz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zfhzdtcm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2uibczdzd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kgojzwpd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2raimpzuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezybiavx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2idwvdars.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pirnownl.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2acsvndmc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jywibubz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zcsdheiz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lgnctsfh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bhhyxswc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eojosajy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hnnwivjd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eonmbtxq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aqwgsbwi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wqrqdpab.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2psbnufci.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mhwpqrpn.html


<!-- 参考信息 -->