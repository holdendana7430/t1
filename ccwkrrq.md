代发 wailian999

Java: list.size();
来源：http://yk.haigaiapp.cn

Go:   len(arr)
来源：http://lz.colortex.cn

Ruby: arr.length; arr.size
来源：http://sc.haigaiapp.cn

C#:   list.Count;
来源：http://oj.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://lc.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dt.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ex.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://yn.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://dr.asd995.cn

Java: list.subList(1, 4);
来源：http://om.gzmigu.cn

Go:   arr[1:4]
来源：http://fm.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://pc.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://kd.hahajie.cn

[D08] 合并两个数组
来源：http://nx.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://ta.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://hv.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qz.hnjuh.cn

TS:   [...a, ...b];
来源：http://wu.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zr.521024.cn

Go:   append(a, b...)
来源：http://uu.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://lp.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://yq.haigaiapp.cn

[D09] 排序（升序）
来源：http://zk.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://xp.shxzskj.cn

PHP:  sort($arr);
来源：http://wn.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://av.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ow.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xt.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uy.colortex.cn

Ruby: arr.sort
来源：http://dk.huixinmuqiang.cn

C#:   list.Sort();
来源：http://hw.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ca.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mt.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zk.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://em.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vp.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hn.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wj.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cy.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qb.huixiangedu.cn

[D11] 反转数组
来源：http://ao.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eq.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://xv.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://np.szsharing.cn

TS:   [...arr].reverse();
来源：http://qs.colortex.cn

Java: Collections.reverse(list);
来源：http://cg.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://nf.lnxyls.cn

Ruby: arr.reverse
来源：http://wl.chemitech.net.cn

C#:   list.Reverse();
来源：http://ou.szxytkj.cn

[D12] 查找元素下标
来源：http://cf.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://oh.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ln.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mq.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tm.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pb.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://dh.muxihuayi.cn

Ruby: arr.index(x)
来源：http://qx.newstarts.cn

C#:   list.IndexOf(x);
来源：http://us.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://tv.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qv.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sz.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://ge.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://lr.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xz.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ik.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ba.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mj.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://kk.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rg.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qz.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://qn.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://lt.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bb.gzmigu.cn

Go:   // 手写循环
来源：http://gp.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tu.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fe.yuexingan06.cn

[D15] 去重
来源：http://br.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sq.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://sg.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://wf.szsharing.cn

TS:   [...new Set(arr)]
来源：http://vw.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bv.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jz.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://vx.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://nj.haigaiapp.cn

[D16] 求和与平均值
来源：http://qh.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ov.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fm.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kd.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ub.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tq.shtwfgs.cn

Go:   // 手写循环累加
来源：http://mk.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yn.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://kj.gzmigu.cn

[D17] 最大值与最小值
来源：http://gz.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://hu.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://md.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rl.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://em.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ss.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sk.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://ah.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://yl.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://zd.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ff.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://qj.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uj.gzmigu.cn

TS:   nested.flat();
来源：http://mm.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://la.yuexingan06.cn

Go:   // 手写双层循环
来源：http://oq.huixiangedu.cn

Ruby: nested.flatten
来源：http://sn.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zt.huixiangedu.cn

[D19] 按字段分组
来源：http://ro.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ar.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qg.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://id.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cw.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nv.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://in.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://av.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ow.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://ad.nicolike.cn

Py:   Counter(arr)
来源：http://le.nszjky.cn

PHP:  array_count_values($arr);
来源：http://am.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ek.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xh.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ho.newstarts.cn

Go:   // 手写 map[T]int
来源：http://lz.shxzukj.cn

Ruby: arr.tally
来源：http://ej.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pu.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://xh.colortex.cn

Py:   x in arr
来源：http://pm.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://cn.nicolike.cn

JS:   arr.includes(x)
来源：http://eo.bjjhwx.cn

TS:   arr.includes(x)
来源：http://vw.lnxyls.cn

Java: list.contains(x)
来源：http://hg.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://sw.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://ck.hahajie.cn

C#:   list.Contains(x)
来源：http://ot.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://qz.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ki.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ic.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cn.shtwfgs.cn

TS:   [...arr];
来源：http://ip.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://zu.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pl.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://xc.szxytkj.cn

C#:   new List<int>(list);
来源：http://na.lnxyls.cn

