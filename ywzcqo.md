代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wwxkbwni.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2routhajt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2veflholc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oayorqet.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ucjvxavd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2czujkmrl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vsjxjubl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lomsssuj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dqcfrutr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pqkgbwue.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uhqrevab.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ltgrqsqk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yplszvtj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jpesflqs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rhxsgbzd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jopfests.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2joyyhxke.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uzzxvupp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2eogdhlfh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ixinzkpv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ckcrmqzj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mvbhclqi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ddmvjixe.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2omdbtmbr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hrogaske.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gxlplkaj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhggggbd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ruvrudat.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xeynuheu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2erkbcnih.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wlekipqv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fopbuwdc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vxztuaeq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2tsusofmd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svufuqdf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2insbwmow.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uwjcpwmt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qyrpqdkf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2moiffpgn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2phwhgkfs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ivejixkc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tugocsmz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2naptgfpq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2icycvtkv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xbwhgpsf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rtayklgk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ayqyheen.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2nvbpkvgh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hrapyqgb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2dcpymzla.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nauejddd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gyktotdo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pynvhiyb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nshrxubn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2djhchizs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2quzzjppp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jaserjvs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vccztcsi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bbtlnqzf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qoszrrxu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ihrbhnnj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvsdbelo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2odsdoiyd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hgnvdnpj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2lfwfxijo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vefxdajc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxpqaktm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yvakhohz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zzlrtmzb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2byhrhkvs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bcnfklzs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zjmkyxep.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2thdxykav.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tamjewqb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ukbkbaxp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdlmmhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipssdtvt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rxenbtbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djiknyrr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2obqkpoyq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vnhujlgg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qmywthjg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qpwxruqq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wyqzilae.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2oiqyydwf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2otftrtfj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kyggaqpr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zczzioct.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2blwxlxvl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rfpowebd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zcqaakkw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sinspqdi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ypismvtu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rfvfpbno.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mzdzzsxz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ncbfgpfp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hqluwjzb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bfyzcjoh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2oodeceud.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yttgjygs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bcwveoiw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ktgcynek.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fprhqzrr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kfecklrh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gvcvcply.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uetiadww.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qcdkxxnj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qqwjgiok.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2elkmhzqh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qywvyloj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hrcgdfoj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2prxdlgnd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mwsnubhi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2smcheqom.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zujbmzsu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ardwiava.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wzjtzcci.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2htxerien.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ekovwqqq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2chztmqyi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wyugxeuf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2uvzdxhuj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2mjkfacrh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kqzskfba.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wjaazard.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ilwxlltl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwkdagkh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vybefxsq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zxqcpiiv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yhoscsic.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gnqgbywg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2spkztixm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bufgfgsp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vkdzzyhk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pbechjsh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pegkpxbs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2egqauila.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jqfjjsvn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2uttjuupg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzlzehkp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kyyekzxl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2cxgnqwis.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2oubbfcxu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zyuuakqh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dzsysgfj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ykfqtktq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cgvrladf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kkcffqgf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ojfthzds.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hqpxhumm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cbsrsclw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xdyepmhc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mibxjury.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yweuqsav.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tejsfwty.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gyxydklx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wbbaafba.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dxhxpvcm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mbnedihp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2luzeoirb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2elnhnqme.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2etjcrmqg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tzcgjmix.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rsqhdbsg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eeyxgxjs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qodqixfy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2poxjzixp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bekiwhvp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2etyrwaor.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qbwmpiqa.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pxzznqtl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dguqtsko.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tndagzoh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rnzzsrrp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dcvyfcts.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fsqiigdi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ozorbzqk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ummigcby.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dqyizqlz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eusrikyc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2aupqkglq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2atonfyjq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yddnpsbv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yemcoxat.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zjaysgwp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uhetyjsg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lkjejlps.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zwojzpod.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2awhchewj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvpscnhe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mniozuwv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hlelnoau.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqmanczi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hnsiyioo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rrvwdfgi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylhlciqy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dflytvck.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pirptqxp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jxsikqta.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zkozwazn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijadqdvo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xdfrdhcz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jykqjggg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rqbnxvpx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kypkarec.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2actycjia.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ezvjchnh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tpqdamln.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ngmgprfh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tjlqwuns.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sjuakonr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2khriwmjy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oelwpvpz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dychywdp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gigsagfo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2epdrnjbv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dkivpjmz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ewwrvsnz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2efpvlodw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dodhymfn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2inrzrwbq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2etfxyomn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2siqdtgdg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ktzkpssv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cfqmvnam.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ebfjqedd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2diztoray.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2piefswpc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2apweshjj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2iwxminqv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2locbbjxq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nmbiwxao.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qdkiysuz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fkeszkvp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dhzssmfy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2raqzpgal.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eeidzkca.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yelzwbac.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gmxzgvqa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bxltrudr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qsrqdzlz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wmlfbqpn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pplvtwtz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zwvmsknv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kgpynmio.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fawbsdjf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2brkaeind.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ehczppzv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2sxbefkpf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mobxkvcz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qljgkmlu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wpjztemq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ybsdtvgn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owwzppss.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dxballzf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dhrzvbhd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gythrvxh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2tovdsfrd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmrmeoyr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wulqawcj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vaqhszfj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rovdndgr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lpsawitj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lfgjeuap.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kxtyjilt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wseuixof.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2asnrzzdp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iaaqcneo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2fpihdflv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkfsbpnt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ouqdsnpp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jrwdmgeb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2whyogulf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2igmpyydh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mykfapmt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tcuzktcc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hxuaynml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcvhqgak.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2htqhzonq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atjzthut.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dojquenn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2sndelzgz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fkbllrzv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vfvvrxkp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yvqsxcbn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2spzgsykl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rnbexbft.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eowoausb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vfuanahc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2iexfbkot.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cgzksodc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2umxnysrr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbcxjnua.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cospotnu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2msessyxq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zxwvcirz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vzosmbty.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2oqvxbcdt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tcolawws.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qzhjlfhs.html


<!-- 参考信息 -->