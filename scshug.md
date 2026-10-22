代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ogzkpnvn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dqwlzadg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ynomoeba.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wguxgwuf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2juuunkgf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kwhrfbfm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ygdhdwse.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gaahecem.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uoyjuhke.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zcbshbkg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2epwepkox.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tolgiskg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bnhvhdiz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mbzygexz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzmqzkva.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nhmytymv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xozwcwin.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jrtgbjky.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ykutizut.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lialcsay.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nppdzwwu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2sywctzka.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wpzwrrdi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojpnjhef.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gyhiceoo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ofvdpjbe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sqedsuqm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2twyqszks.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mmvxmngn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2goxymeyr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2acmdnpqc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lwquxdto.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mzldokhe.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hbjndyfo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fvwdysms.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dfpxlonj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2skcuvugl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ighnrgqa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dynlbtuk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sizgwies.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2uigxzblb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2sweuyebp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qmtrvhla.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2iiiquxeh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yvwdacbj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2afjxzqxv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2cdmedlzw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tnzkhilj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rtvjrjnx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pswzvsvr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2degjvboz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2iyofxobo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ajdsjslk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pwjqppya.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2dzgfsxdo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dorbgslt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2sanacpct.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jqhtdyio.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bbzwbrxc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uorxptpu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2stothfwv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlirnrsz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftdcjhui.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyvudnkr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsqggknh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2soekuciz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vcrnirhj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xhbtwazq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zagxwqth.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hyrriarr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2levugtjp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2azskgmpm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ouolpqyq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bgjhfwqr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ssqywper.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hnorjsqu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hrfxseph.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bsjochxb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jxvpqeaf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uwjduibz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cljyjbwg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2htimzoid.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jagcdxsa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ypxubqbt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhoqqrwf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qrbyaiqs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qxeigsel.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2roijdjft.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytzsiczy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fkqjjobd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2sjfpmrdk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2uvmkhipq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vfzijkin.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2giapabgd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jbrjtlrs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2toadvfir.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hkgzbujq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2karvbtec.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2euyowwiv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rfjecawb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cyhkkokh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wskimgbf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pdkdfflx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rptankte.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2crfguokv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tiqcdkae.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2htbbknob.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jbrmuyem.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tbyjymnt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yvdspglr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vezinrlb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2perwqljy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqclkzmb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2nmwfnlwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eklpuwpd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytxyypma.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2iimqfkjj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lskuaymj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wqdhfuit.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nwkvhvtk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2epzdzqst.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jxqlrsoh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2tfluvazj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wpudenav.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cgjaaazk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2koabjxyt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qvduqhud.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ndpnlmgi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bkmtffkz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xjgrpjsk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2igsjvino.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ryyjnads.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zbpohlyu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hmyryxnw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sijwaloe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2byusnmxz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mceohgdy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lsidepot.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vgowbcsk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2umtwmliu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2soeqrfag.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bzfpclml.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2cpdqsuig.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2amrlodew.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cnuknquw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2elzafsmh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cjkpkdmw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uokqvbao.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dbqrkeap.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aowiksdg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nvbfapak.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vhmftzit.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vntjmlmo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2pduzxsdp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2keficpdp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fcxzhrvh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sipeqxjm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uupqjtqt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tqnyepew.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bjbustvx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ygwqozas.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fxhwkjwy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2outtcgfk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xyluabil.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2virhlrqi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gpjnlnqa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2prvcwyma.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bhftgpjo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zrvucywl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qftzmxte.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2oysuqure.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2noatgkpn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qyydusgc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lhgajvjj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kvrviybj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpykzflw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2niuvyblb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qbyemjxo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zolrrvqd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2idkggogh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ykpkzsax.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2estvorne.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rsigfzib.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2utkwkqha.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lrvwgtdd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2krexnjvl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pnhhxhpt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mejwowzl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2luxyyllr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bqacbjju.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ovknohgu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mimnonfj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eywnillw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jlayzvki.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dqjzwgly.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gpfaduhc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wgerfafa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gaxpxskj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qasxxjoc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kqkptlyi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dxgxoiac.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vixcuint.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2havpqtot.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rlxvcncy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ulosdpst.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mrfapukd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zapjdcwp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2boqvvmkx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rlwfuhlp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oxypbxpd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jykaymwf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nihxrsms.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gijmwuwc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gyrkuhfy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xjyyurjr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fgdlddiq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ptbixmtm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gmjlzucg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2syyelqti.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zdlriukd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2dzbpgmfk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2numlfnxc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vmgdoqov.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ufcepunq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfbhfik.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyfrqybp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bwosqljk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxaolglr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zenlzjlr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hssnynsg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2njlrsbyi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmkdaktb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ghjynrum.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pypwarzs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2btfiqfwu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vcwhcvaj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtzhbeas.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2odwdlpjp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kkyszvqs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ucjdfrej.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pvtrdzdl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2sriajlvw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqncbvsx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ceiqhrmo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wanpcork.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jfxxarqu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ccvueotu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qajzndqg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xglihdhi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzcnmud.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2evrmzojf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rvxlnflc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2entqvtxd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kbzneipj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ddcmdmrl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hewzakku.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dkamkzcl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gzeocsda.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uitzyoyl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nxusnjwz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zgzkllfq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zbjkavdq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fndhhklf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ectapknw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2luhhzfqj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ylyvdiuh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2oduzeuoc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jpggcwzi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bgkmpene.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ddbtonpa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2apqsrlnm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ywczedqy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xvnwfrlp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tbflcsah.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bdwryrfk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rxtnflak.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ckwfxiea.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vxdrkvxp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2sjtslmeo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lkxvbkig.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vtohfdhx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dhnnaitu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lizlmyno.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wfxfodja.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qqmmmexb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bjjxmudx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vftmvomn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fgllkzos.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2frrxtyxx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxklgwgn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnrueahd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aubatppj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zcgzibso.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xhvtldri.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2zcongxni.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rpecowlm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wadjbtvr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oyjktltn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dhbqynpb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gfkhwlmw.html


<!-- 参考信息 -->