代发 wailian999

Ruby: a, b = pair
来源：http://uw.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://ct.521024.cn

[C16] 函数 / 方法重载
来源：http://tl.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dm.nicolike.cn

PHP:  // 无重载
来源：http://sv.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://my.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://wh.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kh.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://ee.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://zc.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rc.muxihuayi.cn

================================================================================
来源：http://si.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://bd.newstarts.cn

================================================================================
来源：http://um.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://dw.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fa.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ut.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jx.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cb.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pr.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://yb.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://qn.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xl.newstarts.cn

[D02] 追加元素到末尾
来源：http://uo.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ja.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qn.huanxung.cn

JS:   arr.push(4);
来源：http://yr.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://eh.huixinmuqiang.cn

Java: list.add(4);
来源：http://cw.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://oo.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://ox.gzmigu.cn

C#:   list.Add(4);
来源：http://tl.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://ct.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://ty.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wt.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ty.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://bt.shxzskj.cn

Java: list.add(0, 0);
来源：http://st.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ct.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kd.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://cr.huanxung.cn

[D04] 删除元素
来源：http://iw.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jq.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vd.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rv.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://va.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rx.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://id.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jz.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ru.lnxyls.cn

[D05] 访问与修改元素
来源：http://ry.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://by.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ys.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lt.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://iu.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://zc.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://nv.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eh.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nr.huixinmuqiang.cn

[D06] 数组长度
来源：http://ry.szsharing.cn

Py:   len(arr)
来源：http://pn.szsharing.cn

PHP:  count($arr);
来源：http://tz.muxihuayi.cn

JS:   arr.length
来源：http://tu.chemitech.net.cn

TS:   arr.length
来源：http://qc.jctech888.com.cn

Java: list.size();
来源：http://eh.asd995.cn

Go:   len(arr)
来源：http://le.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://pb.huanxung.cn

C#:   list.Count;
来源：http://nz.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://bf.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ae.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jd.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://uk.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://rf.gzmigu.cn

Java: list.subList(1, 4);
来源：http://ls.bjjhwx.cn

Go:   arr[1:4]
来源：http://ai.gzmigu.cn

Ruby: arr[1, 3]
来源：http://qv.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://du.shxzukj.cn

[D08] 合并两个数组
来源：http://vo.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://qp.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://sq.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ux.szxytkj.cn

TS:   [...a, ...b];
来源：http://vk.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ie.huixiangedu.cn

Go:   append(a, b...)
来源：http://mh.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://gj.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://kd.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://vn.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://un.chemitech.net.cn

PHP:  sort($arr);
来源：http://xc.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cz.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://go.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gh.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nt.jianghongdianzi.cn

Ruby: arr.sort
来源：http://jd.colortex.cn

C#:   list.Sort();
来源：http://mk.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://il.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ki.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://em.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hw.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sp.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ac.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tr.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pv.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ba.huanxung.cn

[D11] 反转数组
来源：http://iu.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mc.nicolike.cn

PHP:  array_reverse($arr);
来源：http://iw.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oq.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://fn.asd995.cn

Java: Collections.reverse(list);
来源：http://gg.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://yb.haigaiapp.cn

Ruby: arr.reverse
来源：http://xb.9csxet.cn

C#:   list.Reverse();
来源：http://ug.yuexingan06.cn

[D12] 查找元素下标
来源：http://ve.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://ml.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dp.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://no.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fj.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uz.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://gv.colortex.cn

Ruby: arr.index(x)
来源：http://sm.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://mi.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://nj.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hr.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hs.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://xe.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://am.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eo.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zf.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nt.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ew.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://xp.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rz.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zv.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://pc.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://fi.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rf.9csxet.cn

Go:   // 手写循环
来源：http://tw.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://me.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hw.shxzukj.cn

[D15] 去重
来源：http://kj.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jf.panjiajie.cn

PHP:  array_unique($arr);
来源：http://ok.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://qo.colortex.cn

TS:   [...new Set(arr)]
来源：http://xa.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dm.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uc.panjiajie.cn

Ruby: arr.uniq
来源：http://gw.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://cg.nicolike.cn

