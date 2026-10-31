代发 wailian999

[D07] 切片 / 取子数组
来源：http://yx.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ot.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ig.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://wh.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://sg.colortex.cn

Java: list.subList(1, 4);
来源：http://cx.shxzskj.cn

Go:   arr[1:4]
来源：http://mn.521024.cn

Ruby: arr[1, 3]
来源：http://fv.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://cu.yuexingan06.cn

[D08] 合并两个数组
来源：http://ta.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://xt.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://yj.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jr.9csxet.cn

TS:   [...a, ...b];
来源：http://ge.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hj.hnjuh.cn

Go:   append(a, b...)
来源：http://zq.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://xz.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://rr.colortex.cn

[D09] 排序（升序）
来源：http://xv.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://pv.shxzukj.cn

PHP:  sort($arr);
来源：http://xk.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://he.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ka.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wd.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sb.jianghongdianzi.cn

Ruby: arr.sort
来源：http://tz.gzmigu.cn

C#:   list.Sort();
来源：http://at.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rw.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zm.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vj.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bb.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sy.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bp.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rx.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dj.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eg.jctech888.com.cn

[D11] 反转数组
来源：http://ww.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tu.asd995.cn

PHP:  array_reverse($arr);
来源：http://yq.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kb.huanxung.cn

TS:   [...arr].reverse();
来源：http://mu.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://he.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://qv.chemitech.net.cn

Ruby: arr.reverse
来源：http://vk.muxihuayi.cn

C#:   list.Reverse();
来源：http://ju.hnjuh.cn

[D12] 查找元素下标
来源：http://lx.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://iy.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ga.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ht.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ul.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://qy.shxzskj.cn

Ruby: arr.index(x)
来源：http://pu.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://to.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://hh.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vu.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kf.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://tl.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://fb.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zb.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ri.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qh.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gh.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://kg.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kn.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mr.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://sm.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://yx.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wt.shtwfgs.cn

Go:   // 手写循环
来源：http://nw.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yu.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sw.shxzukj.cn

[D15] 去重
来源：http://lu.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ym.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://zh.newstarts.cn

JS:   [...new Set(arr)]
来源：http://yi.huanxung.cn

TS:   [...new Set(arr)]
来源：http://nu.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nf.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eu.gzmigu.cn

Ruby: arr.uniq
来源：http://qy.asd995.cn

C#:   list.Distinct().ToList()
来源：http://lc.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://gt.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eb.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vv.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://at.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://so.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ca.shtwfgs.cn

Go:   // 手写循环累加
来源：http://qm.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rz.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://yi.lnxyls.cn

[D17] 最大值与最小值
来源：http://vo.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://wy.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://ec.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ku.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://kq.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yb.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oh.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://rl.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://mm.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://hr.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fj.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://gp.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pn.hnjuh.cn

TS:   nested.flat();
来源：http://pn.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yi.newstarts.cn

Go:   // 手写双层循环
来源：http://zx.521024.cn

Ruby: nested.flatten
来源：http://nu.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ur.shxzukj.cn

[D19] 按字段分组
来源：http://vf.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cb.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zz.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hg.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hm.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zs.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://ms.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vl.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://on.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://go.nicolike.cn

Py:   Counter(arr)
来源：http://gr.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://xd.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ju.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zy.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://je.szsharing.cn

Go:   // 手写 map[T]int
来源：http://pe.colortex.cn

Ruby: arr.tally
来源：http://ax.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jz.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://lu.chemitech.net.cn

Py:   x in arr
来源：http://cv.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://hi.yuexingan06.cn

JS:   arr.includes(x)
来源：http://qe.hahajie.cn

TS:   arr.includes(x)
来源：http://ba.yuexingan06.cn

Java: list.contains(x)
来源：http://vq.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://fh.hahajie.cn

Ruby: arr.include?(x)
来源：http://oh.shxzukj.cn

C#:   list.Contains(x)
来源：http://di.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://wf.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://af.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jc.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://am.jctech888.com.cn

TS:   [...arr];
来源：http://lv.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://im.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ek.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://df.hnjuh.cn

C#:   new List<int>(list);
来源：http://ry.chemitech.net.cn

[D23] reduce 累积计算
来源：http://zx.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://np.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ej.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qk.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wr.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uo.chemitech.net.cn

