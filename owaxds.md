代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2buflmasb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jidlxpjz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2gwtbtjur.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ugygjhit.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wrhffzht.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2auwbcxos.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vzxvztid.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jznuupuh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2teqemmaq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kejivsao.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2shnprqqm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cvgtyytn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2coqhcbja.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dcslcfzq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2azdvfxvi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukevtbfq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aueflavy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vremcmik.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ivrtojjh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2psnqfvuf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2megnhppf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yrqaxoxa.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ydxpxope.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zsbxosen.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xfviwvjq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2kytcbzde.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qwnszocb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2okqvdrwu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oorchwdo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bkqigjfv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dkjhfkzr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xexsyfhy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pentdqps.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rldvlulm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2xqofecoe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yiuvanfi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2phnybtgz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vvxyjnxd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2djycatot.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zzmquayf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2nthwmppp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pbmoopbx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqxektfl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2doxyrcrm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mgygduto.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cavacpro.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ydilfhfw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ixtwtnos.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2semigfdn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xyykanmx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2irdzmygx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zsmmyffn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yqitsiaf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kimetgln.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsckcqrc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxkuppzl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ufuoczzg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sqhnrhgv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqhvpkx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lksrnrna.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lsasszqc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pyosasal.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jkqizwyn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ayvsoqbs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yexwemjj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2khfkkzvu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xtoiqmao.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cybquliq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mhboohhr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qeguqmti.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2roqnofsm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ipxdflkv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jbecysbo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ajzirqqi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ylhckqhj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2eluhjbvj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wfozpzyf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nshezzmo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zovlckvf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2sjtobgmy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmnuijkj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2upwfbaxr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rdqxrdav.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ezquxbfn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2jzfurdah.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ekbrfixt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nptnbtad.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vzmvikcm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qcczkkho.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntmawdwo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2pfqlagmm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oqpkkare.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bhaftpfk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yaepsmwz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ustnjfpe.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bkyyuimq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tzxfoznc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xhnpwcqr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yjmufcdq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2witnyonn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bvfsvecu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jkmolgqg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bddssfor.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lglhniee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmzhzgcx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2frgjbbdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lntfnpng.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rzvlpuda.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lknztudj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rxslpccy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fdqtsvby.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jgfnzjbg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hzeghwga.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ypeltnud.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zjdvdtto.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2elnkiukf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gzgcgyvd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tvlvquzs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qgjmwchn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qwhtlvas.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oxrkhvdo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vxkdsejt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mlnsqynw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2egsechkj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hhosldbc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cdwmjvtk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mmqymtwr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nkjyxues.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2howtuiax.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bbznofsd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vadwucbe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iyrzitmi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gdkfmvjy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zvuuyffr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zudtkmid.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jlgcpipp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tbwrwdat.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vgacyvxu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xukvilnu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aagcwfhn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qorqpgbo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xqveikoi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hldtomnw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2amjbtqrb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2trquzfgw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hineebti.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2prtgvmkr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vsimfcsw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2krnvngge.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2lbneicbq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wajvxnrh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2metzcjqn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ksxfnidp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mdosydlg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vidkhitg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hnaousre.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vnqicthi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2epqwqdeg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fshtnzxw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pjthpqec.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lglalcfp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fgesmrjd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2owxowtch.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tfcxtpxp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jjwkvqxk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2oujdonya.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rodlormk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2safzwufi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vlndoxen.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wmykojic.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xewbclcu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mfonravs.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ogxdwdjd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wmguhzuj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wgoireet.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ephdxlha.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2okggueeo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uquudbai.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uzagjhvg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vjfvpfwz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kbxowfcw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ypfwbcro.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tsznzvoo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uawnzaet.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kfskqfpe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2znkmyhdk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bfjkprdf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fljkytxd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2plqebjgf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dqwnfkld.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vwzctdzi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tseawxhj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ofcdbzvl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lkprpshe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iahhnsjb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nlkvvkcl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gcymrhps.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xgatskvd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vqnflnui.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uwybokyn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dxoqhqcs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mrluaeaw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vscrvhvj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jtownrvx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xwlmrhvg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tesnwxnk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xioypfbn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ceulaokm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2uhkhucvh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nwnnztvp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nhmlbfcx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2irznctpm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vjxugpxo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bmuubqdu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bhkilybv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2snojcxtz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2knrovxlz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaukuqpv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngkgshcj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmwuedjh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gplrwdpo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nhomrdml.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wyreftzs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zczjtyvb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wpjiymba.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kxvilypy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nwjstbjd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ddkedudq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2orsxkqqy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xzvfnyja.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2chkuscpc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2pfyoromc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cfxzvfek.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yitymppc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vozrxkzp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ouyywjgi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2folhcodo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yrevnmsn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xrzzurpv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahzdpvbd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uodtdvta.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qpsyxocm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ovtjymyt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hoghlarn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jyeufmyj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ldurrkgy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jmhbnded.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2guavhbvj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ouyeikhv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lvwbiqtu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yjlihjea.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dpeuarff.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nppvcyan.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dsshefuv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ooatdswr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lbbichac.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ertzosei.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bzagfelm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jbllffym.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2dfdcwtvn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2dhqgknrg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vymywchr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ibbnhdlf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kgpdbzme.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uctwzaav.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lpshlrbm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2njtazmkn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pvwjecnv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ziarxrxj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kaengnez.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pfmmfspv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2llwspsjp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zycsyusb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2avafzrtc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ebemyxyi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gpmtvsua.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2empxyjns.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fsibufaq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wfgzuwtc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2epwgybuf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ddtnkdaw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zytaazzn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cyprcqsg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wmzpimkg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sikynljx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2scppwkkf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdwydtnh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2muilrlzx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hyvsjaqq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eezscotc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ylrvfmms.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xdeqgxfu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2znduvoxa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hwyzsazm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nucvavep.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zoqhmjtt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2yylmaryy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2krdmhabo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mnefjjke.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2urmbuzje.html


<!-- 参考信息 -->