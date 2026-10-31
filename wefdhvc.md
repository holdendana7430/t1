代发 wailian999

TS:   arr.slice(1, 4);
来源：http://pm.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://bn.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://qo.asd995.cn

Ruby: arr[1, 3]
来源：http://un.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://ha.bookmarksfly.cn

[D08] 合并两个数组
来源：http://wh.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://ay.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://tu.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zj.jctech888.com.cn

TS:   [...a, ...b];
来源：http://zd.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gt.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://ix.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://ok.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://ue.szsharing.cn

[D09] 排序（升序）
来源：http://uh.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://ud.muxihuayi.cn

PHP:  sort($arr);
来源：http://py.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wt.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tg.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gf.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oc.shxzukj.cn

Ruby: arr.sort
来源：http://kj.9csxet.cn

C#:   list.Sort();
来源：http://oo.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qy.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hx.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pc.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nb.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mq.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jz.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ts.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pb.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mg.asd995.cn

[D11] 反转数组
来源：http://an.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ks.hahajie.cn

PHP:  array_reverse($arr);
来源：http://yl.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ze.szxytkj.cn

TS:   [...arr].reverse();
来源：http://ao.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://cs.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://uv.nicolike.cn

Ruby: arr.reverse
来源：http://zr.hnjuh.cn

C#:   list.Reverse();
来源：http://kk.shtwfgs.cn

[D12] 查找元素下标
来源：http://vx.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://xd.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vs.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://db.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ad.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pg.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://xn.panjiajie.cn

Ruby: arr.index(x)
来源：http://zv.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://de.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://ib.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ug.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wn.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://es.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://ts.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tj.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kx.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ax.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bd.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://rl.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rr.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jx.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://qt.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://jv.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ot.colortex.cn

Go:   // 手写循环
来源：http://lt.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hu.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bo.wgjwhj.cn

[D15] 去重
来源：http://wd.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xu.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://ev.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://re.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://oe.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://we.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lm.huanxung.cn

Ruby: arr.uniq
来源：http://rv.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://jl.huixiangedu.cn

[D16] 求和与平均值
来源：http://gv.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bj.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yc.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rt.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kv.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lx.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://ni.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jb.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://xu.shxzukj.cn

[D17] 最大值与最小值
来源：http://bb.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://pk.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://ua.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rf.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://uf.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xk.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zt.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://he.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://io.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://ir.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yn.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://ee.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ne.huixinmuqiang.cn

TS:   nested.flat();
来源：http://gi.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ue.shtwfgs.cn

Go:   // 手写双层循环
来源：http://lc.shxzukj.cn

Ruby: nested.flatten
来源：http://tg.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ty.nszjky.cn

[D19] 按字段分组
来源：http://yx.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hn.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iq.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qm.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tw.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yv.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://bx.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rr.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vb.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://hy.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://eb.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://zk.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ps.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oi.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://am.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://df.gzmigu.cn

Ruby: arr.tally
来源：http://sg.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yb.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://jv.newstarts.cn

Py:   x in arr
来源：http://az.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://pr.nicolike.cn

JS:   arr.includes(x)
来源：http://xg.shtwfgs.cn

TS:   arr.includes(x)
来源：http://kb.yuntaijiaju.cn

Java: list.contains(x)
来源：http://ie.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://av.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://pq.colortex.cn

C#:   list.Contains(x)
来源：http://cx.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://nj.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sk.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eo.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://po.jctech888.com.cn

TS:   [...arr];
来源：http://ad.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://ae.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cy.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://vd.lnxyls.cn

C#:   new List<int>(list);
来源：http://ye.hahajie.cn

[D23] reduce 累积计算
来源：http://dt.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rs.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gp.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yw.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://si.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gu.bjjhwx.cn

Go:   // 手写循环
来源：http://xj.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://st.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xh.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://gf.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xa.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kn.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bu.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cq.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://to.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jv.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qi.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bm.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://ju.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wo.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ov.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zn.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ac.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ab.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vt.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vj.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://px.bjjhwx.cn

