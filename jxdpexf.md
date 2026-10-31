代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://ty.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://eq.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qo.wgjwhj.cn

================================================================================
来源：http://aa.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://tc.nicolike.cn

================================================================================
来源：http://mi.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://oq.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gl.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fp.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yk.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ow.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nr.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://pj.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://hf.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xz.521024.cn

[D02] 追加元素到末尾
来源：http://uz.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ce.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nl.shtwfgs.cn

JS:   arr.push(4);
来源：http://ka.hnjuh.cn

TS:   arr.push(4);
来源：http://vq.lnxyls.cn

Java: list.add(4);
来源：http://ha.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://mp.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://fu.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://du.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://fu.521024.cn

Py:   arr.insert(0, 0)
来源：http://pu.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://if.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://is.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://rq.lnxyls.cn

Java: list.add(0, 0);
来源：http://uu.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cl.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cb.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ms.bjjhwx.cn

[D04] 删除元素
来源：http://jj.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bt.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uv.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rf.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://rr.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fm.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://he.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ed.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kh.szsharing.cn

[D05] 访问与修改元素
来源：http://po.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rr.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cw.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yf.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://oh.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://wn.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://ff.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://br.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hc.newstarts.cn

[D06] 数组长度
来源：http://ss.shtwfgs.cn

Py:   len(arr)
来源：http://ub.huixiangedu.cn

PHP:  count($arr);
来源：http://ao.yuntaijiaju.cn

JS:   arr.length
来源：http://ej.jianghongdianzi.cn

TS:   arr.length
来源：http://wu.muxihuayi.cn

Java: list.size();
来源：http://bs.shxzukj.cn

Go:   len(arr)
来源：http://tp.9csxet.cn

Ruby: arr.length; arr.size
来源：http://xo.jctech888.com.cn

C#:   list.Count;
来源：http://wa.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://do.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dr.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vs.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://nc.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://lv.panjiajie.cn

Java: list.subList(1, 4);
来源：http://ho.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://ti.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://rw.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://sh.521024.cn

[D08] 合并两个数组
来源：http://yd.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://lw.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://ge.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://on.521024.cn

TS:   [...a, ...b];
来源：http://zc.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gw.nszjky.cn

Go:   append(a, b...)
来源：http://jl.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://rv.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://hu.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://zo.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://lc.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://nx.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ey.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mk.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dy.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zy.bjjhwx.cn

Ruby: arr.sort
来源：http://bt.panjiajie.cn

C#:   list.Sort();
来源：http://ks.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ph.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://by.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vm.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ao.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tw.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ar.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://op.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mp.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dg.colortex.cn

[D11] 反转数组
来源：http://ga.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ty.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://zu.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ee.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://ew.shxzskj.cn

Java: Collections.reverse(list);
来源：http://zi.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://tu.yuexingan06.cn

Ruby: arr.reverse
来源：http://mm.szxytkj.cn

C#:   list.Reverse();
来源：http://nh.bookmarksfly.cn

[D12] 查找元素下标
来源：http://ti.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://zj.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jl.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kn.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ds.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eb.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://wp.bjjhwx.cn

Ruby: arr.index(x)
来源：http://lo.newstarts.cn

C#:   list.IndexOf(x);
来源：http://sb.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://pl.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pm.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rk.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://ol.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://yq.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lj.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://an.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kk.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nw.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://vt.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ea.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://se.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://vv.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://gn.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uk.chemitech.net.cn

Go:   // 手写循环
来源：http://zt.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yt.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qf.shxzskj.cn

[D15] 去重
来源：http://eu.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mi.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://le.szsharing.cn

JS:   [...new Set(arr)]
来源：http://io.huanxung.cn

TS:   [...new Set(arr)]
来源：http://um.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yb.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kv.szxytkj.cn

Ruby: arr.uniq
来源：http://zr.asd995.cn

C#:   list.Distinct().ToList()
来源：http://mg.jctech888.com.cn

[D16] 求和与平均值
来源：http://ie.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gh.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ca.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://af.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zn.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gd.jctech888.com.cn

