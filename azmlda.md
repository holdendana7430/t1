代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2imckncku.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ldcmnzuf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbpgzdcm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dsfphrkq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2lrbhsere.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bgqlnhue.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lfldtcgb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hxivpxps.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xrlpqgvq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kcfkazrn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2mitrrbxx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kldqlyaj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fgampheb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cjublxck.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wauccoqj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ldnvqaar.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yhvrrzwb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2tsrzkqdb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jisghdvk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2japlrtwu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2osejdmph.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ttzgputy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2fkokylwn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ysiamdui.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ymiyzems.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vwanbxqd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tvnsgwzw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fyrsngyr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwshxfvj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2commyjmv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2haiwotlr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yfoqtfgy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tgluvqke.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2svfuylxe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qxstbyuz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2dfzkqxfq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bcyslwgy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zivjryec.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jotcqzsx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zaaalqff.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2fkvvsytr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zyfcwxnv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fyrsgkin.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ppdbxqsa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ojbcwbqn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpkfamgs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2radurbie.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tyimsdsh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lkceldbh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2uxeyplgn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xvnhmlet.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ybvwmdin.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kuqkhewn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dkxqzcql.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xgiukziz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2htwwteiy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kkvjfrwl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mgzcsegw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2krawnoak.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2cibsfiba.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2eztxcbkk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vjmhfdxs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2frojzdnl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2oikmmccw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wcspendw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zqoddsnx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ziyobjbb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cctvstfa.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dhurppto.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nyuykziz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anvdxtps.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qwtixewm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yoxxutkd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2axkiinwy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zvkuziow.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2pjtxzogh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xkzfcrhl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pfxqvytl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2guazvdpv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fdtczbfc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2uowadjbv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rpjrzyrp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uggknfqa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bymscaom.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2swpzgmrl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfonxmm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ptjfgore.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2pydmwdfi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hiducdec.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2eebojmyw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2eejczonn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbvfauqg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nygzcvqo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2murmnzlp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pmaidcyz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bmatqtfm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2onbyvjjv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zqyozxjt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yuzktxmp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nqzmyjnv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qdmdbkwe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xjtzfkjn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xnfvdtbr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktxjowbh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hzgudrdu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omjhofgl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oewokstm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rrtqpauw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tznbvhkq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lcbxvtjy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pmsjfibd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2terjhhob.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wnrsamgf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2eigquygk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qpfnwblx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2amhxjlyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gncavmar.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jlbwenvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjqeiige.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eftpcdlr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sjzetfsv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pbipmlor.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2trlreaec.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vmqpoleu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ackpopmp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nnsenpej.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2uwwoqwtf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mzcsbczc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bpbzcprh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fqlcqexm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tejvxyiv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ggrdjafh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2awmiwzxy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mjugwbsi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2spatjloa.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tfvteipt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ktmvbncu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kynyllyj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gabxetjq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2drrperhd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nnvufzpv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2euptcign.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2llcrkyff.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xjjyvrln.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2scearywd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rpknuxvo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gnqcnpcr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nrlcqozb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qensnfka.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pdwnshjx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zidcplmq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oulhiirr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ivlrgykg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lfiycmos.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bazuholt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dxaptfii.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iihgcahp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ozhgtuef.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uxzuwper.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2beqwcpfq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2osrskgwz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jihajbvd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zbpspwde.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bdysaddb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2thkihify.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2eyndqjms.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gubhlnpu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2arhlztaq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2trxlzjfn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hwmbzfzv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdgsogm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2crropfgw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gmyykxdr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wmjbcklr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hwidpris.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hysxcvjo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2aszkours.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xjpcjjhf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2enclttnw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2djgvdita.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ivobpjef.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ievvvbvj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2agitvsyy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2syiwdrog.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tioudjgb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lnwflqou.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2symrguoh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlcwuyn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2fnlcqosd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yntiiiwz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fblzthyw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vkofnryv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ktyxegrt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xfipnpsr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mgzybvhc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hnfuykkr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2weilfhsj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2pwcrcuxv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vnmqydbs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zfwmrvhi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2oczxmjbx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tqbieryq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2vhygzkzo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2knlxxorp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ruqwigbv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wlopvccu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nkahpcjg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pnllujsj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dkhcddnu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oaepaoss.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kypjiiqk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bvdkpyke.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2crrfevgt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cmzvcddu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ngvdrtyj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2izlxcpql.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xkjqkpys.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2adfhpqfg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fjutvolz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zdkjlqne.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zedcfcsl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkjrnljb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vfpciavq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2uuigacry.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tgzprite.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bkfxmuwh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pjmlhxmc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2sheprwcc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qbfjwzko.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wvwhcyyl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2svgtqcze.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bdbdusqg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptmfmryk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lritjxce.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nhsgtpqg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vndnkmnl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ogfmwhwg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lfdzbybw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ridbquui.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2trcjymwk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kngbdghb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ezycvylj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jemlvqgq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xbahnjuf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dnoobkll.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hkzkvqng.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2cdqhzccu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2oljdeihr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ktuhlmjo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zcendnow.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ohwsphht.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zayayyhi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncoarwty.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psfftxds.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dnxidizy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bixoture.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ughqrsxs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hymnozvm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bbhtdkwz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fuztlzmr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nzwtwace.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jhtxjxni.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iwdhgtpg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2layjvweq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2glgksnuz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2itkqdceh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2emuqrleo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wckqcrny.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wyoolevv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gkxayqrd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2elwmjszt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2smtpsltu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2utagmtmt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ocokdtbo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mielankb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hebdnogp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kprhohtp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qabtjwnx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eoxqxozg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2uusuhyaf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqauyjcm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pwhjdkig.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2diqgmtdy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ozbdozjh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zhdqgjtf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qymqdccz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ahxjokmr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fqigsagz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2lzfmuzon.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2hxzsgatu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jzlqbpld.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2aghbtema.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ybmtmloz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2cbeoahjw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjqkvvkf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2reeqmhtx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ylkrqnan.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zvdrnmdd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2agmtpjsj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vnvpyule.html


<!-- 参考信息 -->