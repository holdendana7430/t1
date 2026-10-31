代发 wailian999

PHP:  // 无重载
来源：http://am.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gw.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://bj.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://az.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ux.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://rd.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zh.gzmigu.cn

================================================================================
来源：http://ol.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://eu.9csxet.cn

================================================================================
来源：http://yg.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://ll.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mo.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xr.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ut.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nx.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cg.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://wn.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ma.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wh.colortex.cn

[D02] 追加元素到末尾
来源：http://nu.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qd.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bm.panjiajie.cn

JS:   arr.push(4);
来源：http://rs.chemitech.net.cn

TS:   arr.push(4);
来源：http://jw.gzmigu.cn

Java: list.add(4);
来源：http://bt.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://yt.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://il.jctech888.com.cn

C#:   list.Add(4);
来源：http://xo.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://cb.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://of.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://at.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kr.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://vq.huixiangedu.cn

Java: list.add(0, 0);
来源：http://pt.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://su.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kq.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://cx.shxzukj.cn

[D04] 删除元素
来源：http://ei.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ih.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gz.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://db.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://ic.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ea.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ap.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vh.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xn.newstarts.cn

[D05] 访问与修改元素
来源：http://zs.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kw.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zd.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kp.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://mz.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://rp.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://aa.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wr.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vf.521024.cn

[D06] 数组长度
来源：http://nu.szsharing.cn

Py:   len(arr)
来源：http://tw.bookmarksfly.cn

PHP:  count($arr);
来源：http://qj.huixinmuqiang.cn

JS:   arr.length
来源：http://xw.yuntaijiaju.cn

TS:   arr.length
来源：http://ja.jianghongdianzi.cn

Java: list.size();
来源：http://xo.yuntaijiaju.cn

Go:   len(arr)
来源：http://zm.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://cy.shxzukj.cn

C#:   list.Count;
来源：http://nu.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://hp.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ka.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mj.colortex.cn

JS:   arr.slice(1, 4);
来源：http://ne.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://rk.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://bv.yuexingan06.cn

Go:   arr[1:4]
来源：http://da.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://pk.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://hs.huixiangedu.cn

[D08] 合并两个数组
来源：http://ui.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://tm.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://xu.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pp.jctech888.com.cn

TS:   [...a, ...b];
来源：http://ng.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hh.nszjky.cn

Go:   append(a, b...)
来源：http://tt.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://br.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://cv.yuexingan06.cn

[D09] 排序（升序）
来源：http://ic.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://rf.huanxung.cn

PHP:  sort($arr);
来源：http://oa.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oy.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ur.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rn.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uz.yuntaijiaju.cn

Ruby: arr.sort
来源：http://im.shxzukj.cn

C#:   list.Sort();
来源：http://rp.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://to.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wp.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hw.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sh.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vf.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rl.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dm.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hp.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vs.521024.cn

[D11] 反转数组
来源：http://uu.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dc.szsharing.cn

PHP:  array_reverse($arr);
来源：http://nu.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wu.nicolike.cn

TS:   [...arr].reverse();
来源：http://qu.szxytkj.cn

Java: Collections.reverse(list);
来源：http://zf.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://sp.shxzskj.cn

Ruby: arr.reverse
来源：http://vp.gzmigu.cn

C#:   list.Reverse();
来源：http://bd.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://ar.521024.cn

Py:   arr.index(x);  x in arr
来源：http://zo.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xa.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hn.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fp.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fm.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://wt.panjiajie.cn

Ruby: arr.index(x)
来源：http://ot.asd995.cn

C#:   list.IndexOf(x);
来源：http://ld.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://dh.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wf.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qs.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://oa.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://pt.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fi.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qc.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ob.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dn.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://dq.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xx.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pl.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://en.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://om.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sa.gzmigu.cn

Go:   // 手写循环
来源：http://xu.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wp.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iq.nszjky.cn

[D15] 去重
来源：http://uz.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ro.nszjky.cn

PHP:  array_unique($arr);
来源：http://po.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://px.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://vz.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lc.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lt.bjjhwx.cn

