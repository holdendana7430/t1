代发 wailian999

PHP:  // 无重载
来源：http://da.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://up.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://lw.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vb.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://so.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://wk.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gs.shtwfgs.cn

================================================================================
来源：http://qn.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://jt.shtwfgs.cn

================================================================================
来源：http://op.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://gz.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uh.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qf.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ff.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ys.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wi.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://dw.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://id.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ap.hnjuh.cn

[D02] 追加元素到末尾
来源：http://no.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nd.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pq.asd995.cn

JS:   arr.push(4);
来源：http://qj.nszjky.cn

TS:   arr.push(4);
来源：http://zx.yuntaijiaju.cn

Java: list.add(4);
来源：http://ih.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://gp.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://jd.521024.cn

C#:   list.Add(4);
来源：http://pf.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://xx.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://xf.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xa.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sq.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://fv.nszjky.cn

Java: list.add(0, 0);
来源：http://as.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ak.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ek.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://di.shxzukj.cn

[D04] 删除元素
来源：http://sk.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://my.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vs.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sc.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://gb.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ne.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mo.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://em.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fd.shtwfgs.cn

[D05] 访问与修改元素
来源：http://kb.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lh.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ja.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vn.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://yw.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://pa.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://tp.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qv.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vn.haigaiapp.cn

[D06] 数组长度
来源：http://jv.bookmarksfly.cn

Py:   len(arr)
来源：http://ng.hnjuh.cn

PHP:  count($arr);
来源：http://js.chemitech.net.cn

JS:   arr.length
来源：http://wd.muxihuayi.cn

TS:   arr.length
来源：http://pb.yuntaijiaju.cn

Java: list.size();
来源：http://kb.nicolike.cn

Go:   len(arr)
来源：http://lu.szsharing.cn

Ruby: arr.length; arr.size
来源：http://bw.chemitech.net.cn

C#:   list.Count;
来源：http://ca.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://ke.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://up.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ld.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://pc.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://ky.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://pg.szsharing.cn

Go:   arr[1:4]
来源：http://oj.gzmigu.cn

Ruby: arr[1, 3]
来源：http://bl.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://wr.asd995.cn

[D08] 合并两个数组
来源：http://ay.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://gb.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://lg.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://up.muxihuayi.cn

TS:   [...a, ...b];
来源：http://tm.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://um.haigaiapp.cn

Go:   append(a, b...)
来源：http://mn.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://by.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://ep.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://rg.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://cj.yuexingan06.cn

PHP:  sort($arr);
来源：http://wo.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ep.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oc.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sb.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ka.huixiangedu.cn

Ruby: arr.sort
来源：http://yn.szsharing.cn

C#:   list.Sort();
来源：http://fa.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ae.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hj.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xc.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rt.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rf.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vo.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gj.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ke.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://je.nicolike.cn

[D11] 反转数组
来源：http://xe.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ne.521024.cn

PHP:  array_reverse($arr);
来源：http://cn.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uk.gzmigu.cn

TS:   [...arr].reverse();
来源：http://qu.hnjuh.cn

Java: Collections.reverse(list);
来源：http://qx.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://lh.newstarts.cn

Ruby: arr.reverse
来源：http://dv.haigaiapp.cn

C#:   list.Reverse();
来源：http://du.hnjuh.cn

[D12] 查找元素下标
来源：http://sa.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://dh.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wg.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ye.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nk.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oo.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://at.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://er.nszjky.cn

C#:   list.IndexOf(x);
来源：http://eu.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://hs.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xk.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fg.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://el.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://fe.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tn.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xh.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xd.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xw.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://tq.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yo.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oy.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://om.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://ds.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tu.hahajie.cn

Go:   // 手写循环
来源：http://vf.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nt.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sz.yuexingan06.cn

[D15] 去重
来源：http://ry.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fc.lnxyls.cn

PHP:  array_unique($arr);
来源：http://pp.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://br.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://zp.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://db.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sf.nszjky.cn

Ruby: arr.uniq
来源：http://mw.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://yr.nszjky.cn