[D26] 数组转字符串
来源：http://tp.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://xu.asd995.cn

PHP:  implode(", ", $arr);
来源：http://dz.hnjuh.cn

JS:   arr.join(", ")
来源：http://xe.panjiajie.cn

TS:   arr.join(", ")
来源：http://ya.colortex.cn

Java: String.join(", ", list)
来源：http://un.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://gb.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://jj.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://kp.bookmarksfly.cn

================================================================================
来源：http://ka.bjjhwx.cn

E. 字符串处理
来源：http://tr.newstarts.cn

================================================================================
来源：http://pw.nszjky.cn

[E01] 拼接字符串
来源：http://wl.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hw.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://io.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lt.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://by.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cc.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ux.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vo.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pw.colortex.cn

[E02] 重复字符串
来源：http://cf.shxzukj.cn

Py:   "ab" * 3
来源：http://wz.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://iz.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://ki.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://sp.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://aw.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://ew.nicolike.cn

Ruby: "ab" * 3
来源：http://ma.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cj.szsharing.cn

[E03] 截取子串
来源：http://ip.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lm.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hj.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sp.szsharing.cn

TS:   s.slice(1, 4)
来源：http://uu.colortex.cn

Java: s.substring(1, 4)
来源：http://gh.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ul.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pz.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://jl.szxytkj.cn

[E04] 查找子串位置
来源：http://kr.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://yx.9csxet.cn

PHP:  strpos($s, "x");
来源：http://nm.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wr.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://gc.wgjwhj.cn

Java: s.indexOf("x")
来源：http://pe.521024.cn

Go:   strings.Index(s, "x")
来源：http://il.nicolike.cn

Ruby: s.index("x")
来源：http://qi.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://ps.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gm.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zk.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ja.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aa.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iu.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xy.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gv.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vd.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ob.bookmarksfly.cn

[E06] 替换子串
来源：http://wp.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fu.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://hz.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dv.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://bm.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kw.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://je.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uy.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://hy.panjiajie.cn

[E07] 按分隔符拆分
来源：http://km.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://to.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://li.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uc.521024.cn

TS:   s.split(",")
来源：http://qm.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dx.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eq.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://en.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jx.nicolike.cn

[E08] 数组按分隔符合并
来源：http://na.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://lh.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://dz.hahajie.cn

JS:   items.join(",")
来源：http://yy.yuexingan06.cn

TS:   items.join(",")
来源：http://do.nszjky.cn

Java: String.join(",", items)
来源：http://ev.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://vj.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://yd.shxzukj.cn

C#:   string.Join(",", items)
来源：http://ag.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://kq.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wo.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gf.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://cy.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://gl.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://uu.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ob.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fo.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://km.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://ws.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ad.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://os.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://hz.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://vm.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://cz.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cc.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vr.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lq.bookmarksfly.cn

[E11] 反转字符串
来源：http://js.hahajie.cn

Py:   s[::-1]
来源：http://rn.haigaiapp.cn

PHP:  strrev($s);
来源：http://gd.asd995.cn

JS:   [...s].reverse().join("")
来源：http://am.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://kl.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iq.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tt.nszjky.cn

Ruby: s.reverse
来源：http://gv.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gf.521024.cn

[E12] 统计某字符出现次数
来源：http://ib.haigaiapp.cn

Py:   s.count("a")
来源：http://ew.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://kl.colortex.cn

JS:   s.split("a").length - 1
来源：http://li.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://qb.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eo.521024.cn

Go:   strings.Count(s, "a")
来源：http://et.521024.cn

Ruby: s.count("a")
来源：http://jl.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://qc.asd995.cn

[E13] 逐字符遍历
来源：http://xu.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://oj.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fr.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bm.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://an.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gv.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qm.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ia.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ys.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://dk.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lg.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lc.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kw.nszjky.cn


<!-- 参考信息 -->