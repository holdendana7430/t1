代发 wailian999

[D07] 切片 / 取子数组
来源：http://rm.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ib.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bb.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://vm.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://ae.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://fa.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://lo.gzmigu.cn

Ruby: arr[1, 3]
来源：http://mp.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://rh.asd995.cn

[D08] 合并两个数组
来源：http://dr.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://lr.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://uc.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rw.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://ra.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cy.szsharing.cn

Go:   append(a, b...)
来源：http://gg.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://bt.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://fx.chemitech.net.cn

[D09] 排序（升序）
来源：http://pe.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://nw.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://sd.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ih.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yk.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zj.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xu.yuexingan06.cn

Ruby: arr.sort
来源：http://zx.szsharing.cn

C#:   list.Sort();
来源：http://tj.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bp.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qu.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ac.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ql.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qc.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sh.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oc.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fu.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lw.szxytkj.cn

[D11] 反转数组
来源：http://if.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fq.521024.cn

PHP:  array_reverse($arr);
来源：http://qy.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zw.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://im.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://ql.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://yq.hnjuh.cn

Ruby: arr.reverse
来源：http://or.gzmigu.cn

C#:   list.Reverse();
来源：http://mc.szsharing.cn

[D12] 查找元素下标
来源：http://rg.521024.cn

Py:   arr.index(x);  x in arr
来源：http://cy.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gm.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ou.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uf.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yk.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://hs.panjiajie.cn

Ruby: arr.index(x)
来源：http://qy.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://gk.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://dz.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ew.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lt.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://ol.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://ez.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ub.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mt.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wp.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tu.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://nq.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zl.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pk.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://rg.521024.cn

TS:   arr.map(x => x * 2)
来源：http://ak.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ty.jctech888.com.cn

Go:   // 手写循环
来源：http://wj.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ei.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hp.yuexingan06.cn

[D15] 去重
来源：http://ba.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qo.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://em.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://yj.newstarts.cn

TS:   [...new Set(arr)]
来源：http://xg.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xm.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vu.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://dk.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://fd.huixiangedu.cn

[D16] 求和与平均值
来源：http://sy.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kz.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sv.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gu.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ma.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wt.haigaiapp.cn

Go:   // 手写循环累加
来源：http://na.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rk.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://tb.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://xn.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://ra.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://xn.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sb.521024.cn

TS:   Math.max(...arr);
来源：http://nc.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ow.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rw.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://ne.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://co.521024.cn

[D18] 扁平化嵌套数组
来源：http://va.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ka.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://nf.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://td.lnxyls.cn

TS:   nested.flat();
来源：http://bi.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ih.nicolike.cn

Go:   // 手写双层循环
来源：http://qb.szsharing.cn

Ruby: nested.flatten
来源：http://je.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yf.9csxet.cn

[D19] 按字段分组
来源：http://fd.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ie.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://or.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jz.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sw.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jh.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://er.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xs.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ee.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://jl.haigaiapp.cn

Py:   Counter(arr)
来源：http://nv.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://xi.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rx.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zr.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nx.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://mq.gzmigu.cn

Ruby: arr.tally
来源：http://sg.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wi.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://or.huixiangedu.cn

Py:   x in arr
来源：http://qt.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://zd.yuexingan06.cn

JS:   arr.includes(x)
来源：http://dx.bjjhwx.cn

TS:   arr.includes(x)
来源：http://ik.chemitech.net.cn

Java: list.contains(x)
来源：http://cs.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://bw.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://ka.shtwfgs.cn

C#:   list.Contains(x)
来源：http://gr.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://sn.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fe.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://df.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oi.jianghongdianzi.cn

TS:   [...arr];
来源：http://xq.newstarts.cn

Java: new ArrayList<>(list);
来源：http://wk.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uw.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://wd.nszjky.cn

C#:   new List<int>(list);
来源：http://cv.wgjwhj.cn