[D16] 求和与平均值
来源：http://en.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pe.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rt.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vc.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yi.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rw.muxihuayi.cn

Go:   // 手写循环累加
来源：http://vb.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ay.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://au.hahajie.cn

[D17] 最大值与最小值
来源：http://on.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://to.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://ui.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cy.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://re.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kt.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uh.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://rf.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://ig.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://yh.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ku.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://ay.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://al.bookmarksfly.cn

TS:   nested.flat();
来源：http://zb.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sf.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://pf.9csxet.cn

Ruby: nested.flatten
来源：http://ra.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rj.9csxet.cn

[D19] 按字段分组
来源：http://mm.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rx.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pn.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wg.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hd.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ew.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://wr.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pp.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bk.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://fh.newstarts.cn

Py:   Counter(arr)
来源：http://ra.hahajie.cn

PHP:  array_count_values($arr);
来源：http://kd.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mv.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://be.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://ln.huixinmuqiang.cn

Ruby: arr.tally
来源：http://yz.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nn.hahajie.cn

[D21] 判断是否包含某元素
来源：http://eo.shxzukj.cn

Py:   x in arr
来源：http://pg.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://rr.nicolike.cn

JS:   arr.includes(x)
来源：http://oa.bjjhwx.cn

TS:   arr.includes(x)
来源：http://ke.chemitech.net.cn

Java: list.contains(x)
来源：http://id.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://fd.nszjky.cn

Ruby: arr.include?(x)
来源：http://rp.wgjwhj.cn

C#:   list.Contains(x)
来源：http://nw.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://ty.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jl.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pf.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ji.wgjwhj.cn

TS:   [...arr];
来源：http://fo.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://og.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ck.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://ih.colortex.cn

C#:   new List<int>(list);
来源：http://ka.521024.cn

[D23] reduce 累积计算
来源：http://rr.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dj.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://io.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fu.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zd.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cv.colortex.cn

Go:   // 手写循环
来源：http://bd.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sb.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gw.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://vu.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fs.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tl.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cg.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dx.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lz.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vw.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kn.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qd.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://zu.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://or.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eo.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://al.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jp.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vh.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ot.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sw.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pv.hahajie.cn

[D26] 数组转字符串
来源：http://dj.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://hu.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://sy.huanxung.cn

JS:   arr.join(", ")
来源：http://dc.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://uy.newstarts.cn

Java: String.join(", ", list)
来源：http://wa.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://xt.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://rw.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://dw.huixiangedu.cn

================================================================================
来源：http://nf.huixiangedu.cn

E. 字符串处理
来源：http://yh.bookmarksfly.cn

================================================================================
来源：http://zt.shxzukj.cn

[E01] 拼接字符串
来源：http://jj.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dp.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fl.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wr.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ek.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yg.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xy.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pp.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vv.gzmigu.cn

[E02] 重复字符串
来源：http://qb.shtwfgs.cn

Py:   "ab" * 3
来源：http://er.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://cm.huanxung.cn

JS:   "ab".repeat(3)
来源：http://kx.hahajie.cn

TS:   "ab".repeat(3)
来源：http://pj.szxytkj.cn

Java: "ab".repeat(3)
来源：http://ya.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://hu.shxzskj.cn

Ruby: "ab" * 3
来源：http://pp.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ik.nszjky.cn

[E03] 截取子串
来源：http://kg.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ex.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dl.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sn.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://sc.shxzukj.cn

Java: s.substring(1, 4)
来源：http://bx.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://np.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xg.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://cn.521024.cn

[E04] 查找子串位置
来源：http://tu.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://by.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://ap.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xi.panjiajie.cn

TS:   s.indexOf("x")
来源：http://zg.colortex.cn

Java: s.indexOf("x")
来源：http://wr.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://kl.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://eh.asd995.cn

C#:   s.IndexOf("x")
来源：http://te.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ls.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rp.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pp.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wu.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ee.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://li.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vh.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sr.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jc.asd995.cn

[E06] 替换子串
来源：http://hg.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zi.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://ac.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wd.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://ar.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qw.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ts.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://by.shtwfgs.cn


<!-- 参考信息 -->