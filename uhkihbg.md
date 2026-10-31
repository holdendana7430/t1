代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://kr.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://yz.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zd.shtwfgs.cn

================================================================================
来源：http://op.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://hk.bjjhwx.cn

================================================================================
来源：http://im.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://gi.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fu.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ox.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ln.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ly.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yt.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://co.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://de.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mb.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://mh.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yz.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://li.jctech888.com.cn

JS:   arr.push(4);
来源：http://hg.haigaiapp.cn

TS:   arr.push(4);
来源：http://qv.szxytkj.cn

Java: list.add(4);
来源：http://bk.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://sr.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://to.colortex.cn

C#:   list.Add(4);
来源：http://eq.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://lr.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://jn.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fq.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pu.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://xs.nszjky.cn

Java: list.add(0, 0);
来源：http://ud.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fq.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yu.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://si.szsharing.cn

[D04] 删除元素
来源：http://ji.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sa.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://el.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zk.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://pd.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ok.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://um.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wg.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://im.jctech888.com.cn

[D05] 访问与修改元素
来源：http://zl.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ii.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wr.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fi.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://cd.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://tq.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://en.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zt.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yv.hnjuh.cn

[D06] 数组长度
来源：http://ny.chemitech.net.cn

Py:   len(arr)
来源：http://pt.jianghongdianzi.cn

PHP:  count($arr);
来源：http://ow.haigaiapp.cn

JS:   arr.length
来源：http://we.yuntaijiaju.cn

TS:   arr.length
来源：http://hb.haigaiapp.cn

Java: list.size();
来源：http://mc.wgjwhj.cn

Go:   len(arr)
来源：http://om.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://wr.nszjky.cn

C#:   list.Count;
来源：http://ig.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://xl.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mw.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mf.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://vb.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://ib.9csxet.cn

Java: list.subList(1, 4);
来源：http://yy.bjjhwx.cn

Go:   arr[1:4]
来源：http://gl.panjiajie.cn

Ruby: arr[1, 3]
来源：http://ar.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://el.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://ea.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://ca.521024.cn

PHP:  array_merge($a, $b);
来源：http://ho.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xz.hahajie.cn

TS:   [...a, ...b];
来源：http://vn.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jn.nszjky.cn

Go:   append(a, b...)
来源：http://th.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://kf.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://zy.shtwfgs.cn

[D09] 排序（升序）
来源：http://ci.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ti.bookmarksfly.cn

PHP:  sort($arr);
来源：http://aq.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yy.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hx.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tv.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kz.shxzskj.cn

Ruby: arr.sort
来源：http://xy.huanxung.cn

C#:   list.Sort();
来源：http://fr.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://za.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://af.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fk.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sy.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sm.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fg.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qr.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dl.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mr.shxzskj.cn

[D11] 反转数组
来源：http://xp.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ev.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://sf.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qq.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://tk.huanxung.cn

Java: Collections.reverse(list);
来源：http://pb.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://wb.nszjky.cn

Ruby: arr.reverse
来源：http://fr.lnxyls.cn

C#:   list.Reverse();
来源：http://ot.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://pz.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://dz.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lm.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sw.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zt.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ul.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://xe.huanxung.cn

Ruby: arr.index(x)
来源：http://nf.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://ch.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://nv.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ga.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lh.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://uf.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://fz.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ni.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xf.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oi.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ix.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://oy.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kx.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fc.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://nd.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://yr.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bs.huanxung.cn

Go:   // 手写循环
来源：http://ps.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ae.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hg.gzmigu.cn

[D15] 去重
来源：http://ju.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sy.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://vr.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://kn.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://bh.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cc.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oe.muxihuayi.cn

Ruby: arr.uniq
来源：http://pm.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://zq.colortex.cn

[D16] 求和与平均值
来源：http://bu.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xx.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wr.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ke.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pw.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ph.nicolike.cn

Go:   // 手写循环累加
来源：http://xj.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tk.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://ot.nszjky.cn

[D17] 最大值与最小值
来源：http://zf.colortex.cn