[D23] reduce 累积计算
来源：http://yh.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://au.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kk.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cg.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pp.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wg.gzmigu.cn

Go:   // 手写循环
来源：http://hw.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kn.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ut.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://fk.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ff.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ci.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wh.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wx.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sz.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jm.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rg.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pr.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://cu.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uo.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fw.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ct.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xa.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jo.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zc.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://er.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ei.shtwfgs.cn

[D26] 数组转字符串
来源：http://oa.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://nq.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://ya.9csxet.cn

JS:   arr.join(", ")
来源：http://cd.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ef.wgjwhj.cn

Java: String.join(", ", list)
来源：http://ly.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://uv.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://ub.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://vt.lnxyls.cn

================================================================================
来源：http://np.huanxung.cn

E. 字符串处理
来源：http://gq.yuexingan06.cn

================================================================================
来源：http://ra.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://zh.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rf.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fk.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fk.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vx.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wp.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://be.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://be.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eb.shxzukj.cn

[E02] 重复字符串
来源：http://rp.jctech888.com.cn

Py:   "ab" * 3
来源：http://fl.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://xf.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://eh.szsharing.cn

TS:   "ab".repeat(3)
来源：http://er.9csxet.cn

Java: "ab".repeat(3)
来源：http://id.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://ku.haigaiapp.cn

Ruby: "ab" * 3
来源：http://rc.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zs.huixiangedu.cn

[E03] 截取子串
来源：http://jd.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hx.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lz.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ab.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://js.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://ng.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pq.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kv.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://fh.nicolike.cn

[E04] 查找子串位置
来源：http://ez.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://yd.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://zg.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gt.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://me.nicolike.cn

Java: s.indexOf("x")
来源：http://rf.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://qk.hahajie.cn

Ruby: s.index("x")
来源：http://tz.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://wb.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qh.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aj.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ae.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ce.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://il.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fl.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://av.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tk.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fy.jctech888.com.cn

[E06] 替换子串
来源：http://yo.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ba.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://hn.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yj.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://cz.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fo.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nn.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zi.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://ph.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://go.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ic.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zp.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tz.hnjuh.cn

TS:   s.split(",")
来源：http://vo.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pw.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dk.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://cc.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ow.huanxung.cn

[E08] 数组按分隔符合并
来源：http://sw.lnxyls.cn

Py:   ",".join(items)
来源：http://ji.521024.cn

PHP:  implode(",", $items);
来源：http://oq.shxzukj.cn

JS:   items.join(",")
来源：http://qs.muxihuayi.cn

TS:   items.join(",")
来源：http://wz.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://cx.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://ep.wgjwhj.cn

Ruby: items.join(",")
来源：http://lv.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://nz.huanxung.cn

[E09] 去除所有空白字符
来源：http://px.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wm.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wz.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://jh.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://oh.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://uz.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hu.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ai.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://py.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://yf.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yj.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vz.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://bh.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://pl.huanxung.cn

Java: String.format("%03d", 7)
来源：http://gt.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fc.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tf.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vw.9csxet.cn

[E11] 反转字符串
来源：http://wc.gzmigu.cn

Py:   s[::-1]
来源：http://ut.hahajie.cn

PHP:  strrev($s);
来源：http://hk.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://oi.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://jj.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mg.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yq.panjiajie.cn

Ruby: s.reverse
来源：http://jg.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rk.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://si.yuntaijiaju.cn

Py:   s.count("a")
来源：http://sx.521024.cn

PHP:  substr_count($s, "a");
来源：http://na.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://yj.hahajie.cn

TS:   s.split("a").length - 1
来源：http://nt.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oo.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://eb.asd995.cn

Ruby: s.count("a")
来源：http://js.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://dl.szsharing.cn

[E13] 逐字符遍历
来源：http://yd.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://cq.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ke.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://js.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wi.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wr.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aq.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nl.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tg.haigaiapp.cn


<!-- 参考信息 -->