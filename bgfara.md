代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3itbtmzqc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qhtogmuu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zanlfqel.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3orpywxnp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3igojpvyf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3atdvbbuc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqqcutlb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qcahoxro.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gpbhcpkd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ybvsxdsy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ondxbajo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3btwoojwb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tpkmiphm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zfbocguv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nqdftkcs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pntexllu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3henqgbom.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvtmrjxb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tnjifdee.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dfofeblk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oerfmrty.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzzgwjge.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlsxgych.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3najeitod.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nofyzctb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3eejbmycm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vhbnsezt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3bvxifqcb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lzonbexz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cwysrbqc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3sctgubni.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3cclxzmkr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ilthieik.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yvyqqbpr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ebrgvgkm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3omnbulcp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sxbudujs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rjiirgcv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xauzarvy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mznhwflp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvvzhcb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3oxggewgv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mgoguvbr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cwsbkmxc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3busmbyqv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lapmoegt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3clsrdeov.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3etfmggcq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zbtvqyer.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ryyufyxi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3eacweqrj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3cqvrvwev.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3grivvrhl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lalxtyud.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ljcmemsc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmtgfil.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ibkupejp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nwsdfsjv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ocsmleao.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lyppsugg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bryctubd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3obsdqsdb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ajiwcxsn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pnblmdkg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hbmlxzuk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eufstart.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3owzzkfkr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jrnsezmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qylggwuw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qfihoubu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mclnqthm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3muedlstx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3eccbsxhq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ikowwlxe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3frpslbju.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3chsnvrtc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3oyezoxvy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qdehowzs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uhdpnfqr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fukyzslk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ukbujzwv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wnnrpyoj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bgsjalfw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mebicvsi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jawxlnfm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vzqejcdz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bobkznoy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pzvcjiaz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tpbzgoze.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3grxksqig.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3tqlhkwyk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ttmnytyp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mhgazkta.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yononeyp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iywumgbr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ijchmkza.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rawnnobm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qkizqjii.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ekycnpvw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yydjdkhs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gjrzblok.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mkjdiyzw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dfjispci.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sfzivuwl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wwscwlpk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hlptdnxr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lucdixqs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yixqdmga.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3reynsdnq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rboezcig.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pzncbrrc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jmlshryb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xzbypayy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3umpejfcy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cwbobrey.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fexsynow.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3kczgliag.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdstthsl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gjouiprl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rdjbgthw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dmstixgd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zecfrhvz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fckoaqat.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hwhmxwyi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3strbxgrf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fulrnavn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jjfmrgzm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehbghyzi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvgjhhb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gorouoaw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qawrrrqg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nwbtklul.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hrpkvncs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3oafoojxg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3rkfavclj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qikgcfbf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ynmpaayx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lkiglcqi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eifghrcf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jwchwjik.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hljblhzg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ggfokuqw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ddsuwdkb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3gdnuhlhi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xuemvekq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kwmpnqhb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gtwimemm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ewmlacwf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ferbhpks.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cnnrtqys.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3slwwfwvb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nnccxnpk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mdhqkjrr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fcsyieyp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3acvxpfmq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mpzlceai.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nblnrsxm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3llfzsxos.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tbzplavk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3voxgnsbn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nvxglibb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3adhmdarz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ctdwhqhb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ijemlrnk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wkzbyxmq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oomxipvt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3snstefdj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zuabglpd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dxmjpbod.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wqztflqs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cbmllxnl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xaassdme.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tezzhofy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lwxcblly.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yebvrarb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dgnbahcu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vlngwqdc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3itwoozox.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3soxrdncc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lbmzpoau.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3eexqpzte.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3sczwwxuf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kybthcxx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kvfdzqbd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjyabkxd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sizyxluf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jkfjjbjy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3adtrkvtw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wwruzuxr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qvytwzhq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3wncxwdpn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dawbazyk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzfjnger.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jqlxhlht.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3uvbglqvc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3meybtxvh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rrktvgvm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3issikxng.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmfwzzfx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3caclrlqn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3haxeofzg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rhubmllv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vlqcdfat.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3odkrxldh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pvjucnel.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3eeaduxbd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yqctuaqr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3njpholmt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3trrvvcuo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lwspnqcv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qgstmnbe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fxyspdzi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3htygbrgm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3voikwmte.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3geixdzcf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pprabspj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qwvibfit.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ahulrvue.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ygzgjxec.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mjhqzypy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjuhzvpr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lhwpfaki.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mmrmrzeh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tbbazjqd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ikcudqty.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ivgauage.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3euubmbim.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gaeyivba.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxuwtetf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fnqocxrr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zibzvehp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3yovfzdop.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ovfspnli.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qqkgwuhr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wuwbgmmf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cndrfjon.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dzelbjbj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bpgrbxig.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtllwkpx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kabqfnsx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3korepzku.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lmzmknye.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3lxpwbjuh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hgjvcjia.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3dhzdvzlh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyhaokxx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjygaisp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxsqvpyf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dczizrin.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yxmcxvok.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smvbqqid.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xbkimluc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3trixleax.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pkiykidr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xnbwqvis.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xffenlbb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3udssupol.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3eijksswt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ustithzd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oncnaztj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gtosdxca.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tdfrmxub.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3abjiuopc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cwagfxof.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zyhqszla.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ntuoamuz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kicyuhnv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wbfwcdeh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wrafbtxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgelipro.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ubpzcttu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idkondry.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sjbtvjhr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tocpuhnl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3edfqwgbs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pcodfmwa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wpujxfaq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xsiaqmrr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qcjiyujo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjszukqv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3povqnlkj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dfscpdkb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zmtyywll.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhykzna.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dfdxgtxk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewxfuglh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xmdieipl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3cqcrgjjt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3iprjzvpq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rhnnctmg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ujqwgcfy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cyfoyecx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3agpbkzjd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xmdpivlp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bdffjuux.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3teufcpxb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fxamipky.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ituaawan.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tvhvcoxf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vukktwxf.html


<!-- 参考信息 -->