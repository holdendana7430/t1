代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ttyfegxl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ioipljqc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2nwwljkov.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gvkduxtl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2upfasini.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2jryggprw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uzfwxylg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dbruzuix.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kagyxudr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2khlieaoy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dgimbigq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cluyszht.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ngaewavk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ebszhbcg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqijkica.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qffddaiz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rmeptcjz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ozsbsznz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2juhsqspo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2iddijvut.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fudtmqdc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hsplqquj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2csirnial.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zkyqunoh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ioeoxwff.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mlzilrey.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uwaejaqo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2azfrgebw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aqtkcnqr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rsxbnbsm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gfyfojkm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2knnabesz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybxvebgk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2bcwauvzt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcvbkbl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fscqrnbh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xmoentrz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yblehffn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2aptnsjqn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2bmvthlhd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qtsiuqad.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2afwsmcyu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mqnocakl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hufdebyy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rozdrkkh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vhzhlxrv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ewuwnydf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qlnhcfte.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vkmeovsd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bfdsonlb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2khhtmvag.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2egvfkvko.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ynbxsnfw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hzwvhnxo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fckuqiff.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xrgtbmdg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2heigfhoa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hqnsyeuk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vclvsyib.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2drntcdqh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bgcssykf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sreowpfb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rmeynkus.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ecddklgj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cdgvkmga.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gqolfzkp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2csaegpms.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xgskohws.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xjhdtubh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhuepxhr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2obcstahx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gcxomzql.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gdlknmnv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oktdbalu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2srngremr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dzufmofy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgwriumd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jtpkqyib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krwozvlo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mfvgxhcz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rtludfyj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vdwrflcq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vntcvfqi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bzzzrjhx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lpsrfbfm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qnvxkaef.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2dqvbejao.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2npsxwdfi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fdhrzjxs.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rkcnbsjt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bnwgtrfv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2juvhraxf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uizibung.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ogtkjzkd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nojzjxre.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gnztefkb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aishyhyq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sygulciu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bvvnldug.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dufvbjik.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rbalqhrc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zphgikpq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sudkgeei.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vesxqymx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ialnbszb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhywnhnz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2otkgtqev.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nheuokcz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2eplavnaf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nywkjanf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yuaembqm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wnilosmk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kngmckks.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rkzorvtl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rlrnthih.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2nzvdouds.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mrqksbfl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2bskjimbt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qriycsnk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2clmvjlpl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xknfosbx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uvilchix.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sfcflpou.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ejxlbvre.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rsdbhfbj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2diskrprn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jykqugfr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewfggsxb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kfinyjyo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dwywozbe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hdbzwlcq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kqofwpbx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gmuglgin.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lyxnmevm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gahillnk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tesecjmo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mofqwdua.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2teekcajx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zcqloejd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iemkfsxb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mqdeorum.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pceukdjj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kxvyzgtg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ipsfgheb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2szsyxpmk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ntfajabn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sapmmqlw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tqitcihj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2anxvbugy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vbuxthna.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ghgsoiey.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tlzidqjh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dalcmhaa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qwxgkzak.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ozpuieur.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ankbcswn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bcvnvnot.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2mfxoggct.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lhasycbv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2emuvqiyc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bxqcwuca.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2czrufwpw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jfvdlhmc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mfiocghm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jwswqopw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vruetvkg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tiwxpiao.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ikluezft.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ukopuucc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2viqzbogj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nnivxugm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zklbwhmi.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ufttghte.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bhrkfeyi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mezxdynd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2somjqcsj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xgzrchwg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nwnuvsxh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vizvfehu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ldahdltr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2nxlupcgf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qlzyaqed.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qgmofgei.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kidsdqnx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mfkrrstx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lafujwgm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ioosqkrz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vhiyfdxe.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2oucnldtz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2trtvlnmc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hdwlybhb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bewrcblh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bpjuvajx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uknmrxoj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qgnicblt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkkhvpud.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vmjcqavm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2trwssfai.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dlhqblxe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ihkzyldv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wleixqkl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wkvuygzz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kdoseuic.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ywrozply.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mzjxhnbc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jhypwdvi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chqfrhgw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhjxatoj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vsflmqui.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vqetnqvb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jglvdftb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2thkxvcpa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wsnloemg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gifvmhxk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mvssqshv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vwkwxsia.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2pvrdbuqz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2puceqggy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ffwsljdr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jxkdvlpp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ktognhnl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2mkljbrpx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zqkaavgl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rdprwrso.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xzqbzvyx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbvekujq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bkphpwth.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nmsoxyyy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2utxfbyjs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2eoeebqlq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2spcrlzsf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kcqllnif.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mtngqwdk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gdxfmmmw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yxzvetze.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wiipxiyi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ghohmnng.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oonatwaj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xndoesby.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dcajwjvu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifkskjhc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nabcjweg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mybieijo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sicebnju.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fkexbgrh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2juhvkfus.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gtibqojp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gnysbbjj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2afeeszwk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ezgrqydf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rkqdrbai.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zwmhwzhx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wpdjcpeo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2futcghfj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ivpzhwlo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igfdkkty.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydgfrefq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wfqkjobp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecwtboee.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bretknxc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2sshilcnt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zcpgdviz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eswjtwtg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wlkfercw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zcpyqlcq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jgvqktmr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjytrshi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kzjrkhvd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xgvskgjy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmnajlzc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vcrtpwhp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gkpglrxw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yxqddsau.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hujmxyey.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xtawvera.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2arntjtao.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ykxmylsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsuxgklu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2pvnxbvee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrqxsduy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cofsfdrr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2oqmvrmnm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rwcvigge.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2khyhxwlu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yzzorker.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2poouncgq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hlivxzpe.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2spitwhcm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tznnowsc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wbtpyhsr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2djhfqkcx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jclemmul.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqdqlxmd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hazopttp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gpzwvxkp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xcoiomfo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qblchfik.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2saryllsr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2arxazsim.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pnvwochw.html


<!-- 参考信息 -->