Go:   // 手写循环
来源：http://ci.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://op.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sg.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://il.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yy.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rp.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yz.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rq.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://br.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zf.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bq.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bd.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://xv.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wg.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xa.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ns.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uh.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vd.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rs.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nx.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fu.nicolike.cn

[D26] 数组转字符串
来源：http://at.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://wf.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://yd.521024.cn

JS:   arr.join(", ")
来源：http://ec.shxzskj.cn

TS:   arr.join(", ")
来源：http://ph.szsharing.cn

Java: String.join(", ", list)
来源：http://va.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://rt.9csxet.cn

Ruby: arr.join(", ")
来源：http://tr.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://ol.muxihuayi.cn

================================================================================
来源：http://xf.lnxyls.cn

E. 字符串处理
来源：http://eo.nszjky.cn

================================================================================
来源：http://od.shtwfgs.cn

[E01] 拼接字符串
来源：http://qv.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kb.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://if.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gh.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yb.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ah.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wr.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lg.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pp.nszjky.cn

[E02] 重复字符串
来源：http://ti.colortex.cn

Py:   "ab" * 3
来源：http://hc.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://gy.hahajie.cn

JS:   "ab".repeat(3)
来源：http://pe.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://ax.asd995.cn

Java: "ab".repeat(3)
来源：http://nv.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://gi.bjjhwx.cn

Ruby: "ab" * 3
来源：http://va.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pu.bookmarksfly.cn

[E03] 截取子串
来源：http://wo.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zd.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://el.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uc.nszjky.cn

TS:   s.slice(1, 4)
来源：http://wh.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://rs.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ap.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://up.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://gh.gzmigu.cn

[E04] 查找子串位置
来源：http://yy.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://jz.szsharing.cn

PHP:  strpos($s, "x");
来源：http://av.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://co.nicolike.cn

TS:   s.indexOf("x")
来源：http://zs.chemitech.net.cn

Java: s.indexOf("x")
来源：http://tw.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://zn.jctech888.com.cn

Ruby: s.index("x")
来源：http://vy.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://hr.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qj.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ef.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://px.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bh.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oc.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dv.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ca.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://es.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qp.gzmigu.cn

[E06] 替换子串
来源：http://it.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ca.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://wl.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gc.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://rq.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qo.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hm.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://po.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://jh.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://ux.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ad.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nz.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://om.521024.cn

TS:   s.split(",")
来源：http://te.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qw.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vo.asd995.cn

Ruby: s.split(",");  s.split
来源：http://pt.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ia.nicolike.cn

[E08] 数组按分隔符合并
来源：http://fg.9csxet.cn

Py:   ",".join(items)
来源：http://ch.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://bt.yuexingan06.cn

JS:   items.join(",")
来源：http://zg.yuntaijiaju.cn

TS:   items.join(",")
来源：http://nf.nszjky.cn

Java: String.join(",", items)
来源：http://fw.521024.cn

Go:   strings.Join(items, ",")
来源：http://te.shxzukj.cn

Ruby: items.join(",")
来源：http://zj.szxytkj.cn

C#:   string.Join(",", items)
来源：http://se.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://iw.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nw.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ud.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://gh.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://uo.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://uz.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pj.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dl.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cg.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://nj.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://si.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fo.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://dl.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ou.colortex.cn

Java: String.format("%03d", 7)
来源：http://no.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yq.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zy.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lh.shxzskj.cn

[E11] 反转字符串
来源：http://zu.nszjky.cn

Py:   s[::-1]
来源：http://cr.hnjuh.cn

PHP:  strrev($s);
来源：http://st.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://ib.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://ai.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ec.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wn.shxzukj.cn

Ruby: s.reverse
来源：http://sn.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bw.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://gp.wgjwhj.cn

Py:   s.count("a")
来源：http://gj.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://ur.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://qx.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://fu.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ar.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://xd.szxytkj.cn

Ruby: s.count("a")
来源：http://ny.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://ts.521024.cn

[E13] 逐字符遍历
来源：http://da.521024.cn

Py:   for ch in s: print(ch)
来源：http://fe.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zq.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zl.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xz.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kq.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hm.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://di.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sr.yuntaijiaju.cn


<!-- 参考信息 -->