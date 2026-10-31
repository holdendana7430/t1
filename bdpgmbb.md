代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://xy.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://hj.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mi.gzmigu.cn

================================================================================
来源：http://nx.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://gr.haigaiapp.cn

================================================================================
来源：http://vg.9csxet.cn

[D01] 创建数组 / 列表
来源：http://pm.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ju.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://he.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ut.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qy.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hm.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://pe.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://zi.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oc.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://jb.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tx.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hg.panjiajie.cn

JS:   arr.push(4);
来源：http://tc.jctech888.com.cn

TS:   arr.push(4);
来源：http://qa.lnxyls.cn

Java: list.add(4);
来源：http://jk.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://zb.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://rz.nszjky.cn

C#:   list.Add(4);
来源：http://vc.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://bm.521024.cn

Py:   arr.insert(0, 0)
来源：http://mx.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ax.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://na.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ug.9csxet.cn

Java: list.add(0, 0);
来源：http://fa.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ke.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vw.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://uy.haigaiapp.cn

[D04] 删除元素
来源：http://tw.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ju.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fy.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uw.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://yp.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tl.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pp.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ye.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jg.asd995.cn

[D05] 访问与修改元素
来源：http://cg.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hh.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://at.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pa.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://lr.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://fn.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://hm.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cl.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://py.wgjwhj.cn

[D06] 数组长度
来源：http://tb.jctech888.com.cn

Py:   len(arr)
来源：http://ye.szxytkj.cn

PHP:  count($arr);
来源：http://ui.hahajie.cn

JS:   arr.length
来源：http://cx.newstarts.cn

TS:   arr.length
来源：http://yq.yuntaijiaju.cn

Java: list.size();
来源：http://ao.hnjuh.cn

Go:   len(arr)
来源：http://qt.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://oi.hahajie.cn

C#:   list.Count;
来源：http://mk.huanxung.cn

[D07] 切片 / 取子数组
来源：http://kq.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://px.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ap.521024.cn

JS:   arr.slice(1, 4);
来源：http://hb.asd995.cn

TS:   arr.slice(1, 4);
来源：http://cb.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://uj.shxzskj.cn

Go:   arr[1:4]
来源：http://oa.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://zm.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://op.9csxet.cn

[D08] 合并两个数组
来源：http://gz.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://dn.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://or.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mm.muxihuayi.cn

TS:   [...a, ...b];
来源：http://lo.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gw.yuexingan06.cn

Go:   append(a, b...)
来源：http://bv.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://sh.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://rk.wgjwhj.cn

[D09] 排序（升序）
来源：http://cc.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://cs.panjiajie.cn

PHP:  sort($arr);
来源：http://sn.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://en.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mo.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eh.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jn.521024.cn

Ruby: arr.sort
来源：http://bz.bookmarksfly.cn

C#:   list.Sort();
来源：http://wm.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gi.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oi.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ch.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tn.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wd.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hg.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tc.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mq.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sy.wgjwhj.cn

[D11] 反转数组
来源：http://wa.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://co.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://ud.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rw.panjiajie.cn

TS:   [...arr].reverse();
来源：http://bd.shxzskj.cn

Java: Collections.reverse(list);
来源：http://xr.521024.cn

Go:   slices.Reverse(arr)
来源：http://ur.asd995.cn

Ruby: arr.reverse
来源：http://tw.yuexingan06.cn

C#:   list.Reverse();
来源：http://jo.huixiangedu.cn

[D12] 查找元素下标
来源：http://yn.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://xm.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vf.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yh.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vj.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gw.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://rc.asd995.cn

Ruby: arr.index(x)
来源：http://uy.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://wn.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://oq.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cl.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ax.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://vi.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://nc.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fk.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nx.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zy.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://gz.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lj.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dp.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://yy.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://im.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://be.shxzskj.cn

Go:   // 手写循环
来源：http://ej.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gn.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://em.jianghongdianzi.cn

[D15] 去重
来源：http://xq.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://at.szsharing.cn

PHP:  array_unique($arr);
来源：http://fh.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://we.nszjky.cn

TS:   [...new Set(arr)]
来源：http://yd.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rv.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sc.yuexingan06.cn

Ruby: arr.uniq
来源：http://xt.521024.cn

C#:   list.Distinct().ToList()
来源：http://ki.szsharing.cn

[D16] 求和与平均值
来源：http://ju.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bd.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sw.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wo.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qb.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://go.muxihuayi.cn

