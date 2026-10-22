代发 wailian999

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jgjxzcuv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vxdlyyzg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qctdpyxc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dohpbzpc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dqhirnuc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fubfasnv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uyxupzqn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwzxpkub.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kqcvzinc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2mjlwlmah.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ekkmdiul.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dbjuiuqz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fcowytvb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wdddyqng.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgsafzmc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmmpvgtk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rpkzglch.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dohmpjvl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dlyjdjsd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2vgbiizft.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ymnyjkei.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ifakvajh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iclkskpt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xopoqfnf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nucexipv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2klwionel.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxzjfkrc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hbaxchah.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jfqerami.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ejddutuj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2stmyivmm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2enfnmyrg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gelbsovp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ryezmzco.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zedhcysz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jojmvkce.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lljqknht.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dfuzpnnw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yygfksoa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubwifudv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jjqyrfwh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rbgvgsaj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qnydsgnh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2shtzpixj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2yyhqfzob.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qeegunok.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jawboifa.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wpwkhylp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ceketsej.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cruevvgc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ysavskud.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jktopmda.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfuwfktf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gyctbdxq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2sqjgaibj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2oiiqqfsr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jlsuwrak.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2miextyor.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ygqotrco.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zkirgaxt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjjcjews.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2haoendrz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2opalrzbz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ssauxlku.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2sjjvpeqg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkupzbtb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wgjpvddc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2kuofkjxf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lqvkgohj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pzdpxbyk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rhvmxfjk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2yjuhylro.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zhjjptnw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2klxwdeer.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2viddlfjx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fbozhzaj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xkqgeoxv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mhwkpden.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lyniwgor.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2oxrbxcxp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bdiawtib.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qxljwswz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2iyawkkni.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2okmpkeic.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2baeazmhi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nxyxfrlb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oyhcgpkp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ppkmtzea.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xjqsirur.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gprvjflg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xdzkjfqo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ckkvipgg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vugppcux.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2grwsvfgy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkgsoqk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zgzvmwne.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2iscfwqom.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dvcffllq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lzxfyaev.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hbgmykkw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2deeujfim.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mpoytapz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2uikpalqd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2afksxynk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2votefsuy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fvqxjlhv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eblgtqoj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2iuxpoqro.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxjlnafe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2sybmxacu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yywznznq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fnyyxoem.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sutkmchf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mrlciycp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vlenwfyw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2earlizol.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bchqijau.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ikwidjzk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2eqlcnwip.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hmrflfmk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ksnsiebi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pireythe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2gtxiedpc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckvltuup.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qdzlpwyl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sfxkifou.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rzvuxuzs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqaazvsq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bzjhnwiv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ugljhgqp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ltrlypxw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fbumomcr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hhjqzqzp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hkwhqwkc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yalxcgox.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vtfvqqzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffyxnxgd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2yotrwmca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxpqttle.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2scijscoc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zlplrogu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2obumeylc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vaqjmwxb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qsvldkhq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hpautnre.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ufcpttyy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nmuoreyk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2trhiqnoj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2quapqtbh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2edjxwjwd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dyskxkpa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hbkgopeb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gegwavdf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hrpbuwma.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2daonrozj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bpvqppdd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2viohehkx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pvopdcqb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fjvdegah.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dafctggf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dceoixay.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wakiplzm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lwoilxep.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wlnzzcju.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ciilwicx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yogxnwhx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2owemefva.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2teodvoow.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cxselbog.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fojcxhqa.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2odwhkwrw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nialvhfg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2snxahnkw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2amaddmob.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bkyrgtnc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2amgciuta.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2exibtbqr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jvwllknb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qlpkpkbl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ajkogjty.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xwykmfno.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wzmvqclh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2pbaeccsn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rkkgjmfz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yonrteig.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2aoibrlrk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ufplewtv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dpvfcpta.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fckadsbj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xptawvuy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2viygqtou.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zetuocyr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2thchgvfk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cnuqclzy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2oncjoykf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cduzoury.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zujkfqxm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jixqoivm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2eraqyhft.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2fxvthguk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2bzgarolm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2hmlefvey.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2cdsasbtq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jlbtkphp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tnywlypw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2puyyoidg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2czilufpo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yqsgswzg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lgclhseq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2blbgklpp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfxattj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2epmnjsmt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxbxdodg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2snsapttl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2orvgzxgu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pjxpperb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2smuchybq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qlqosdnf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hmjjpzyq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iirpnebd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vibnjcwj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bdqjnzug.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bvtdmfql.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2byxlddny.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hfkcwzfh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bbpnxctv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jwmarhfz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xmmeupfx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yfmvhveg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jkxhadxa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2frzagiou.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ileekibb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iljayuqm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2adhgwkxi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pmnzwixj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kmjllmiw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kyaswuec.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ezetaqve.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ngwnhqkm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vvsvasfk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fuqespbb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rluimzhq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zycqlzup.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hioccbxc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2nnuyaqeg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ppppurlq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rsxseulq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2owsuaxvc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2okoyvcov.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gflmvdwh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cdykyxlh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fyxjldsq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cewnnwbe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tsicpjcn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2idufvxhs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gnxknkpj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wpitdnse.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2upxildhd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gzrcxqxw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qqubhset.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wxlhzmxx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fmdryxls.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zuzwegya.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mrrxstuu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dweyjzps.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gomexeil.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uoaezzgf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ayktzadc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oyyjieen.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2elfkcetd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hyplqssa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zptvnhum.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tadfflzc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvarrxpz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wssfpntb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yditlbyi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kxtojaze.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pyvbgdeb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bghwtdoq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2lrsniunn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fooklpzg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2txvckvhm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ougezdka.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2oobjmjkf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xeizekkm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hswavvjd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohvkpzai.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfetoeti.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2irkjqegp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ofisfcwt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kzzcfvcu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xttyhggc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vudfykgg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kgwpovex.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ljndhrsy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ejpodaer.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vukuilwm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rvaznjty.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yybqurrl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hieazxep.html


<!-- 参考信息 -->