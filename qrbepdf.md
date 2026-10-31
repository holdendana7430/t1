代发 wailian999

C#:   list.Insert(0, 0);
来源：http://go.jctech888.com.cn

[D04] 删除元素
来源：http://ip.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://na.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sk.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sp.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://mg.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ye.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cu.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qr.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kp.newstarts.cn

[D05] 访问与修改元素
来源：http://uq.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ge.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cl.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dj.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://oz.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://vy.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://gs.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://he.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nm.bookmarksfly.cn

[D06] 数组长度
来源：http://xa.jctech888.com.cn

Py:   len(arr)
来源：http://ek.yuntaijiaju.cn

PHP:  count($arr);
来源：http://ka.szxytkj.cn

JS:   arr.length
来源：http://ux.bjjhwx.cn

TS:   arr.length
来源：http://oj.szsharing.cn

Java: list.size();
来源：http://mj.colortex.cn

Go:   len(arr)
来源：http://jb.szsharing.cn

Ruby: arr.length; arr.size
来源：http://ea.asd995.cn

C#:   list.Count;
来源：http://fe.newstarts.cn

[D07] 切片 / 取子数组
来源：http://rw.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ks.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ds.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://ws.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://tl.shxzukj.cn

Java: list.subList(1, 4);
来源：http://jy.bjjhwx.cn

Go:   arr[1:4]
来源：http://fm.huanxung.cn

Ruby: arr[1, 3]
来源：http://gz.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ab.shxzskj.cn

[D08] 合并两个数组
来源：http://oe.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://vb.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://oo.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qp.jctech888.com.cn

TS:   [...a, ...b];
来源：http://mr.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yh.shxzskj.cn

Go:   append(a, b...)
来源：http://zt.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://qz.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://hv.bookmarksfly.cn

[D09] 排序（升序）
来源：http://nw.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://fg.szsharing.cn

PHP:  sort($arr);
来源：http://vk.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://as.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mk.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ho.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qg.haigaiapp.cn

Ruby: arr.sort
来源：http://gr.lnxyls.cn

C#:   list.Sort();
来源：http://fo.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mt.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cn.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ja.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mm.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fh.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://if.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wj.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wa.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rf.chemitech.net.cn

[D11] 反转数组
来源：http://oy.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ig.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://ia.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ad.asd995.cn

TS:   [...arr].reverse();
来源：http://bo.asd995.cn

Java: Collections.reverse(list);
来源：http://ii.asd995.cn

Go:   slices.Reverse(arr)
来源：http://pk.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://pu.muxihuayi.cn

C#:   list.Reverse();
来源：http://wp.szsharing.cn

[D12] 查找元素下标
来源：http://ia.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://uu.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://br.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bs.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sn.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://km.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://km.shtwfgs.cn

Ruby: arr.index(x)
来源：http://dj.9csxet.cn

C#:   list.IndexOf(x);
来源：http://nh.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://ax.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ss.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sl.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://fi.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://cx.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wf.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cx.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://so.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kc.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://eq.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nq.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cg.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://ki.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://bc.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://or.521024.cn

Go:   // 手写循环
来源：http://mj.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wj.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pj.nicolike.cn

[D15] 去重
来源：http://pm.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://df.hahajie.cn

PHP:  array_unique($arr);
来源：http://uv.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://ud.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://if.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wk.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nh.nszjky.cn

Ruby: arr.uniq
来源：http://lg.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://dg.haigaiapp.cn

[D16] 求和与平均值
来源：http://oq.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ig.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mu.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rf.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://es.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zy.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://pz.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kb.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://fn.gzmigu.cn

[D17] 最大值与最小值
来源：http://ny.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://nl.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://ro.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oy.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://ig.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fh.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bc.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://fl.colortex.cn

C#:   list.Max();  list.Min()
来源：http://di.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://vg.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xe.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://ff.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eh.colortex.cn

TS:   nested.flat();
来源：http://ip.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cu.jctech888.com.cn

Go:   // 手写双层循环
来源：http://wl.9csxet.cn

Ruby: nested.flatten
来源：http://sf.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cf.chemitech.net.cn

[D19] 按字段分组
来源：http://nr.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hn.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://br.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tn.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gg.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kp.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://qy.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://es.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://vd.shxzskj.cn