Py:   max(arr);  min(arr)
来源：http://he.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://wu.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ob.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://wm.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vb.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xc.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://lc.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://dc.521024.cn

[D18] 扁平化嵌套数组
来源：http://jy.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ge.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://nk.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ef.hahajie.cn

TS:   nested.flat();
来源：http://rk.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ii.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://lo.hahajie.cn

Ruby: nested.flatten
来源：http://yd.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://es.nszjky.cn

[D19] 按字段分组
来源：http://ea.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xn.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yj.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ir.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zw.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cl.colortex.cn

Go:   // 手写 map[string][]T
来源：http://be.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ay.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sa.asd995.cn

[D20] 统计每个元素出现次数
来源：http://cw.asd995.cn

Py:   Counter(arr)
来源：http://th.huanxung.cn

PHP:  array_count_values($arr);
来源：http://hb.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bi.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nv.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ry.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://pd.nicolike.cn

Ruby: arr.tally
来源：http://as.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lh.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://ze.nszjky.cn

Py:   x in arr
来源：http://ws.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://lp.yuexingan06.cn

JS:   arr.includes(x)
来源：http://mb.chemitech.net.cn

TS:   arr.includes(x)
来源：http://ba.hahajie.cn

Java: list.contains(x)
来源：http://rs.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://jm.gzmigu.cn

Ruby: arr.include?(x)
来源：http://jg.yuexingan06.cn

C#:   list.Contains(x)
来源：http://oz.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://ww.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://py.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vd.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ns.gzmigu.cn

TS:   [...arr];
来源：http://xj.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://gg.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ri.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://ax.521024.cn

C#:   new List<int>(list);
来源：http://ts.colortex.cn

[D23] reduce 累积计算
来源：http://yx.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zv.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dn.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rt.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zk.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mq.haigaiapp.cn

Go:   // 手写循环
来源：http://iz.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lx.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ov.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://cj.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ko.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jr.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wo.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://em.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kx.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oc.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ku.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yg.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://jt.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ct.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bk.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eg.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pa.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cl.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vi.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fz.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://au.shxzukj.cn

[D26] 数组转字符串
来源：http://ke.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://zn.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://ym.hahajie.cn

JS:   arr.join(", ")
来源：http://mh.gzmigu.cn

TS:   arr.join(", ")
来源：http://sm.9csxet.cn

Java: String.join(", ", list)
来源：http://iu.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://cl.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://to.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://qy.hahajie.cn

================================================================================
来源：http://zr.muxihuayi.cn

E. 字符串处理
来源：http://wf.shtwfgs.cn

================================================================================
来源：http://yj.hnjuh.cn

[E01] 拼接字符串
来源：http://ws.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cp.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zy.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mh.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eq.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bn.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jg.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://re.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qc.chemitech.net.cn

[E02] 重复字符串
来源：http://px.hahajie.cn

Py:   "ab" * 3
来源：http://fy.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://dc.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://gd.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://ya.shxzukj.cn

Java: "ab".repeat(3)
来源：http://as.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://xt.shxzskj.cn

Ruby: "ab" * 3
来源：http://cq.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fa.jctech888.com.cn

[E03] 截取子串
来源：http://pq.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iz.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tr.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ks.9csxet.cn

TS:   s.slice(1, 4)
来源：http://kv.shxzukj.cn

Java: s.substring(1, 4)
来源：http://gb.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pv.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pr.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://in.panjiajie.cn

[E04] 查找子串位置
来源：http://jr.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://mk.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://jc.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rz.nicolike.cn

TS:   s.indexOf("x")
来源：http://vv.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://zc.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://mz.szxytkj.cn

Ruby: s.index("x")
来源：http://tf.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://gq.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mo.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ls.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rz.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rx.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://we.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lv.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xy.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xt.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ur.haigaiapp.cn

[E06] 替换子串
来源：http://ch.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tn.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://ev.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qp.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://dc.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://we.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ka.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yp.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://ge.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://xd.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://og.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://no.hnjuh.cn


<!-- 参考信息 -->