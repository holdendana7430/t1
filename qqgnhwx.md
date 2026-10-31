代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://th.521024.cn

TS:   [...a, ...b];
来源：http://vh.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ra.bjjhwx.cn

Go:   append(a, b...)
来源：http://mn.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://zv.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://nd.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://mu.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://yk.szsharing.cn

PHP:  sort($arr);
来源：http://nv.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dv.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hn.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gm.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mx.gzmigu.cn

Ruby: arr.sort
来源：http://xa.huixiangedu.cn

C#:   list.Sort();
来源：http://ja.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rv.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pr.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ri.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kd.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lr.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ze.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ka.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zd.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iy.jianghongdianzi.cn

[D11] 反转数组
来源：http://cs.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cj.hahajie.cn

PHP:  array_reverse($arr);
来源：http://iz.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rb.szxytkj.cn

TS:   [...arr].reverse();
来源：http://ub.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://ee.colortex.cn

Go:   slices.Reverse(arr)
来源：http://md.shtwfgs.cn

Ruby: arr.reverse
来源：http://sn.lnxyls.cn

C#:   list.Reverse();
来源：http://ew.szxytkj.cn

[D12] 查找元素下标
来源：http://zg.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://jh.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://st.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yb.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xd.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ul.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://oi.shxzskj.cn

Ruby: arr.index(x)
来源：http://gv.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://sn.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://ao.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hw.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dw.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://di.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://bx.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xb.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wb.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lf.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kp.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://rk.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pv.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gr.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://sm.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://mw.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gc.muxihuayi.cn

Go:   // 手写循环
来源：http://rh.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jy.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qc.jctech888.com.cn

[D15] 去重
来源：http://ts.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oe.lnxyls.cn

PHP:  array_unique($arr);
来源：http://fu.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://du.9csxet.cn

TS:   [...new Set(arr)]
来源：http://ty.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jw.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zp.bookmarksfly.cn

Ruby: arr.uniq
来源：http://vh.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://kt.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://ms.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jw.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ca.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ma.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wg.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xj.asd995.cn

Go:   // 手写循环累加
来源：http://wn.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ak.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://jo.shtwfgs.cn

[D17] 最大值与最小值
来源：http://nl.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://jm.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://xp.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://am.lnxyls.cn

TS:   Math.max(...arr);
来源：http://hd.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gj.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iu.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://ae.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://ft.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://bp.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://do.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://bx.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ap.bjjhwx.cn

TS:   nested.flat();
来源：http://bd.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oy.panjiajie.cn

Go:   // 手写双层循环
来源：http://bc.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://tg.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wt.shtwfgs.cn

[D19] 按字段分组
来源：http://zn.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://um.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hf.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hh.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mi.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dp.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://cl.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hi.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vb.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://nz.panjiajie.cn

Py:   Counter(arr)
来源：http://kr.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://ep.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rw.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vu.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://rv.colortex.cn

Ruby: arr.tally
来源：http://xq.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dh.521024.cn

[D21] 判断是否包含某元素
来源：http://ga.szsharing.cn

Py:   x in arr
来源：http://bj.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://ai.panjiajie.cn

JS:   arr.includes(x)
来源：http://el.521024.cn

TS:   arr.includes(x)
来源：http://lx.bookmarksfly.cn

Java: list.contains(x)
来源：http://bj.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://td.gzmigu.cn

Ruby: arr.include?(x)
来源：http://of.yuexingan06.cn

C#:   list.Contains(x)
来源：http://pd.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://sv.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zi.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mg.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ec.muxihuayi.cn

TS:   [...arr];
来源：http://xy.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://da.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rb.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://hm.9csxet.cn

C#:   new List<int>(list);
来源：http://ho.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://gl.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lk.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://it.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nf.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xy.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rl.nicolike.cn

Go:   // 手写循环
来源：http://xw.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hd.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://od.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://yh.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yq.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bx.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bt.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xo.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wk.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ma.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nw.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hx.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://vl.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nj.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lv.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vn.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tk.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wt.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ku.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tw.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wk.szsharing.cn