Go:   // 手写循环累加
来源：http://aw.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wg.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://in.jctech888.com.cn

[D17] 最大值与最小值
来源：http://qd.colortex.cn

Py:   max(arr);  min(arr)
来源：http://wg.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://ff.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://em.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://vc.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gf.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bm.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://mn.521024.cn

C#:   list.Max();  list.Min()
来源：http://ln.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://hb.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mu.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://du.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cx.huanxung.cn

TS:   nested.flat();
来源：http://fw.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ne.hahajie.cn

Go:   // 手写双层循环
来源：http://gh.huanxung.cn

Ruby: nested.flatten
来源：http://oy.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://be.huanxung.cn

[D19] 按字段分组
来源：http://yo.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nf.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nc.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zq.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ip.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fj.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://cy.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xc.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://se.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://wr.bookmarksfly.cn

Py:   Counter(arr)
来源：http://jz.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://gy.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ia.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xt.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://so.asd995.cn

Go:   // 手写 map[T]int
来源：http://oh.bjjhwx.cn

Ruby: arr.tally
来源：http://er.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lr.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://da.nicolike.cn

Py:   x in arr
来源：http://me.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://so.colortex.cn

JS:   arr.includes(x)
来源：http://dg.wgjwhj.cn

TS:   arr.includes(x)
来源：http://rt.hahajie.cn

Java: list.contains(x)
来源：http://rn.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://lq.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://wk.shxzukj.cn

C#:   list.Contains(x)
来源：http://ed.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://ur.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://id.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hs.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mw.jianghongdianzi.cn

TS:   [...arr];
来源：http://vb.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://sm.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zl.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://ez.hnjuh.cn

C#:   new List<int>(list);
来源：http://lq.shxzskj.cn

[D23] reduce 累积计算
来源：http://ku.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wl.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ds.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fa.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jh.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://td.shxzskj.cn

Go:   // 手写循环
来源：http://zf.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ai.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://im.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://yc.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nu.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ww.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sp.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xq.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gj.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zx.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tk.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ep.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://fz.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yn.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ga.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wm.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pn.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sf.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mg.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lm.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cg.huanxung.cn

[D26] 数组转字符串
来源：http://tg.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://et.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://ma.hahajie.cn

JS:   arr.join(", ")
来源：http://te.szsharing.cn

TS:   arr.join(", ")
来源：http://db.newstarts.cn

Java: String.join(", ", list)
来源：http://xa.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://mw.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://gf.nszjky.cn

C#:   string.Join(", ", list)
来源：http://az.jianghongdianzi.cn

================================================================================
来源：http://qx.asd995.cn

E. 字符串处理
来源：http://ft.shxzskj.cn

================================================================================
来源：http://vz.szxytkj.cn

[E01] 拼接字符串
来源：http://gz.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wx.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ud.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cs.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tu.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hu.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sa.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wr.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fn.shxzukj.cn

[E02] 重复字符串
来源：http://ys.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://zw.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://fe.newstarts.cn

JS:   "ab".repeat(3)
来源：http://qg.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://vf.shxzukj.cn

Java: "ab".repeat(3)
来源：http://zu.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://dj.chemitech.net.cn

Ruby: "ab" * 3
来源：http://vm.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qh.haigaiapp.cn

[E03] 截取子串
来源：http://wk.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yb.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wx.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yt.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://mx.nicolike.cn

Java: s.substring(1, 4)
来源：http://bl.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vh.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lo.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://gy.colortex.cn

[E04] 查找子串位置
来源：http://wa.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://te.521024.cn

PHP:  strpos($s, "x");
来源：http://mq.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ql.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://rx.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://mm.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://so.521024.cn

Ruby: s.index("x")
来源：http://bq.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://kf.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nd.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sz.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ih.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vt.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ut.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oj.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ti.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vn.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sf.szsharing.cn

[E06] 替换子串
来源：http://zh.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sl.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://uq.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://et.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://iy.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kz.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://co.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oo.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://kd.panjiajie.cn

[E07] 按分隔符拆分
来源：http://nv.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yu.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rl.bjjhwx.cn


<!-- 参考信息 -->