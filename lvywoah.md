代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://ub.hnjuh.cn

Java: list.add(0, 0);
来源：http://ei.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gy.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://og.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://om.huixiangedu.cn

[D04] 删除元素
来源：http://nb.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lk.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jf.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nk.521024.cn

TS:   arr.splice(0, 1);
来源：http://ad.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xi.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tv.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vo.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://er.huanxung.cn

[D05] 访问与修改元素
来源：http://ak.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xn.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mp.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bh.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://eq.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://jl.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://tf.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lm.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ws.shxzukj.cn

[D06] 数组长度
来源：http://bd.9csxet.cn

Py:   len(arr)
来源：http://mc.jianghongdianzi.cn

PHP:  count($arr);
来源：http://iw.yuexingan06.cn

JS:   arr.length
来源：http://vg.colortex.cn

TS:   arr.length
来源：http://dc.nicolike.cn

Java: list.size();
来源：http://mq.huixinmuqiang.cn

Go:   len(arr)
来源：http://au.newstarts.cn

Ruby: arr.length; arr.size
来源：http://bq.shtwfgs.cn

C#:   list.Count;
来源：http://tr.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://bg.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dq.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wq.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://wi.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://xu.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://nx.hnjuh.cn

Go:   arr[1:4]
来源：http://gu.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://du.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://el.yuexingan06.cn

[D08] 合并两个数组
来源：http://pk.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://am.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://aw.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://az.huanxung.cn

TS:   [...a, ...b];
来源：http://ze.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tp.yuexingan06.cn

Go:   append(a, b...)
来源：http://ve.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://gp.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://ix.yuexingan06.cn

[D09] 排序（升序）
来源：http://fh.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://vq.wgjwhj.cn

PHP:  sort($arr);
来源：http://we.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sn.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ua.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yy.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ha.yuntaijiaju.cn

Ruby: arr.sort
来源：http://dz.hnjuh.cn

C#:   list.Sort();
来源：http://xe.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ki.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kh.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wq.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ig.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nx.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://an.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xa.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vc.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wf.yuntaijiaju.cn

[D11] 反转数组
来源：http://su.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://av.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://ti.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qu.colortex.cn

TS:   [...arr].reverse();
来源：http://xx.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://vg.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://zt.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://rl.haigaiapp.cn

C#:   list.Reverse();
来源：http://su.szxytkj.cn

[D12] 查找元素下标
来源：http://qa.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://yg.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pe.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ae.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rt.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://nk.huanxung.cn

Ruby: arr.index(x)
来源：http://iz.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://ta.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://ok.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://po.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://se.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://yd.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://kv.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sr.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mn.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xd.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xz.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://ud.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tg.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kr.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://nr.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://je.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ka.asd995.cn

Go:   // 手写循环
来源：http://ed.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ua.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xh.panjiajie.cn

[D15] 去重
来源：http://qe.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ps.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://aa.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://mg.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://pr.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bo.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zp.asd995.cn

Ruby: arr.uniq
来源：http://rt.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://qf.shtwfgs.cn

[D16] 求和与平均值
来源：http://ma.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qp.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nk.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rv.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://io.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pr.hahajie.cn

Go:   // 手写循环累加
来源：http://up.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hy.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://cz.shtwfgs.cn

[D17] 最大值与最小值
来源：http://ga.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://iv.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://dl.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ap.gzmigu.cn

TS:   Math.max(...arr);
来源：http://bt.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ud.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uo.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://bj.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://ix.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://ub.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fd.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://sa.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wo.yuntaijiaju.cn

TS:   nested.flat();
来源：http://rj.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xn.huixiangedu.cn

Go:   // 手写双层循环
来源：http://ph.haigaiapp.cn

Ruby: nested.flatten
来源：http://fd.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jp.hnjuh.cn

[D19] 按字段分组
来源：http://xr.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dp.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rp.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jq.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pa.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://er.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://du.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hm.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gd.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://ed.nicolike.cn

Py:   Counter(arr)
来源：http://kj.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://bt.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ar.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zf.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dx.szsharing.cn

