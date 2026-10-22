代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sgpjprlh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dmtcphpw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbrqplso.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2akjorgtm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uupfelfr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2snffmesw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ifxrrlbv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kfozkupo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ongxbmql.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bynxnelg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iojpgqkm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lnkoyucp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2racxxnzi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cjodwkle.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hncfbcjd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2whcunqdn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mqwlyzsh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wsdvoyjm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2txnirfeu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xhugjvjp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ivsfzwxh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qdqmbczj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cojcdycu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zevcxnmz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mrcjjzsv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ypqxqhko.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2irbfbcuy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ctowzyks.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kbcencxc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2frrnuxhq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xccxhdss.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2oiioecpe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uwierjjw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yvmwgtfc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2capdlanc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2leuildws.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2futsipnl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gseosccx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wzhqegls.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ukgjudrk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qgipyrja.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2uelnilvr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bhefwddt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bblbmppi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ckgwxuph.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wkhcyjop.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2davkwoit.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2didcsvjq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2waunnvbl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2akmfdvdv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ondwqgma.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2igzmqfsd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2knuevvlu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cjybsbtd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2peeutcgb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nlmfojpr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zhvkrkyo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vumgdrrg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dxyjlhlw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kzytihec.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fvkcqedk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ppqyjbkz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fmyrwlms.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2szurbapd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2htgondjj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xgqvnyrg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pqforrxb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fqfnqyoy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ozstcqrv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2swagdrsc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jbhyerkh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xmkvqvdy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kefpmoiw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bmavnvqp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qzcoqqwx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xrvvhvvx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vxhwoths.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2mcmdzerg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vwdzwzyi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fsxapolo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hrcssywt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gxoypcra.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pjbozodf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2inztbjir.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqeledu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hseyhshx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lqhtndun.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2whkbinrc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ngchdnld.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tuysqgku.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2psnngxse.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2lletoxgw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ptdkpnfn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqyouwxz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zkyayadh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bavuirrm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2brzhqmzz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gqdbfpkc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2szhwfxat.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2elhrjaxd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kzcckjro.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fvpitjln.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jgvwzxps.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2umjthbtp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hqefulhj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gdvtimmq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2abpwldlf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2deyugepf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmggtkac.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ayfaxzwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgdvgjac.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fnumedya.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2whpdfanh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lbemlfmw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uzlivmxt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2iyhpulid.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dwisksbs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2stvrmrxx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lkijovar.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qzezrhne.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wlxdvnsz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ipnfkcdz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hbzdbdsd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfrkjev.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bstfguaw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ovtkxofv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylfmjkzh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ihrgwybv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2aqknaxol.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2quxdgkka.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vmxvvnpk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kikewahq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bkhxdorn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lvhpcdlu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vftpsyhr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uhoseuih.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rtnsaizn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkmykpp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2reqxqbpl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dspmesnm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lwxgsvoa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xnztlfwq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cnunlvnz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zbplvnbd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ppnpmvro.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2iovxadlc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uuaaoiea.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xmemlbrp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pfesllpr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zvkdwqqo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aaalcfbo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yhsrzeoa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wvmmicgh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pavhzquz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jxhdjrzk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2irqlaaro.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2nubozcnn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pmxbtmzc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gcgeawtp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nfphnwqy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dfullacr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rutvggqz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2eignovwo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kewdvzkj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ferkjzyc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dzakuzia.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2sfjgktar.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sizhhrrx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2iqyspjtk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2caeumlju.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2krynibkw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxpjmrtd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2xydnwpkr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2uedbtglv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2cnuocoye.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tlxkyrwt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tnmuspuj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fqhglfol.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mmwcdluq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lzliprff.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qggfeuon.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rhoyxarr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nkmdhrtg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hypjongf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fatbphvn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mjbrsrje.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tmnqbvze.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2adxiqlif.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xvcxoyql.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2jygvbuxt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tgghdeyt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jvqcpdqm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ybnmlylt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yrzdldzq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2itwdeiih.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uqohdckd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fiuwlyyq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eotsulxl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2loniydij.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2txqdpprh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2nxqgvkjd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tqjkgbml.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sfdhxmlp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aaymxetp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yosvyves.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wofjkifb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2rgoxwhrm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kivgrepq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gvigyvad.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zqgwuktn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2scxpocow.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fruncqvy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2afzpkxgm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkdwwpef.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xemawalm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mbfnsowc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2twegqyfs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xapfjajp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mdqhtfpo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vwnejqvs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2pgghaqvb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2cxxcesoo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2upvboyug.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fpkaqauh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuqhuntg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2caiwsdvn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cdkmrjkq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iyprimvm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2aeukbzmi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2iwzzojbb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2naynrpjt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wzswisfz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkvfhpzd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ublwytvf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2cokhypso.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ncgojcau.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2brkaogoy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nmahjtow.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ykfurkwz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2paugvmdj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bukphmsn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rfkptusd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2cflisuny.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvpksqqi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbjtupxz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ouwlcsqm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2timkxukx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fclsgerb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wngknreo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2astdjqpf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qwcouwwu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2opdfhkms.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hieqayxe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bnrukrra.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tfzulcoe.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yeaolqyb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bsxtvcaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2crausezz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xhtlncbk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cueqndbl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clhljmlx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vykeemim.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jwjoqirw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ilamhfnt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gdgjjdqj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gtetaeuq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fdgfgern.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rahkdkej.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wkbkffwg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wakzktrl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xttntjdh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hlrlruna.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zhfikbyl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nioqwhkb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2txxgluiq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fqnudnfx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2icfeoqny.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nggcezup.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gqwkurrt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ifujgmee.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2uycqpspv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ogwmommn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hybakivx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qawtynti.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ucyzynsn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndxganbb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhdntvzy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqdlzaal.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vbnfdvni.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vdtyowdd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlreyvpw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2occkbduf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dlagsfgt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sbnibvxy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qfpghtea.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2itztsngl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jnkwivfq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zvaygnwn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xjfformo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cexlenrf.html


<!-- 参考信息 -->