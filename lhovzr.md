代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hmwfespe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wguvfyst.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khqlqxif.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3phkjyzlb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yjbkjdwj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dcuemgto.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mfwaibtz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3enbslgot.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nuhqehzq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hrramkow.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3twbcvjte.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yeqwlwxf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zqbmbfdo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3psfenaly.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kgnkehxi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nvjadtfh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ttxlstex.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ejpxdwau.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nsucqbtx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dwsyzhzb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3numptwzx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3elesfnbq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3osrbfwwe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3nweexjoc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3eapdlpjk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rrdbdmlz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3aabdcpkv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3utzvkzlp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xpvnpwsb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bmwkiqep.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zzvimosl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3oeypkojf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wwlosstp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dnrocrje.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ygdnsssh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yylwzxfj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3eoltlhev.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yulfnigz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kajppeow.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nelzztkn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iciwnzzp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uisntahb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffbtfvkx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3wuvhgjix.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hpxvaawv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vmejffpm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcfddyh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rqdoekgg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gdnfhgkc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kbxvibuh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3cfveoojr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3paojvxbe.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3txhrsouo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fuqafvoq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dydngiph.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bmcvxqyi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bulrriuk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dmiaymsv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cdaiqhjx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jekzseit.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdkzlvcn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lkwqatsd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3txfhjffd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vuqvlbbi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkvuwxb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3phpmyvbu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pugugnrq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3sodrutiu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fqkgesyn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ihontmpd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3smulfwsi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zxtwkozw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vjdmpbmi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kyhjzptr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bathmnqr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3evoqcqpd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hqwuddwc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cqsfdgnz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xnpzzggc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdydfvgy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qoetfhdz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ojdkwjte.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uulkkjro.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3toqcagsb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3oqeyhjpw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ixuhdlmj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ryzpnlgf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gqnfvkdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reupciea.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ktqbedxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qburhzel.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vclsrpok.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hstnstlb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hqfwopco.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yjmitcji.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hrhuupwr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vsdjxnaa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3joppggcv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tyathtmi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fjysobat.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vcgnstkx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zbzqbidv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3fuswogic.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvhmoap.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qbmqrcpn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eewzpjke.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xjdlcwhg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zvthppgj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ebydejcs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kkiclwyg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ghgbyays.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cmonpaoi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dqufrnze.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ujmonveg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3arlbmvcp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rxlhplko.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3lhlficpm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ikricapb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vjfffpky.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zbtjohnt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3sczhkkzj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3odzchbfn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kkfmecgf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lgxnxnnl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ytbjdnaw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sbdjacpf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vhzzucxy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vnuqyxll.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tukckgsq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3icmthydi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3trruqyya.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3asznaqvp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jlhmrjdj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uyekcigk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cxapqtfq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cngyqioq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jfpxdpgl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbcizph.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3aalhbjnw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3thnubufc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ltdazfoc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mslwcqqm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ftnjrsqf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jjkcxsio.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3feilfmhv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vfzxssvi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3iuyontcv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cserejah.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zciaahko.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rpdjprgj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kusjerfa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nniilbaj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wvaebqvo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fxenszck.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vykitpzu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xzeehzad.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jzbehjjn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3genlkrka.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wehiveda.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jxphqahv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3sbvtpyek.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bqwtasnk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jywoxyxs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3akwumnpa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fphrjbmb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wzukzzkk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3oekjhkqr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fqyqgzjh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bhgcmawy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3cywaqgca.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vxpkimkr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mqpqqdhm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pxkuqzhe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sgdscqxy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3efxtkwbx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dvuzwqou.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lmqdcgmw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ocipsirg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3thccnjqk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iyjbgkyi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3civhfufm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3aeteecxk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xuoucnzg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nnluxflh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3voiymwuh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3utwodlwy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vaflgyuz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3owoinizr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jopvfior.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mezewapb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bsmwlcyl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ribfwesp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ujljrjbg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xgsdkana.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ulpbmkaj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3frtrogwm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3orewbrua.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dnhijpmp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kdcllbae.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3alnnmttp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3twxvvtlr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vsygdwhx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsnisspp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vflwustu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3evqzsegp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ksyyosaq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rgxvrwmr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xtyskund.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nulplhhk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cpdsynkj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gfucpvfa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3msqmoilb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjgikudd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mctuflup.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ozjampmj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3fcdjmqoz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gueuadnc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3axmgwlin.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3myqmvvrl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dpnjsfqa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlwkjmrx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jnyixucy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nxjdagqm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3lrmszpni.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onyzicbb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3eacsriju.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gsrlbmim.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zlnxqsjw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ndaytvlo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nqzzhzjt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3aipkkvgm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jzanfafj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3iwexmfzq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3eqlnnsbw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwduvyc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3svymofcz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ilqytbeq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mjkmqtmy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3khssxmvt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3verslyew.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cygxtdiw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kuxpsqrr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vpdajism.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hbqynsbn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vzrtijzw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3thdqzvtw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nfivsbps.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3evcyuzgl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3clwexxbq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fhcgdjof.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fvsueppx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3akbpczpe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zkansngj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ywkhxozd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zhemslut.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gqiadcjl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cstqssid.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wovwnmut.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3gmfbmkrb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3suokdwbk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hamhyunq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3eyyptfin.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dukciabu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3waomlzxt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hghetvqn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfpoadow.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bubwiciw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnedwimn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3kozyexkj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3egzlgitv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tsgicbwx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qfhodlat.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3whknrjxd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dwakqbvi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gvorbhff.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jrrsbxoa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iawmahlf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3cldeorhf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fkbqlrtm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rshycino.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wphvubxj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vvxrkcwq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rhhsuzpi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zkcmnkci.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3svhvcgsv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fyragjtq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3lkftepgw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rhkmfgji.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qbhsitgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vujxuthu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bcsfjpap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fptkqiqq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3fsatgazc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zplrkcca.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pmfsijks.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ubgacdiy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xjmssjvn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xzoumngl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vluifgrk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwpivsvt.html


<!-- 参考信息 -->