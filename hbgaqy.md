代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3zxuvpsnn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lvzzcfrm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eawbnnok.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xqxgwkdq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lzxixgcw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3lpgmedef.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vnhmekel.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vdmnwddr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tiwvoxiy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jzqqmsnu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yjkuaosz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arobhpwj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3entpjrcr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nzrwvpkl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xcgezgof.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nklomjvd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qchryqjt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lidoxgey.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iuziswyt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iqixquko.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pxvozimt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ibfzujwm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mflcdsxh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kxffrzbk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ycnrapih.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3aduhaydf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbfqtjnx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3obwskued.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yvkinuhh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fbwczzar.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ypycfvoe.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uglxxmzl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zzdsztng.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lrulddvt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3efpxgsgf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahzrbwsb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qgrfiyel.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ftdsxuqh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dflcpahc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lmvhqlfd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3possrrny.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3zlufymse.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fvoghpjj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3icxxlroy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3dgxunkyb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3uagjzawq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3bolwbjxd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3liigirbp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ovhysymp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3pclmfxfb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3rcnoqyav.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3maoehomh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3coiqgkjn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjjnqgee.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vxkpapgt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3nwtucqgx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vajylpzz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fevxyiiy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3mdzhluvy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3xpjzdsiy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ynqiberc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tdhlndad.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pqychicl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kmquatms.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xzmnhsic.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ixsbxfcq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ugumdgua.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3gfykqjnu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kwhsqczy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3pcutvmyz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3sfrzjzwe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tbwolwml.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fhpydltl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfcgkgtm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wnvmczaw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ggnhvrrx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wnhatfix.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvxffqs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wygglxzk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qslssgam.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdnpkej.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3paujzskf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3olstejdd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3txpqaduc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kilbsbll.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3slaygwky.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ilupcbwa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tcxsrnpp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zuwqedim.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrivnzf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hdtuqqgg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cyycyzzo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3btvsjvvj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kupogzzt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fuqkbfwe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3crrypecc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fxpcwesn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mifeehej.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nhsheije.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tbbinmcc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3czuyhtfo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vhpomaxk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3awpodkfn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3oycescbi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ltboxncm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fkogxnww.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ngojkytl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3yrclwotz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hvttdsir.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujxjzmwk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3czmflpst.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdiijbmh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vbfwlind.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yibuzgtr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qjoxonhl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3stewfsyn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3yriijkdd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lqwljfkp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zmstazmv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kzalglsp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3muqhqpqo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lmpnfnmw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aykbnjmr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tqrjqkwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slaogmcb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dyuuyrmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqkckepd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fmkvjvbt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3porpjjci.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aryijohj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bfzjhujl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vabbicyd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hotgaaoq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3orrduyzb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ccnrkwlu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aytfsjrh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ivimiiky.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mqtfpzie.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wbradbvs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3youjssgz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ewbspobc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fsyeeizw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dgklmmbf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3eztygiiy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hgmxrcwh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qbroshxv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fqadwhfc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ehpgfoxm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jdoktwro.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uweuwink.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hrkjrkoq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3klwnhwnb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pxhbcxhs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3meniiuqt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3miizdgee.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3omqpkmqk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3akavldie.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ccizzvdb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cstwbzib.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3arpqgsjx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lrducnsx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vwzyatcf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3btwuuvjz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jclujcgv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pemavdcw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3piwnrebv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ygouxmae.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3fqoszify.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lhghlmle.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uekkzcmw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vrsaoozg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nomaqbqp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jcbguzry.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgtutsnh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lntzybmy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gnxtabrz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ktszzvye.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ejbaqxhn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jyntbzml.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3akgzlmmi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ooecjktb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yivexaaa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pjmgzrgi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3whkhlzms.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3damlybbl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dehhempm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qcuqsbii.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sogptrzi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3uomwgkri.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qnbzyciz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3rnkqtaqe.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3olzoaphz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tioujwod.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wyumkxdp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ciuxxsks.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rviqlupb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3idjqxixl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wpvvzokb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3reshdtfi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dbhnxvgc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qtkducxp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rerkffcc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qtkjatme.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xbxtrsuw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kmbdulnc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wlkhdjsr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3cplmquwz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3brfugxha.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wwspxzmg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hwptknyy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tuqiswgt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gzldoexe.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gyultblb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rsnqceyt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vmqyoutb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xgxqacsw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rpnewcfn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lrofumvy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bexluifc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yzvsgubf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hztxyeqt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aapfgqqk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zlxyvnup.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zkcvqapo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pljmlyqe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3czuzkfwp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dktdeevi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zvssrfsh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rceskztn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3eazwviox.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wruojwtj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dpiaahan.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3atkvhuou.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jtshnoej.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cxembcjk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zcwgkwsz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gfpigbof.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyhhgbih.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tkqiibzo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jakeklhs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wykuuohs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pzoabiwi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rrdtfwmr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrosisms.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3txhvxvwk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3sfrdqfwj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3yqshwevm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ltikzdiq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3xzwrtbsu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zyhcfzkc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qsdjykcj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3upskerlv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tlsvovtl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qurgevqm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3thhcgygt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gsvdgtlf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3duyewmad.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lqytikga.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ekxbbnos.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecrngdob.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pcylavmv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xxqzslir.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cxbiqhtt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dyffumbv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jugnnoci.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bkeugkpm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nsfftody.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bezihpwc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mcvtodlb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ttaxptgt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3awipqjrk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jxadpxqk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3defimyeh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3dkwwpitf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3acnukbyt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eyddgmkh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3mwnhlulw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cylqdnfg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ufmfpauz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tcczddny.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kwalzkbh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3aweifhbs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hyecwvmm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hzkyvmmi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zqyzhjfz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3figciwlc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3evswybau.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3eozirlyt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zhixwydk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yzivajne.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fzbkreyo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bwojdrtd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wzfgmwrs.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uvcjkykg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3sswywhcy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ogqcvzrl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3edsrmmao.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xbllwvel.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3adplyomf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nljpkqat.html


<!-- 参考信息 -->