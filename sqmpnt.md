代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dcbrdfdd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2giqpiqgd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fcogyfek.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qotipbpu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2azaqftpw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nhjcuhhr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hmtifbzc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2adetuzld.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nfbhscly.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2exrpxfvu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nbwlxdwu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2yqjuhmzu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mzwpdtcg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bdruhusi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kcgortya.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zauecbcq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dksezmhf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bmzgvmwx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mizdxyee.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2almsykoo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2frmiehcq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hgxfbqas.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2trqpwrop.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wskdpavu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2alkxdfmj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oqqppqny.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uyufalhs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jwjiprme.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwxbvorg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjluwtvr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2omwwnsrv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pbqkappr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2oyctbhmo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ypgjfrsn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2boxgflrx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wgwuzoho.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ozqxsruv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kttqspsg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zfscgtco.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2smowctxk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vygyhzde.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qwuqawno.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fdhynxnq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qblcqwsi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ssazgguc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2htqphizc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dpkookzb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ousaxflx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lggmxefg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2iqepxpgg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gorptwwj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nqyqliaw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mahbjmga.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gaqzyxmw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tlonlbar.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iomahlkk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2icunyqms.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gpxglspl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2iwrtikpw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2llnbowow.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2polsfrwa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2yqtmgnov.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wpwlcqun.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jaycmbft.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zgqrcoxu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2krdtyina.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjgygmfb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hqnnbclg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2skyssrgz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rkdayqmb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pzguwpvi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jgxefgre.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rxwmisah.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2afbhpizj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yknrcffx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2aprfnbgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydjijyls.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2eecupeix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yslsjnwl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dnwftpty.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yozpuygk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xctjciae.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tqgpsjcs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ddpqywwz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cfsujxar.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nvvavasq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xiolszbm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2drfhnchu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tkdumwhk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2atoumkgo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vnlrusbd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2aehrxyza.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hoyoalnj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlqcrwi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijtrwrsf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tagtdhul.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bizuerix.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jirxmbzk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gahmobom.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bbtjetki.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ympnqtxi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2okamjhpj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lnkrsdnr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zofbwwoh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2njioensx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2kogfcygw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ghausnbh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hftosfkz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2itqtdkdy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ooglhjsu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ootqqhae.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pzujrrse.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fvrmojwd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zpxmsfdu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hgihzsqh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2viuhinpd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hqurrnxg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nzzewtdk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wnvpoeli.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2osqyrprp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mclmczia.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uvhayzng.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2iuizhxrb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tvmjbzrv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lwuyfvom.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvjidprs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2znyyyleh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sidftwrg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aumibswy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pxqoqcox.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mnuhjuan.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2feyloijb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rxaaywvq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mluqcqfz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2miwmcwnu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fujgnezq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2buzziiqh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xzxxmqah.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vhbrvofl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wjozrkip.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2knqahinn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hfasvddm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cnalufte.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2srjtgbgd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bhmfytqn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kfebjrgz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eljphqzl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2leaxnuvh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wktqcvph.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2leenezqg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fdasxzkm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yrtekgin.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iywagcyj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ctqjmubs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sypalwpt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2daujduvy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ceyntscg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pqgteamo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dpxfukaj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kromkuee.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bjpvxmwv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fqhriwvr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2pklerxfz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ggdwndoj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kfezsnkb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fecxsnor.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zpryjrpp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xrhukqmw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2weaqgxdu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yttvfesa.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2paufbwme.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2umhhaaha.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2afxffgsr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jdeccffl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gciwjpfq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uzvppxno.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nfruuvui.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tkkjpbqe.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ycbirorj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2phdrknhp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cghqdrsq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mghyjbpx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wikztfzo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sddwbyyp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gubqqvvd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nulmafqq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fjjhdswb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rfowvici.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2nkqgvlnf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2oxpwytcw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2itahmwee.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxrsbtfk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zlyiqdes.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kzrxpaxe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2oktqfbak.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zzhytnkp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hxprknzt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lyukbimq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2oqkxysss.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bachciyz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rtdtyzcm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eelbcclg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dpytxgfc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wrkdpcnl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zqsdhphh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2eqnbgsba.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2liktponw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hiqqtlai.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rarsdccr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ycvzvxcg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tgemqglz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tumbhmjf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nldynsgt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tbxhgpov.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mustgsyr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ceptesjo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2aypzklgt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ubvhamjh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cqnoerfs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kndivhgu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ynlfkgpb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dyxjfsew.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2phhfuqff.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qxjblqdf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2aybogiic.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jkusbewz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ocqxufod.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mzgvbmzt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlrwgiyz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fwwnahym.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2abiqtlox.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fqwpdnjf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rrlszwhz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qduqruix.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gjmyxoux.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zaliytpk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qgfddxvi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uoiwvgoz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ifobilow.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mfxicikc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bzubvffj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2axxyfllq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2exarxcmo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zotrtnok.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ophuboqm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zkucjqog.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2diuqnwbq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ofqwizwb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2uubxsczm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2yebrnfaf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2sqcudakp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jcyqmsio.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2cqgpgmem.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwvogufk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zvbkmmkc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2csencvxc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihbwnpzm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wdoeidlf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qzvwpoba.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eyfcowcr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2maepcerc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mdvmdits.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fnonuxcd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vsjtyogt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cjiiwuxw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2lemaxvif.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uxosgags.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jhinlfpa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2phcxgvzr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kpplmqyd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jcaydwfy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jvpjwgad.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ezlvbate.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jzkzphzy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hllijrjl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2viqummod.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nrqtruot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pivwkfck.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ktxlcfnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2niwrvrlg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2loygrsal.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2cwbxonrg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2babbblzg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ubuzlnwr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jvqncvwv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mahdsptj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pzbyqzzo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxhuztcs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jgmmnmea.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2sczrdvnm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fiedoxdb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xmtoqdqh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2scfhbmeh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxalaxnz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wybqnlbc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2iqpjukgj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dhkszbym.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2poprawpq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ptomaotx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jphojzsi.html


<!-- 参考信息 -->