[D16] 求和与平均值
来源：http://vx.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gg.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uh.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ov.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kc.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vq.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://ar.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cy.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://gf.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://xg.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://th.521024.cn

PHP:  max($arr);  min($arr);
来源：http://ss.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ap.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://qy.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kq.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qk.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://wr.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://et.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://ku.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zs.521024.cn

PHP:  array_merge(...$nested);
来源：http://ya.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jy.wgjwhj.cn

TS:   nested.flat();
来源：http://ij.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tu.chemitech.net.cn

Go:   // 手写双层循环
来源：http://ec.huanxung.cn

Ruby: nested.flatten
来源：http://jg.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bl.nszjky.cn

[D19] 按字段分组
来源：http://aw.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ki.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nh.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xc.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ef.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xt.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://cm.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ur.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dz.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://sn.asd995.cn

Py:   Counter(arr)
来源：http://mz.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://ti.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wh.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ci.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rv.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://bp.muxihuayi.cn

Ruby: arr.tally
来源：http://tw.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gv.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://nc.gzmigu.cn

Py:   x in arr
来源：http://nv.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://xm.shtwfgs.cn

JS:   arr.includes(x)
来源：http://nf.9csxet.cn

TS:   arr.includes(x)
来源：http://dc.521024.cn

Java: list.contains(x)
来源：http://gi.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://do.newstarts.cn

Ruby: arr.include?(x)
来源：http://ki.asd995.cn

C#:   list.Contains(x)
来源：http://ps.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://nb.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ig.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bj.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dh.lnxyls.cn

TS:   [...arr];
来源：http://ir.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://pq.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bh.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://wf.huixiangedu.cn

C#:   new List<int>(list);
来源：http://ag.hnjuh.cn

[D23] reduce 累积计算
来源：http://mo.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gf.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://um.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ab.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bv.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fj.huanxung.cn

Go:   // 手写循环
来源：http://fo.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nn.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qc.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://ix.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ey.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hl.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sc.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oz.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tj.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pi.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vm.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fr.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://ky.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://we.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xo.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hw.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tz.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xp.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eg.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bn.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qw.bjjhwx.cn

[D26] 数组转字符串
来源：http://wk.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://mc.asd995.cn

PHP:  implode(", ", $arr);
来源：http://bf.szxytkj.cn

JS:   arr.join(", ")
来源：http://ii.bjjhwx.cn

TS:   arr.join(", ")
来源：http://ot.jctech888.com.cn

Java: String.join(", ", list)
来源：http://vn.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://ff.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://tj.521024.cn

C#:   string.Join(", ", list)
来源：http://zn.shtwfgs.cn

================================================================================
来源：http://rn.bjjhwx.cn

E. 字符串处理
来源：http://jp.asd995.cn

================================================================================
来源：http://ry.shxzukj.cn

[E01] 拼接字符串
来源：http://qu.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ac.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nq.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bh.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ki.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ig.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jx.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zz.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bq.yuexingan06.cn

[E02] 重复字符串
来源：http://eq.521024.cn

Py:   "ab" * 3
来源：http://nf.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://im.asd995.cn

JS:   "ab".repeat(3)
来源：http://up.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://xz.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://qp.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://ru.nicolike.cn

Ruby: "ab" * 3
来源：http://qg.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fp.nszjky.cn

[E03] 截取子串
来源：http://vv.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zn.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ir.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://py.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://zr.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://qx.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://va.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fx.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://zi.nszjky.cn

[E04] 查找子串位置
来源：http://zt.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://uc.colortex.cn

PHP:  strpos($s, "x");
来源：http://ws.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fa.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://qk.hnjuh.cn

Java: s.indexOf("x")
来源：http://yv.colortex.cn

Go:   strings.Index(s, "x")
来源：http://bw.hnjuh.cn

Ruby: s.index("x")
来源：http://ng.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://uo.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://es.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ev.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ou.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cm.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pu.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bm.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vp.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vc.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uh.hahajie.cn

[E06] 替换子串
来源：http://ai.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ub.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://qi.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tf.nszjky.cn


<!-- 参考信息 -->