Go:   // 手写循环累加
来源：http://ff.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uf.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://vx.bjjhwx.cn

[D17] 最大值与最小值
来源：http://vw.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://se.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://ux.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zq.nicolike.cn

TS:   Math.max(...arr);
来源：http://ov.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dt.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ar.asd995.cn

Ruby: arr.max;  arr.min
来源：http://lh.colortex.cn

C#:   list.Max();  list.Min()
来源：http://gg.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://bc.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://js.asd995.cn

PHP:  array_merge(...$nested);
来源：http://ng.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ze.shtwfgs.cn

TS:   nested.flat();
来源：http://sw.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mb.bjjhwx.cn

Go:   // 手写双层循环
来源：http://ir.colortex.cn

Ruby: nested.flatten
来源：http://zu.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lr.nicolike.cn

[D19] 按字段分组
来源：http://qm.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://el.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xw.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pb.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yb.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hw.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://yv.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gz.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xl.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://zs.wgjwhj.cn

Py:   Counter(arr)
来源：http://uc.nicolike.cn

PHP:  array_count_values($arr);
来源：http://cj.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vb.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nt.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xa.huanxung.cn

Go:   // 手写 map[T]int
来源：http://ew.szsharing.cn

Ruby: arr.tally
来源：http://wy.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nf.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://px.shtwfgs.cn

Py:   x in arr
来源：http://dn.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://vn.bjjhwx.cn

JS:   arr.includes(x)
来源：http://jd.szsharing.cn

TS:   arr.includes(x)
来源：http://yx.wgjwhj.cn

Java: list.contains(x)
来源：http://qf.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://js.szsharing.cn

Ruby: arr.include?(x)
来源：http://uv.panjiajie.cn

C#:   list.Contains(x)
来源：http://sg.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://bx.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ws.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ia.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fe.newstarts.cn

TS:   [...arr];
来源：http://og.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://ke.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ob.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://ql.gzmigu.cn

C#:   new List<int>(list);
来源：http://sb.muxihuayi.cn

[D23] reduce 累积计算
来源：http://ba.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sp.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://if.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wl.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wx.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gr.bjjhwx.cn

Go:   // 手写循环
来源：http://nh.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://as.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mp.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://nr.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dv.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://co.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oi.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vz.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://he.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vm.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bz.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://py.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://bw.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mf.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xv.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bx.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vn.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zn.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://si.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dm.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kr.bjjhwx.cn

[D26] 数组转字符串
来源：http://io.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://tq.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://gk.9csxet.cn

JS:   arr.join(", ")
来源：http://zn.asd995.cn

TS:   arr.join(", ")
来源：http://sj.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://uc.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://ho.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://hd.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://mt.huixiangedu.cn

================================================================================
来源：http://ay.jctech888.com.cn

E. 字符串处理
来源：http://bq.panjiajie.cn

================================================================================
来源：http://ru.asd995.cn

[E01] 拼接字符串
来源：http://cc.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rw.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sp.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wo.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qz.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cr.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jl.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zm.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eg.yuntaijiaju.cn

[E02] 重复字符串
来源：http://ou.colortex.cn

Py:   "ab" * 3
来源：http://rk.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://fn.hahajie.cn

JS:   "ab".repeat(3)
来源：http://gf.colortex.cn

TS:   "ab".repeat(3)
来源：http://xd.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://cg.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://bh.nszjky.cn

Ruby: "ab" * 3
来源：http://ud.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mw.jctech888.com.cn

[E03] 截取子串
来源：http://fo.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wa.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nd.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gm.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://wv.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://jl.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oj.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ro.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://vj.szsharing.cn

[E04] 查找子串位置
来源：http://ut.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://pd.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://hn.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://df.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://so.haigaiapp.cn

Java: s.indexOf("x")
来源：http://kn.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://rw.hahajie.cn

Ruby: s.index("x")
来源：http://ux.9csxet.cn

C#:   s.IndexOf("x")
来源：http://ab.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mw.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ez.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ot.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rb.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pt.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sp.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gd.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ox.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ul.huixiangedu.cn

[E06] 替换子串
来源：http://bd.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mz.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ug.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uw.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://hs.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mf.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wz.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vl.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://dc.gzmigu.cn

[E07] 按分隔符拆分
来源：http://qn.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xf.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yw.9csxet.cn


<!-- 参考信息 -->