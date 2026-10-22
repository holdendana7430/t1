代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lkqaddnm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nszqnkbe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dratxccg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vcuiezpg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2atgftdol.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bvcqdhiz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tgrmqxbe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fnprvqdf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dxnargka.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iohgiicu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2exqdbutb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yedcelko.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2azljoncj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ppiildtz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yrfpdssx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qnjkeaff.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qeuqidyx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vjcucpwa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2texuxrsf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xjzkbbtv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cmswckdi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ibnwknnr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2olmacttr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dfekaxax.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mybmnihn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2kyistdbp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rhmmpfwm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kjvbplgx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2soxkmqav.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxlgzyej.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enmddyvg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxsyaur.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocofgmya.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ibbwfdkr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lgggcrmp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ogirejqa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybfesvuw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2bcylqahx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbggbbh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zasvenxm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fgnxrjxi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ogkiappr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wdcynhqd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2fpaihicd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hciqyoew.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pkaxctqu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bnoguuxj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dnepnozq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uorjdchz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ppjeiwhr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fbkrqxjd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jwomiggh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2molzcxnh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2znfspjtc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2spqpvrzo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ilbcvymd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2duesukuu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xwuqyhoi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hbzacoxw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fzjzaidt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xnnzkpzp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2smxgadlh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qfqzggds.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pfvoozxe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2panovpre.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rdbxlfnn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qrqjbclk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjqgxoz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yvfqbyyf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pqtkqkdg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oxjxvlmn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2orevczqw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2vowdqmqk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nonyomve.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oxclsvyh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rhypywif.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2eitpqqec.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ckserjls.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2coofdevf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xztdmbkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veirdlsk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bpowbcmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvfspgtp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iperpkcz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2nlxkwlqq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ruifnafc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gwzyxhln.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zsetabhm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vblvhdrd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ejjwrwdt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bksslckb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ymlndqpr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rwfmezzb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gqvrctpp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dkclqnev.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dtkfquwi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gzbmzelj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2umjjtuok.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qvzajsnm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tfcxmmlt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ygqzfkhc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jwsvffen.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2saxywphz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rcdtkkax.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gnexbefw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yoioefug.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vwgedmxu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bimlpuam.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bwyzhguh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sspxwpxa.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2asdenrlf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2scrddzof.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2uwhurume.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vkaqknqx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qicxkmvi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aaaqrudb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2lzhdlkzv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cuikeerm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cxtnzbup.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2oopjmmer.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gtzwhxjl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pvgvlhhh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2habmkbxq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xinkjcnc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ncydoeks.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rgrwhbst.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gprxqofm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2svnvbevz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2plzqgpnw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2btokvjrw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwgsllpe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vevbhjke.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cprqfbfk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uakwtvwt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtvnyrdr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sidbksje.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2teuaztzc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hlzngfgb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2epaqqjqi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eplgwfna.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kzdcjklw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tsiwxvtw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2eqekapln.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2fmdegbzz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2edabjfnm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hoznsosa.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dhzzjgds.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sirkzvxm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kfzsabcd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aunvdlji.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwhdttoo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wjcfmtuf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qhrsovuh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nxmjvwoo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qmmjjvpx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2abjbfohj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbaeerls.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lxavdbxt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2clhoznez.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2flbehzfm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eyuojufr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2bqdokmwr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2smddwcst.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ftfqmarl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2trblmnrx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wmnmvwlv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ycoqrfta.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ifkebtrw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dgftrqjz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ldvrdhba.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ymuieeub.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zahpmfkz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2gefwaehy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wobnobqp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yplyjabx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zyuuensa.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jsgrbfrl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yiskfmno.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qwjkbnoc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uqouvqjs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vdcgters.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qhjtzqvq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nxdvylxf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gqidoujc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xmofglrk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2irrwnrwl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2iwtzvxre.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2stvguelc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tcxrehmf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2guuadfct.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cvwmtynv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vtepgyda.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2idqbjife.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpwbnqce.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2swxziegd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxxqodjd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2finvdqcd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wgepronb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjeffqi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bqwwsvnj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hpudepdw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2abzcjbmd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cntcnjxo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xtvdrfky.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2likvxzpn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcnnvro.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vvpetozp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zshpeaql.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rubeludn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rortwibf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fnauegfe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wxjftxhi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nlbuwtmz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ahohfruy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xftzljyr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbjsiwyl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqcnwupk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nfzuizvy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vufnrxsi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cmhsccdp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wlnoafxq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lecndoys.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nnxmtivz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dhxazpdz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2purefdgg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2otdpykaf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fszvoufy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dxudgwoa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fhimgouh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mzawovgr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdfiplus.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fgefadew.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xggtllij.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lkavgvpk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qzgnlizu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zdezsjms.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2bcelstul.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2yhhcqakv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zvmndkjp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bfiblstt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lpcgmcbq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sfjkbsmh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2irafcafn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2kplonsaw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pduhphtv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jztabepr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ebdxqgti.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zywrgcfu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sqjuffxj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jrulnisq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rjcqtwmc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2siovenzi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2chcrubuz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2thttoxos.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jkioeopo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2umhtfatj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vtsczimt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbmpovtg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2hsqlopcf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2msfbfggp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2chbyuykb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2inwiaixr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2avwkutmw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ztcfkupq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wljbcxld.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zopipnqn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bxwksiyz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vdalzvor.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nxwyykav.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tblycmuh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2llznouzv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qrzuhszf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2bivczmpu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2njdszzmb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qssuluii.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tnjslfzc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cbgmkoos.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rriiukhg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2akmfuprw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fcjxsyrx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fyedlvdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kycicuwp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dqibzuql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hktambfj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2voiupvrq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qkudqxei.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2thtfnnes.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lbqmwxxq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wlsbcqpi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hqfhbunz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ybrximpx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yeudvlpf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rgpuepeg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dknevdav.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2irlxtbga.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wecfsnun.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tztkalmz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2krjuvqtp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ymhplzpy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yovxohxg.html


<!-- 参考信息 -->