Py:   Counter(arr)
来源：http://eg.newstarts.cn

PHP:  array_count_values($arr);
来源：http://xc.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wz.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pp.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ai.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://go.yuntaijiaju.cn

Ruby: arr.tally
来源：http://nn.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mw.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://sm.szxytkj.cn

Py:   x in arr
来源：http://ke.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://oa.bjjhwx.cn

JS:   arr.includes(x)
来源：http://ha.szsharing.cn

TS:   arr.includes(x)
来源：http://mh.bookmarksfly.cn

Java: list.contains(x)
来源：http://ix.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://vn.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://gi.hahajie.cn

C#:   list.Contains(x)
来源：http://mj.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://iw.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lu.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yu.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mp.shxzukj.cn

TS:   [...arr];
来源：http://vf.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://yy.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iv.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://zg.panjiajie.cn

C#:   new List<int>(list);
来源：http://im.nicolike.cn

[D23] reduce 累积计算
来源：http://el.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pm.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gm.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nn.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rh.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ju.521024.cn

Go:   // 手写循环
来源：http://er.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bp.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sd.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://lb.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fn.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ef.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ng.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dt.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zj.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ux.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mp.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vg.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://fy.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qo.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rc.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ob.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mi.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dd.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tq.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uo.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kp.wgjwhj.cn

[D26] 数组转字符串
来源：http://ey.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://sv.colortex.cn

PHP:  implode(", ", $arr);
来源：http://nb.wgjwhj.cn

JS:   arr.join(", ")
来源：http://ve.jctech888.com.cn

TS:   arr.join(", ")
来源：http://ng.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://ey.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://gw.hnjuh.cn

Ruby: arr.join(", ")
来源：http://wn.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://kh.huanxung.cn

================================================================================
来源：http://yr.colortex.cn

E. 字符串处理
来源：http://aw.muxihuayi.cn

================================================================================
来源：http://bp.bjjhwx.cn

[E01] 拼接字符串
来源：http://ux.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qs.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xa.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vx.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ux.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zh.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cw.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nt.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mq.hahajie.cn

[E02] 重复字符串
来源：http://yv.bjjhwx.cn

Py:   "ab" * 3
来源：http://si.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://sm.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://ck.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://dv.szsharing.cn

Java: "ab".repeat(3)
来源：http://is.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://qh.lnxyls.cn

Ruby: "ab" * 3
来源：http://bk.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gb.huanxung.cn

[E03] 截取子串
来源：http://my.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iy.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://va.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zq.asd995.cn

TS:   s.slice(1, 4)
来源：http://vu.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://dj.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ci.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pt.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://zq.chemitech.net.cn

[E04] 查找子串位置
来源：http://ms.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://sn.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://em.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kr.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://ac.asd995.cn

Java: s.indexOf("x")
来源：http://ql.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://nx.huanxung.cn

Ruby: s.index("x")
来源：http://tv.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://id.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sc.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ls.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://td.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ug.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ox.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ew.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fb.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fh.gzmigu.cn

[E06] 替换子串
来源：http://lq.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qa.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://jw.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vw.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://xo.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ex.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://af.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ab.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://vh.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://ka.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fm.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://em.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fg.szsharing.cn

TS:   s.split(",")
来源：http://gg.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://la.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nl.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://ez.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rt.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://nw.panjiajie.cn

Py:   ",".join(items)
来源：http://pe.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://ti.huixinmuqiang.cn

JS:   items.join(",")
来源：http://av.shxzskj.cn

TS:   items.join(",")
来源：http://im.521024.cn

Java: String.join(",", items)
来源：http://mp.asd995.cn

Go:   strings.Join(items, ",")
来源：http://ci.jctech888.com.cn

Ruby: items.join(",")
来源：http://vk.nicolike.cn

C#:   string.Join(",", items)
来源：http://fb.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://hw.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wk.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ug.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://sq.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://ri.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://kr.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vw.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sv.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yj.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://ab.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dw.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hh.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://bt.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://te.szsharing.cn

Java: String.format("%03d", 7)
来源：http://ej.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://no.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ab.bookmarksfly.cn


<!-- 参考信息 -->