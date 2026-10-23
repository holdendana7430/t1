代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3kaqmizeb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3berzqjpn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3iubgmlrh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gvfmwdjx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3djeteteh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gezgwfxa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3njjbuisi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fminwnof.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wibijdwf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vhjhtmcm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3whcfhcwq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ksnklrsw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3asgunomx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cjvhemec.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dvvwumia.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3datbqfyh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3eflinpdt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3foelkspz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tnxipahs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zfmznzgw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ffsfejmm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vmrjfiqx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pxfxqcvp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hgtkpxrn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3hglpjvca.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ealikwgu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tagzdhbj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3devgtjwr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dffvmisv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fwyykjhf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3huogsqwh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hdkckswc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ykayvtac.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gjekggnw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zuxjzxzf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ykiladcu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oypyqgxz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ifmxzudv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ocdsnafu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ffpkkddo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xkamnujc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fkvyueyp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uegkunlb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zycjefvk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fhjulstv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jzgudego.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3feeiknxh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hgveligs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fvaphzjs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wkybmnhh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tjliwvoh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3twvzhtzm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mjjsgueb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jzhbduwk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3iilqdgdh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rstgnebr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rlbottbe.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rkdqjbpn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qjbocwjq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zjgdbazq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3emdnldgy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ffeghrsa.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tviudeyr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vdtmxhks.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3yjijpdke.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkdjmica.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fiiooirs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hjeilqpb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wbvdikgp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pwrqhzvt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xfujbglt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3lxanmxmz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3znfeiudk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xfjcfzhb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fwqmdrml.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hqmxuxxe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3upadwqou.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3auleeseb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3oflirbfi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uedzvjaj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kloyboca.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ipzqvqql.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3phacjhyu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gkkjfzqr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3frakdurr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fzrtetnz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iidzsbjr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uauwhzkc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3crijaiif.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iiqfavtc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bmdmrilu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qqayjsbs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3eapnnwmt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3obdxqodz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bzctdkyo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3esvxeqfo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3drqjavhi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lygqpwow.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jnlgxtlp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uxgsdiha.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mgpvfpdk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fouynxda.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qknidfxr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xwtygohf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ynsdodeb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3csutjwcl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eaygtujj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dggzfnff.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pqhemofe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tgdvaulw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hqoduvmy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zsdilmcc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bruqfddm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ofhzajqg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qnpcyrhu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bajfisjp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xvydwgws.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vpofwhip.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vhulcotb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3llpomyri.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fllpnzql.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mmvnmrqf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnqirkib.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qwnshmkq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ullekmcd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3penvgoxs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfbontjq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dsltwysk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lsxkvpgr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3snlhfgnb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ykfqihov.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eqrgtzwj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hvjlyewq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kncgqeoz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zlycozxt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nbzbuwzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agupuykt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kdakejhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdhiewsg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3chzezowk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kxvanppu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ofldtgkp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tdixbtgk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jfnwpvte.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3juorcmpz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tzjkkuut.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wulfgbfh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bbjjlxuz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3tdgipyjp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oioldhho.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zkgovzex.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qjtdgrer.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3egqtfgib.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jegvzgsv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3oremnalq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dxawxwdc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bsoczrez.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3iaaeabbk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3kjrteoyh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vbewrgwi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hkdhwxzf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3engzllye.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ygjuthuy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tetqwxei.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vetdjyyb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvddwrcn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3bvnscpbv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xyucwjvo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ipxfnfgh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3cfowuida.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jtosuibx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tlsqeepr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3aruprxsu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3padmaklc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3huanuvld.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3knkgkmzk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ngmqsfnl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3zugpnxka.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ohbmpozb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3icpmpryl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cfxhhwdu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3izyjjztr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3olrioias.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bgqqhqzq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3lnptqpyq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhcmzsf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3puphfdmt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ypmvdlso.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mzrdimdr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3upyxzmwm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3chlgogmv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jvsnlvbp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zrsyakot.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mgpoowuu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jcdxztho.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vghlpcxt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3snmoldoz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3veceifqo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dhsxabkv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ewarzvrt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jkahobiy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uzrkhqxf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3rulqusps.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3tpiddjvv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zpnazvxu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hvftslop.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kuqdzajd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jhnroiwn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3cpoxkjpa.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uhljhvyq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vwaawxrt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3secaiars.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kzfvxepr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ljmwylxt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kmbuncuz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mqkrxivy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3runuihqr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jckftdjb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qghdjyxg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fihnhsjy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hrdqkkbh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aeurnkof.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tifiotzm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vutbznmc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3unvlwtzf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rsgjhzem.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wpodmboq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qvihuusw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qtbicjvr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3onffxcgo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cykwgaxp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qakezwcv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dslbqdiz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hmgrbkky.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3klufyoap.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ewpvwcrr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fqwrxdfm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dglnwhsa.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mylxktqz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aizerwsi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hisqaacf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3oshjcwul.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uhtbuctu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mbhidwmt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3eqpumira.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3aqdpgtux.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3spwmjxdh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ftaqfavr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fchwygha.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3awurthyt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xolutjux.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lakdafzn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnrgkixd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eovdbiza.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xwadbjvv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wjhdcbnl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3aqkqdfgf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3sktqionp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3fohninut.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ilwczddw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osublqko.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dicdgqif.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bfgtsmdv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vvnulidy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qcyicjpf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ytwljixb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewtqvfnj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3olidlecf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ljshkluh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3dyzhqzkm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wkuiqags.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owhhbtuk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3edvhrvag.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hnfsihxt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lfdnkizl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3kmjfreui.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zhsuhdtc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bnthrzsp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kqaqmedr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rsrsyogu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3aklqdwzn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iueouucf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lqqlzcvd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rdbkcqkk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hzkjnlju.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3raizyjep.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3efbxejwn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cysxnvkk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3yaryhazf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bllnzjwc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hfclmfip.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3muwthyqo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ycnhsdxt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pvgfwsxm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pcaivrgs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kyihzgwg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mnztcwqw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cnexgpaj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jjramyhv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zjjnlvkb.html


<!-- 参考信息 -->