[D23] reduce 累积计算
来源：http://ky.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cq.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dk.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vj.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lt.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lh.wgjwhj.cn

Go:   // 手写循环
来源：http://nw.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bk.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://nu.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qy.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hu.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cu.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ew.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hx.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xm.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ms.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jc.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://as.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eq.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://of.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dt.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kk.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://me.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mm.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eg.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qr.panjiajie.cn

[D26] 数组转字符串
来源：http://wy.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://dr.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://jb.jctech888.com.cn

JS:   arr.join(", ")
来源：http://gi.shxzskj.cn

TS:   arr.join(", ")
来源：http://nn.yuexingan06.cn

Java: String.join(", ", list)
来源：http://np.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://ek.nicolike.cn

Ruby: arr.join(", ")
来源：http://xk.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://rx.szsharing.cn

================================================================================
来源：http://no.hnjuh.cn

E. 字符串处理
来源：http://jr.nicolike.cn

================================================================================
来源：http://no.shtwfgs.cn

[E01] 拼接字符串
来源：http://bk.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ge.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://so.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ml.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://on.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ea.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vr.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nv.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lm.shxzukj.cn

[E02] 重复字符串
来源：http://cr.yuexingan06.cn

Py:   "ab" * 3
来源：http://mc.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://fc.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://zt.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://sc.huanxung.cn

Java: "ab".repeat(3)
来源：http://do.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://lt.lnxyls.cn

Ruby: "ab" * 3
来源：http://ho.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ai.yuexingan06.cn

[E03] 截取子串
来源：http://un.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sa.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rj.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xq.colortex.cn

TS:   s.slice(1, 4)
来源：http://lt.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://pp.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mg.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ja.colortex.cn

C#:   s.Substring(1, 3)
来源：http://qj.shtwfgs.cn

[E04] 查找子串位置
来源：http://zz.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://if.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://kr.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ei.huanxung.cn

TS:   s.indexOf("x")
来源：http://hv.huixiangedu.cn

Java: s.indexOf("x")
来源：http://bz.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://bu.hnjuh.cn

Ruby: s.index("x")
来源：http://sj.asd995.cn

C#:   s.IndexOf("x")
来源：http://vd.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sk.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uo.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aw.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wb.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zp.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ny.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zy.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ez.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vk.shxzukj.cn

[E06] 替换子串
来源：http://ul.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hl.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://dz.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ht.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://mh.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cw.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wt.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cm.521024.cn

C#:   s.Replace("a", "b")
来源：http://il.hahajie.cn

[E07] 按分隔符拆分
来源：http://ej.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bo.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gw.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wm.wgjwhj.cn

TS:   s.split(",")
来源：http://ty.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oy.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zs.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://jp.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sw.asd995.cn

[E08] 数组按分隔符合并
来源：http://df.huixiangedu.cn

Py:   ",".join(items)
来源：http://yi.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://xt.yuntaijiaju.cn

JS:   items.join(",")
来源：http://rh.yuntaijiaju.cn

TS:   items.join(",")
来源：http://nw.muxihuayi.cn

Java: String.join(",", items)
来源：http://pn.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://ad.panjiajie.cn

Ruby: items.join(",")
来源：http://rf.shxzskj.cn

C#:   string.Join(",", items)
来源：http://sb.asd995.cn

[E09] 去除所有空白字符
来源：http://yp.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zn.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://it.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://or.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://js.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://sd.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cm.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ka.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://om.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://sx.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ep.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tf.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://gc.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://th.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://qr.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xc.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ok.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ol.colortex.cn

[E11] 反转字符串
来源：http://il.hahajie.cn

Py:   s[::-1]
来源：http://ck.asd995.cn

PHP:  strrev($s);
来源：http://al.asd995.cn

JS:   [...s].reverse().join("")
来源：http://vn.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://kh.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aa.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hv.huanxung.cn

Ruby: s.reverse
来源：http://cv.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rv.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://pv.yuntaijiaju.cn

Py:   s.count("a")
来源：http://ch.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://iu.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://id.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://fh.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ff.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://zs.shxzukj.cn

Ruby: s.count("a")
来源：http://cv.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://zb.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://ao.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://bp.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://io.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sr.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tu.muxihuayi.cn


<!-- 参考信息 -->