Ruby: arr.uniq
来源：http://sz.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://nd.hahajie.cn

[D16] 求和与平均值
来源：http://uw.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eb.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ty.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qr.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://di.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vn.newstarts.cn

Go:   // 手写循环累加
来源：http://il.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ca.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://on.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://st.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://nt.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://ac.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xi.newstarts.cn

TS:   Math.max(...arr);
来源：http://hz.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vu.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tq.asd995.cn

Ruby: arr.max;  arr.min
来源：http://kg.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://uv.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://fd.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yu.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://hz.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gv.colortex.cn

TS:   nested.flat();
来源：http://vq.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nl.haigaiapp.cn

Go:   // 手写双层循环
来源：http://rk.yuexingan06.cn

Ruby: nested.flatten
来源：http://jt.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cr.huixiangedu.cn

[D19] 按字段分组
来源：http://qm.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://if.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wm.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://il.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gi.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ld.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://ao.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gl.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://go.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://hn.gzmigu.cn

Py:   Counter(arr)
来源：http://cp.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://tg.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://da.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mv.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://di.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://nn.gzmigu.cn

Ruby: arr.tally
来源：http://om.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ll.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://kt.huanxung.cn

Py:   x in arr
来源：http://zo.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://us.bjjhwx.cn

JS:   arr.includes(x)
来源：http://ik.lnxyls.cn

TS:   arr.includes(x)
来源：http://oa.shxzskj.cn

Java: list.contains(x)
来源：http://rl.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://eh.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://ow.newstarts.cn

C#:   list.Contains(x)
来源：http://xu.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://wd.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://so.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qx.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ej.huixiangedu.cn

TS:   [...arr];
来源：http://zm.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://nm.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zq.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://kt.asd995.cn

C#:   new List<int>(list);
来源：http://jw.shxzskj.cn

[D23] reduce 累积计算
来源：http://az.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hv.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bh.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zj.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://my.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sx.asd995.cn

Go:   // 手写循环
来源：http://aj.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cx.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qf.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://bp.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gi.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ce.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iz.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vg.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bq.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hs.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hy.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ef.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://um.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://id.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ax.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tr.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fk.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://if.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mj.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pb.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dl.newstarts.cn

[D26] 数组转字符串
来源：http://gu.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://nx.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://um.hahajie.cn

JS:   arr.join(", ")
来源：http://ii.wgjwhj.cn

TS:   arr.join(", ")
来源：http://ed.muxihuayi.cn

Java: String.join(", ", list)
来源：http://qu.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://bp.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://lu.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://eb.yuntaijiaju.cn

================================================================================
来源：http://tm.huixinmuqiang.cn

E. 字符串处理
来源：http://fb.muxihuayi.cn

================================================================================
来源：http://ac.chemitech.net.cn

[E01] 拼接字符串
来源：http://qo.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iy.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sw.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wp.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://va.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hf.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cq.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nd.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://la.jianghongdianzi.cn

[E02] 重复字符串
来源：http://em.nicolike.cn

Py:   "ab" * 3
来源：http://wu.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://it.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://lc.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://ip.nicolike.cn

Java: "ab".repeat(3)
来源：http://aj.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://kx.gzmigu.cn

Ruby: "ab" * 3
来源：http://aa.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uy.yuntaijiaju.cn

[E03] 截取子串
来源：http://no.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jq.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tx.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cl.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://sm.newstarts.cn

Java: s.substring(1, 4)
来源：http://bw.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jw.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jw.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://zz.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://nr.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://vg.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://zr.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qc.gzmigu.cn

TS:   s.indexOf("x")
来源：http://sz.shxzskj.cn

Java: s.indexOf("x")
来源：http://pg.521024.cn

Go:   strings.Index(s, "x")
来源：http://oj.9csxet.cn

Ruby: s.index("x")
来源：http://yf.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://gs.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dz.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uf.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kf.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bw.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gh.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://np.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qd.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sx.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ic.asd995.cn

[E06] 替换子串
来源：http://zp.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nd.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://hk.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ax.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://cg.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://su.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sj.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yi.nicolike.cn


<!-- 参考信息 -->