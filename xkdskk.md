代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pbkgnjzi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mqvvsxpl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jibcfqle.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fggyhcsw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mbqkvmaa.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uiyhlskk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2frddnusw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2beyolvnx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qtjdvbvs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hameamia.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2uanuocyu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dqwvumie.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gesauxzc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ntcrvpxa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dkabzzdf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qbjdgkor.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2znielqat.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bqekcmwr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwthlviq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2irpdvuak.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qecfijmm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hqdspmjt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fhbjxwrd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jhhthols.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2pqijmbxq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qpaqwnem.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2xqigfxrm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lbwzshuu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jkleljth.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eqnmmprv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2runearek.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ggzbbfmm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrmejsep.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfygdhhf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqyiyptz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2tfoeglnq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2oyrabkiw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kypzsfwm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckiontty.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yffgrwov.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yhxamaup.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zfwzzevd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2cjiqcgvw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ashkpmee.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lhnkmbex.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ihltpsqz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vgmybloh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dhabbfge.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dblwakgw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ievfmxhk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2brsdklru.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qlnabtog.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2synhexre.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qcsgohlm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nafrhomr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zwdxuddz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bvftqpei.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2chiwgxpl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2emxmgyfd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mhhkllte.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hlpsqehq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mpwwtqqt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jplbyxzx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ddwqqlou.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vwgcvcuu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jsyapohy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gbeilvuc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2egoikfog.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2eqapomnl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcezgcbq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aiomletx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2arzlobyd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nmghkeic.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2epgrpizs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zghvppbx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jdcygpfk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nfnblmuy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2novjvxhr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mqqdvhaz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wwazuimr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdzispwd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gzjukkut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xoarrtol.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ecnogucp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xanxdfvn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dsqlqnvx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uyowxmcy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ulrfnsem.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ritoezzd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jwpfqkmy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jshnfkrj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uuxnhnaa.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jzpccciz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hzxvbbti.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zokedjuz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sqyvvmxa.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogxnzeum.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwwcuhin.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zlhprqvh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vrccxqcr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2apgcsdsa.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2krvyjebq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2flltmyya.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bvilqvlg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dikefkwg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hquzpupq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vhkszgpj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2igboyamv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2braddycc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2iwoccbmu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2odnnlntv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ssoklnhb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2nolqstuf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2bgipaqov.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wmayardp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ximrfauo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2lnpdczox.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lcpawwwx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xsrhifdy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2skxcxtzk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iwbvmxec.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mwgzrclk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cpnzsgjg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2odlbvqqy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iolmbfll.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ghaudgst.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dbrgsypg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sglnxdqc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2prpshstt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rvpdudsx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgguwzcn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2npyoflmz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pcinegvk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2govifxsp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdhafjkb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nyzhjwpm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozwytkqu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uxjblvde.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2nzwruwtj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nnzvrdgt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2iyawznlu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mhxdsrse.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mpcunprd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gsdtnmdr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qnnfuleh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nzjrilyz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wpcffklv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ffczrusz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vyjmfayp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jumthpfy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eoyxnwmw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xsxyukod.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2shwqidqb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gsekzzue.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cahkijir.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mmslrjhr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xysclmzx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kzsjbmff.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zwdiotcz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qrloiqzy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fimbmqev.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2yxtnkqpg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2afakwsgz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oycifukp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2grxrkjfw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hhypgrdr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yegijbcd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2shjzmvkp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vferuizw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dqymieya.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ptxxgidv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2txmfupbd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rsdaabnx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ymfeyqsy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qdvederd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iqowsskg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bcufcecp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xmjpzsht.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dnxqghru.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pmyczkse.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vllpposg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jrxmofoc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2svqbbhhw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gokdfomp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2yzxvwghx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hkryvzmm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ioxvaguk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2miewvnpg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zggoxyqg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eqkjfphq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2uxsfcjaa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vfyxkuzx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2budpbxyc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tucluvid.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hquzgiep.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqiuarjm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdgxaopc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xermoohc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rqdvoysd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxlpdbsp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cckfffls.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hjsojslf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2czjtgtzv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pynjajnd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2akdayuau.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fohawumo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2swlogfcu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wrjnpnae.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2flwguzgv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ndvejqup.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbytcyps.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yjxcllzs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwnehzic.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dkkmmhwf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vmnvklvl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2paliolxe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdpibzva.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2eufgyzoi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zkpwtxpm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2osmmwyrd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ytwzlihf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wrlejdzh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hryplkyz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vmoboiit.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2eealoerq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2egblsigu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sfarevia.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2daiatrfv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ynnbbpau.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wlkwsjmy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lsxihscw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chqfgink.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfcvsqyi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zbzbdzzw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mwplapsd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tvxjmcms.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2jddyscue.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wkgqzxku.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mnpocvxm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uhtgwtmu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wpadwrrp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfwafcm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xgannosn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2citkvcyh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fiauubmc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2athazxvg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2gevitmcn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2irrbjkuy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lzjklglw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcdmtsd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dgnbsrwl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gkmflcyp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2seuxqqnx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2arqfzzpl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2uppniibt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nuhhicay.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qpasboeb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2tgquhyar.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uwmkjhjl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tcrrakkg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqafxqrq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ndnjdjdx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2inigantx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fmkugywt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fhsqtssl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tlkfahqg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ezlriaos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2azrxixvl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jukqgevw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2spmpbyec.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2johntdqb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xitcdope.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wftvinal.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2prslpcsn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wcczoonn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hgqljnti.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mbgrnsir.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dtzuzxdb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rooskdng.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jhtoybuy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xizgwjnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2febyunbg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hcsqnpty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umarhcfr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ebdnuwmj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wdwueklj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uowrjpnd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hwtzroxu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nrvrqgdv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kqpoyrhd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2tmcufjfp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gojdaflk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pbufooxv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fbkcliiz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bgzrbtfz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cieozcrh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cxksqpyr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouamtnvv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cezxhenv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ktrakmbh.html


<!-- 参考信息 -->