[D26] 数组转字符串
来源：http://wm.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://wo.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://ya.chemitech.net.cn

JS:   arr.join(", ")
来源：http://cu.chemitech.net.cn

TS:   arr.join(", ")
来源：http://vj.shxzskj.cn

Java: String.join(", ", list)
来源：http://ts.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://me.lnxyls.cn

Ruby: arr.join(", ")
来源：http://gu.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://ba.hnjuh.cn

================================================================================
来源：http://md.szsharing.cn

E. 字符串处理
来源：http://dl.huixiangedu.cn

================================================================================
来源：http://iy.shxzskj.cn

[E01] 拼接字符串
来源：http://uy.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mb.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pv.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hn.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://id.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yv.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wf.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mq.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xh.yuntaijiaju.cn

[E02] 重复字符串
来源：http://mo.shxzskj.cn

Py:   "ab" * 3
来源：http://nw.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://ij.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://pg.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://bk.asd995.cn

Java: "ab".repeat(3)
来源：http://gw.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://oe.nszjky.cn

Ruby: "ab" * 3
来源：http://am.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uj.yuntaijiaju.cn

[E03] 截取子串
来源：http://ju.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iq.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fo.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uc.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://mv.521024.cn

Java: s.substring(1, 4)
来源：http://ek.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ll.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jw.asd995.cn

C#:   s.Substring(1, 3)
来源：http://cp.hnjuh.cn

[E04] 查找子串位置
来源：http://jd.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://ib.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://fk.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jp.hahajie.cn

TS:   s.indexOf("x")
来源：http://fi.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://ky.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://ik.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://ci.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://sb.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wd.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vs.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fm.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qr.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gk.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://by.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oh.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sh.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vi.521024.cn

[E06] 替换子串
来源：http://zu.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yq.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://vm.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gd.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://hb.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dr.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hm.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mk.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://oo.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://ph.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sw.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hw.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wx.chemitech.net.cn

TS:   s.split(",")
来源：http://db.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gs.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ck.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://xt.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jl.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://da.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://ye.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://wp.chemitech.net.cn

JS:   items.join(",")
来源：http://ti.huixiangedu.cn

TS:   items.join(",")
来源：http://aj.bjjhwx.cn

Java: String.join(",", items)
来源：http://jh.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://va.wgjwhj.cn

Ruby: items.join(",")
来源：http://il.hnjuh.cn

C#:   string.Join(",", items)
来源：http://fb.shxzskj.cn

[E09] 去除所有空白字符
来源：http://nx.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iu.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://st.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://ig.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ps.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://mk.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ul.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bj.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bl.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://gd.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://if.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mo.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://du.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://om.newstarts.cn

Java: String.format("%03d", 7)
来源：http://nx.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vf.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vn.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ef.hahajie.cn

[E11] 反转字符串
来源：http://fo.nszjky.cn

Py:   s[::-1]
来源：http://da.haigaiapp.cn

PHP:  strrev($s);
来源：http://pi.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://if.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://qh.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pk.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vm.bjjhwx.cn

Ruby: s.reverse
来源：http://pn.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pg.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://oe.9csxet.cn

Py:   s.count("a")
来源：http://pk.colortex.cn

PHP:  substr_count($s, "a");
来源：http://ed.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://pm.nicolike.cn

TS:   s.split("a").length - 1
来源：http://eg.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tw.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://gp.hnjuh.cn

Ruby: s.count("a")
来源：http://zy.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://df.shtwfgs.cn

[E13] 逐字符遍历
来源：http://xm.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://pi.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wu.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fa.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://db.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vs.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wz.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ui.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mm.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://bj.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xp.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vn.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jr.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zg.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wc.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gm.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xv.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tx.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://pt.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xm.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hg.jctech888.com.cn


<!-- 参考信息 -->