Go:   // 手写 map[T]int
来源：http://ig.shxzskj.cn

Ruby: arr.tally
来源：http://vg.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ta.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://jl.shxzukj.cn

Py:   x in arr
来源：http://lv.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://pd.haigaiapp.cn

JS:   arr.includes(x)
来源：http://is.wgjwhj.cn

TS:   arr.includes(x)
来源：http://is.nszjky.cn

Java: list.contains(x)
来源：http://zc.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://ve.szxytkj.cn

Ruby: arr.include?(x)
来源：http://mj.colortex.cn

C#:   list.Contains(x)
来源：http://wq.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://mo.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bn.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gv.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zr.jctech888.com.cn

TS:   [...arr];
来源：http://cg.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://ku.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nw.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://pw.gzmigu.cn

C#:   new List<int>(list);
来源：http://hp.huixiangedu.cn

[D23] reduce 累积计算
来源：http://uc.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mo.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://na.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ll.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rw.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xu.bookmarksfly.cn

Go:   // 手写循环
来源：http://ro.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wd.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vx.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://mg.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hs.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bm.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xo.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xy.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wl.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qg.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://au.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mw.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://rw.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ts.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mg.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mk.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xl.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dy.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lf.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ub.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sc.huanxung.cn

[D26] 数组转字符串
来源：http://jw.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://od.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://mb.nszjky.cn

JS:   arr.join(", ")
来源：http://ln.newstarts.cn

TS:   arr.join(", ")
来源：http://kf.huanxung.cn

Java: String.join(", ", list)
来源：http://zq.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://kh.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://oa.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://ly.jianghongdianzi.cn

================================================================================
来源：http://li.521024.cn

E. 字符串处理
来源：http://oa.9csxet.cn

================================================================================
来源：http://rk.colortex.cn

[E01] 拼接字符串
来源：http://uw.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wk.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gz.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ax.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bk.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rf.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rj.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vs.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sf.nszjky.cn

[E02] 重复字符串
来源：http://me.shxzukj.cn

Py:   "ab" * 3
来源：http://kz.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://dp.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://um.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://wa.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://ky.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://df.nicolike.cn

Ruby: "ab" * 3
来源：http://jm.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dy.shxzskj.cn

[E03] 截取子串
来源：http://uv.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jt.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://no.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ob.szsharing.cn

TS:   s.slice(1, 4)
来源：http://ey.colortex.cn

Java: s.substring(1, 4)
来源：http://mb.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ef.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ex.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://rv.asd995.cn

[E04] 查找子串位置
来源：http://ys.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://df.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://rc.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ml.hnjuh.cn

TS:   s.indexOf("x")
来源：http://qb.szxytkj.cn

Java: s.indexOf("x")
来源：http://ra.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://lz.muxihuayi.cn

Ruby: s.index("x")
来源：http://fj.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://yk.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ev.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://do.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://us.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ef.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://op.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ji.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yv.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ep.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cx.nicolike.cn

[E06] 替换子串
来源：http://cn.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cn.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://yp.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://le.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://kj.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lq.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qo.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://su.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://bi.hahajie.cn

[E07] 按分隔符拆分
来源：http://ha.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ng.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gd.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ao.gzmigu.cn

TS:   s.split(",")
来源：http://mb.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wt.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vt.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://eh.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gm.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://ye.colortex.cn

Py:   ",".join(items)
来源：http://tw.shxzskj.cn

PHP:  implode(",", $items);
来源：http://yj.nicolike.cn

JS:   items.join(",")
来源：http://lb.asd995.cn

TS:   items.join(",")
来源：http://bx.bookmarksfly.cn

Java: String.join(",", items)
来源：http://kz.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://na.521024.cn

Ruby: items.join(",")
来源：http://np.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://tg.nicolike.cn

[E09] 去除所有空白字符
来源：http://pu.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://py.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fx.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://jm.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://bi.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ow.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://je.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ek.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yq.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://hr.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zz.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dz.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://ln.huixinmuqiang.cn


<!-- 参考信息 -->