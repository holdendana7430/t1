代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uztpfbbl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rsszctgl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ywhcinye.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wrnprbaf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kipmcivv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qaibjmge.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gzvkrbuv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2iooaskco.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dlllqkhh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lfiwbxhy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2omlcljco.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hvsttnzr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ioewucqn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2riowjssv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khvalsah.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qqegllql.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2suanijxt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kqrsckmu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mimelkya.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pjnxzjeg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2njnzvzfp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nxfnzgee.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2teloqpgb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2sczispea.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2brnyjjyi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhwxeuem.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2isnvqeik.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dznqvulk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2egvndwwe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rpnswkba.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jnnzqspy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fqrwuece.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdlejuts.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2gscdlsdj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xbgrvxcg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nnzfqfcy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mlpdjzpi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fxhpjywo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lwcrssxq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcojbyqf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2avcvhpgp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lxnrkaoq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ukcqybvf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pyjpgwjn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rfsjkuft.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hatngasc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2izunqkum.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yeutvebm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kqdnwbjr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ihercfft.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fywxpczt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ggpyluuj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2huhvnwbl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2irevabyv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2uxnddvjw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2frlqvhby.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aaazsexb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ocmslmaq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bgqqiehb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gobqxgpg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2yzriaicq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2grlmyceq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ttptkgqw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jydmacmg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hnyyoavh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2nhyypsgw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2abqmcybs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aslcummd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mwyavyil.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zdlshupw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mcepycuj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zakxebbw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vrvpzvea.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nohrgokg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rvrlxlvk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2necvyqyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iepywuro.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2quasdmuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aebecisw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mlwblpqu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zvhginka.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fwiffyxu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hanrfywj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lvwzminq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2uqvmwcxf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zhrflrat.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xddafefg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hqbjugmf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pjmkinun.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wrojffyv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wjbpzacj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mwnxiism.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eluexzki.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uoooteef.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yyjtszet.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tiewtxqo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lnugnzvz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pbtbbbri.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2olehumjf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wxodzuws.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gzirbojl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2enqghvih.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mywqxsrz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hawtxace.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bdlwdtpw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ponxlxex.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2oaqtemqh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kucrmsaw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jblxljtd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fsemudwc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qogpodas.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vgmvoedy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ayyiuurm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2iuisuijo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tqrrpfze.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ndnfolgd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fegtcjxy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wkixqopv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ylukzgho.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kqbwccyu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zethgquq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pdbmfwmu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pocjrmps.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fjxvqpjr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ipmmkkry.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dieplbah.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ivsepzvf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cykpazdj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iekmdlpc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pyvlvhlj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2olhwnfxh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2odowlbyg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wtuqkrrw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2glaydenk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gezcuqqp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ehcfufsv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fjjxlvrv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zdllwfiz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hglndftp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2queufrvl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2byzjnzwh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2cbakskxn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fwjbcabs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pzexspnx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qtequizl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kdyfgbuy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oazljuhf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xfhjyfgw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jiyvmvsb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zugjofgi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bxcwynvs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hxfjdgdn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gluwieoo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jkebqehc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ziordezs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ntkjsgqg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kycpopzx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2bklqmvbm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bqzpdzcx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ppqnqhtv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2essqktpd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fqiajrvq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jmclntle.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yyjgvqck.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dxtmizfi.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yxfutkxf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dwzwpnve.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kmdtjzau.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vusraduq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2alfaovmm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fbvvrkgu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hvjiqyrp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hpxmkenl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kcksvrds.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dmnnsumx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fcwgroki.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2azzojxsa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gpxpydni.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rvhejwcs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rezmizls.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zgctaobo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bzatyile.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hnwxeueb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xwevvfxe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2brgaioab.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hbstbuuy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2heumwclw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2uogsuuzg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xuxwncon.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqvwqnmh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cttppwmt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ldalzeri.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcdphfpf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ylbsnheq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gqnmokwk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2abgfihqo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fapfexqm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ftavhfvr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rbqhbdad.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gwuqjffz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wxmbmbhe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ubyecpec.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2seyquthl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2twskbpsk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dmlzkcmf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lbuavakh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pwlomjij.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kdiscioj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xoozjngo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yjamgydh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2aywncgqj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ekpherqt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpdtanu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwzvtoul.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ldgonjbl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tockuxwj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ehmtkpkm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2oezyjznh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ksxtmdwt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ldbftmqn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ojatlqci.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xyruwuof.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2tpfbojje.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jriovftb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2amywzgvl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2trmhwlli.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnrqmchr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtlkdles.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehjigzrx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zilylhnf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2illnjvol.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2dqldzmne.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rgngmfnc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gxpwdfzx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2hforlcly.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2venvghzz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ufjzrbwi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dauoubfm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gjcfzmbg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bgbkygyl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iawzjscc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2epauccxp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jratlxjn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lmecibnh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qcqbfbar.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zsmoehql.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hvfxtmei.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ccpzgkmk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qqcbuefz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2sblgdcer.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zttzmgnr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rtnzthjy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gxxpujva.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2aekobydh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2riaahtrj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qwstyrgw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2avtenywt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fnjfvaze.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wniypobk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ckvfxggp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2luvkpnsi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mfcgipfy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vznqaqkk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yarpdqxs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dixirazk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dccwokdk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hkttzzwr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ysvagyfc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sorbutef.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2paoxcmng.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hebpfala.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qrgukroh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cvqawlij.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hqvyusqh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dchjrpbg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vcwukfcd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ndggznfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmmubtdw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2awlhhwtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogtrveyc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlnhxdlh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2equirbaz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qxzofttc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jconmldx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lxisinrh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rovomepp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mstwbqgj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2auldkpkp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2odexpwga.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxeozeqq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kbwnahpf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwfjcmsl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaajjqsz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzbnximx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2taecvkhu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qdvyourm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xmrtorlx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ihsnbzjm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2fgjuoxox.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lbnzkypl.html


<!-- 参考信息 -->