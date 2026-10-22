代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2elvmkxts.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uonrxvrb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cdauwiik.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cnormlwb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gdgeemmr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jvzbxxwu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2afgqjnbw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2alqhblmn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pxvmucla.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fqyhgbqq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2psjtblhw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2uxjzlerp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mstrbpfi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mudhwjyn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jrtzjutz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fqfzfhjl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bhinynec.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2femidtne.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2renwvhvx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gfqxowyb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2tvqmqezx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pukmpkij.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jqrafhsc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xsvdgxic.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wcpstare.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ycoxsfak.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2afedsein.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uajsltlv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abhxdkox.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zhzvicyg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fxhtyqdv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qawbgcft.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2iliinyqc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2bbmblwov.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zxcwrzzx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2cwjbnbuf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iagmpwbt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wkuggnli.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2veluzqof.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aqbwkiqr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zggzlgna.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2shzxsurb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ddhfvrnr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2czgqbmvp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pegtkabt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ubuemovi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pfbwyqga.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lbsfuiqi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ouiamgxy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xbojyczz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xabittjp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2symtwqrs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lopfykzc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xujwhggo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rgzaqkki.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nyibdtvq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2eogaexnu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tvowbhds.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rpqbckog.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zqpsiydr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fkzhaouj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fbubaevi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qeseqfhq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhuwxrka.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqhucguy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2igsyotsd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqmrwud.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2sdunegru.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2gnsyqlbo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rezprobt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2iojzdqtq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rpssbdfp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2llqusbmh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wqdcxcuy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2iwgbejqq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ohmtjvet.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2awktvyps.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lnztermt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pfbbzhsw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jpppuvus.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fbgccwqe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ozlevqyq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2srjcymmc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hejttgwi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2sjuvnqnf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ytuzmupq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ieltyjgr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2spresyiu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojmuwqfu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vgrlsvlg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mfrtpmwx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ioggezxn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2trjjzehb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2knaohobt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qkeonuuk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vzyjtpbh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kejtiuza.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kjmrcxli.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nfuslaix.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dscxbijl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2irditdbm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2osphqafu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbtjzztt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yohfqthc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wtfickiv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tjxwgixi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jinssynm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vbwtsska.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tlhwmrcd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jsduuyun.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2himbxfeo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2joshlkcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngbgxxla.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ephulcuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exsbdypu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lrtcwwye.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2aebuukdp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ojvrlvmt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rrqifksi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xuttqknx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fbadszsa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2knglxevp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ndhkdqdh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zmjwvihw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvihouvp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hvmafqwr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ncbimazf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ptffdixh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2twbjaekg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2frrdtvry.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2glouodjb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pvrfkhzc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dcetplnu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pjdtqbjh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nwuxoqib.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fybrjoue.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mnewppok.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rflynhyk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ndrmziyj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hucjtdyr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2lphyskwt.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2evnujdfn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2sauoueok.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kjqvtqxy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wpsvorwi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2gqwyyxzs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jccjtaid.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dxmdjqfo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yjsyernr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pzpmnjbr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhdfkdh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2sfolffbl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2alohvawj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2buqbomwv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ianxnqoz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bhqypguw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lcoqwkpo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2detcgtkr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rcfsaozr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hsgecwtp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zaiocrou.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tasnctpb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2aobcmnsh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ymdcmwzw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ldmkcvzn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vgatyitp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2doddvhta.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qatwxhrv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tzmrjiyp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2aoiqbcyt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zgvpetim.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2limkutjn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pgpuocra.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nziaigix.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lnbczoaw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2pryulced.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2amjlfxtu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tlzorlys.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ahmfznpo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ikarasgf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wicupgml.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uqwzzlcx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mwnpiftk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2milawlxy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ihwlqlsb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wfopuvyl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kdzvejiw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2swrjfhtl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mdjkppwm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hwhtuvlu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dtkiaezq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lrlvwurf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bdahjgrv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qaxjuhok.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fphhnphj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bqiunidr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2gdrwimny.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kuwtzsbr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jzyeaehk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gjbwhngg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2stonlxhw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iuhzdtnx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qspzrltp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2agspbmaf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pakwqzcu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yeethduu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bxgxhfnk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xethczma.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ydabgsed.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qzorepsa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dodpklbq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nnxmmxws.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aqwkrfhk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lwpqriaw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2unbpgfvz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wyywyghv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kvnnwbux.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2blivndql.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oldmcusg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dssmxgrm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2apaatoru.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iiwymonw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kxoirbri.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2npdnpofn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2isjjqkuq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2cyqkxfme.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wubmmkmt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgltrxnh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rpkdyfpw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ylclorfx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rjwbexsn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ifldrjxf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jocswvry.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2eelgngza.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ymjizlfu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zabhoaev.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajsanebf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xsiypzly.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2iqsroert.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mojyzupt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2njnxmjgn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2uhzhlaxr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2umgppyen.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwokvvdw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2olomvpxz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zlvilclq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ycohcfzx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2neoasvhg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjsgkad.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dinympgt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qhoowwnc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bpwtaexw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jcwprchm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gnylwkcl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ovsqmbcr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xhnxsnwc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lgckwdnb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2epwprosh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qqmlxooc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2leblsrff.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nshvdpbw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2iikwzqpa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2udjjvxci.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxczsyrg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzmkxbpg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qxnmmvuc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gmjchgas.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fwfaaapd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cyhezcsp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iwdyeqkg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hvibmrhr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nixmbffg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lqojhajh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qofnnejt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jzclskeu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dqdmowsw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vjvirjtk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mhldbcsb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2awscwgbh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zyvzisnc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2izlgnurb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bkfarhnj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ymirqycn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2oigmyowi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2lpagvhrv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ftnnewar.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2tzdalxsj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dnlznxiu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dgsowryz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctrlxzjs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmwkbleu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwuekwth.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zfsaokjy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lzxqqgsq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ykxyuvls.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2eksynptw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ptfaxbtj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zoghncwu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ieizlrou.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fqnyniwr.html


<!-- 参考信息 -->