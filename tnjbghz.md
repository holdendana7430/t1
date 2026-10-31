代发 wailian999

PHP:  // 无重载
来源：http://bd.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yx.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://ca.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://im.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://dq.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://fz.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sw.shxzukj.cn

================================================================================
来源：http://pu.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://jw.huixiangedu.cn

================================================================================
来源：http://fb.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://lf.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hg.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://td.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cc.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mz.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tw.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://pb.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://bk.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vs.nicolike.cn

[D02] 追加元素到末尾
来源：http://gv.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qt.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oj.muxihuayi.cn

JS:   arr.push(4);
来源：http://ow.hnjuh.cn

TS:   arr.push(4);
来源：http://jb.panjiajie.cn

Java: list.add(4);
来源：http://uh.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://hq.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://mt.bookmarksfly.cn

C#:   list.Add(4);
来源：http://ab.nicolike.cn

[D03] 在指定位置插入元素
来源：http://uv.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://fe.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xh.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dv.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://lk.bjjhwx.cn

Java: list.add(0, 0);
来源：http://vl.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nx.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://in.asd995.cn

C#:   list.Insert(0, 0);
来源：http://wm.jianghongdianzi.cn

[D04] 删除元素
来源：http://rq.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tv.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dt.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ja.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://je.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qp.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cy.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rg.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://na.shtwfgs.cn

[D05] 访问与修改元素
来源：http://yj.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tb.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hk.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vi.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ba.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://fz.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://dh.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eg.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ae.shtwfgs.cn

[D06] 数组长度
来源：http://gu.hnjuh.cn

Py:   len(arr)
来源：http://wk.jianghongdianzi.cn

PHP:  count($arr);
来源：http://vf.gzmigu.cn

JS:   arr.length
来源：http://tl.nicolike.cn

TS:   arr.length
来源：http://zj.lnxyls.cn

Java: list.size();
来源：http://ei.shxzskj.cn

Go:   len(arr)
来源：http://zq.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://vv.nszjky.cn

C#:   list.Count;
来源：http://nt.9csxet.cn

[D07] 切片 / 取子数组
来源：http://ue.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ns.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qm.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://ah.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://jm.521024.cn

Java: list.subList(1, 4);
来源：http://cu.yuexingan06.cn

Go:   arr[1:4]
来源：http://dt.huanxung.cn

Ruby: arr[1, 3]
来源：http://cl.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://zu.nicolike.cn

[D08] 合并两个数组
来源：http://mw.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://xj.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://qx.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wn.haigaiapp.cn

TS:   [...a, ...b];
来源：http://yo.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ki.gzmigu.cn

Go:   append(a, b...)
来源：http://gp.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://ie.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://sn.bookmarksfly.cn

[D09] 排序（升序）
来源：http://kc.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://rl.nszjky.cn

PHP:  sort($arr);
来源：http://zx.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ut.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fq.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pe.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cr.muxihuayi.cn

Ruby: arr.sort
来源：http://va.hnjuh.cn

C#:   list.Sort();
来源：http://gy.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://we.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zn.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zr.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eg.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nz.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pe.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ar.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zr.521024.cn

[D11] 反转数组
来源：http://yo.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xl.colortex.cn

PHP:  array_reverse($arr);
来源：http://tw.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://er.shxzskj.cn

TS:   [...arr].reverse();
来源：http://vo.9csxet.cn

Java: Collections.reverse(list);
来源：http://fc.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://um.wgjwhj.cn

Ruby: arr.reverse
来源：http://xp.shtwfgs.cn

C#:   list.Reverse();
来源：http://ky.hahajie.cn

[D12] 查找元素下标
来源：http://hj.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://sg.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bm.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dk.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dc.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ke.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://yj.nicolike.cn

Ruby: arr.index(x)
来源：http://dl.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://yc.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://cm.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hu.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lc.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://hm.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://gd.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vq.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wt.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://if.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pd.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://nz.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ax.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bk.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://qz.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://nl.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ld.yuexingan06.cn

Go:   // 手写循环
来源：http://sw.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ui.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uq.nszjky.cn

[D15] 去重
来源：http://pq.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hd.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://tr.asd995.cn

JS:   [...new Set(arr)]
来源：http://xs.9csxet.cn

TS:   [...new Set(arr)]
来源：http://ie.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mp.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://px.haigaiapp.cn

Ruby: arr.uniq
来源：http://fv.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://ul.9csxet.cn

[D16] 求和与平均值
来源：http://ty.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fs.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vz.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aw.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ow.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cl.szxytkj.cn

Go:   // 手写循环累加
来源：http://sq.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gr.521024.cn

C#:   list.Sum();  list.Average()
来源：http://sj.newstarts.cn

[D17] 最大值与最小值
来源：http://vi.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://qc.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://mg.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vn.nicolike.cn

TS:   Math.max(...arr);
来源：http://uc.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ho.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dr.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://ky.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://bt.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://lh.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ii.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://pz.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lw.jianghongdianzi.cn

TS:   nested.flat();
来源：http://bp.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hu.szsharing.cn

Go:   // 手写双层循环
来源：http://su.muxihuayi.cn

Ruby: nested.flatten
来源：http://ev.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cp.9csxet.cn

[D19] 按字段分组
来源：http://jw.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ui.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://md.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gs.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ae.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ex.colortex.cn

Go:   // 手写 map[string][]T
来源：http://uv.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wy.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sr.colortex.cn

[D20] 统计每个元素出现次数
来源：http://ku.9csxet.cn

Py:   Counter(arr)
来源：http://kk.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://vh.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ai.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://up.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://di.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://zk.521024.cn

Ruby: arr.tally
来源：http://ho.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://js.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://sq.colortex.cn

Py:   x in arr
来源：http://om.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://iz.nicolike.cn

JS:   arr.includes(x)
来源：http://ep.nszjky.cn

TS:   arr.includes(x)
来源：http://yu.newstarts.cn

Java: list.contains(x)
来源：http://nc.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://es.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://qf.hahajie.cn

C#:   list.Contains(x)
来源：http://ed.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://nc.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mu.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ud.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rw.wgjwhj.cn

TS:   [...arr];
来源：http://nu.521024.cn

Java: new ArrayList<>(list);
来源：http://oh.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xd.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://bf.szxytkj.cn

C#:   new List<int>(list);
来源：http://hp.nicolike.cn

[D23] reduce 累积计算
来源：http://ir.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fd.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fs.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ke.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qh.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://al.huanxung.cn

Go:   // 手写循环
来源：http://wq.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nh.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lr.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://xb.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dx.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dr.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wn.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kj.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rh.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ye.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hc.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ig.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://rz.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rp.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rv.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ko.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://et.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nx.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ww.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aj.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cd.newstarts.cn

[D26] 数组转字符串
来源：http://ug.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://ol.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://fd.wgjwhj.cn

JS:   arr.join(", ")
来源：http://zy.jctech888.com.cn

TS:   arr.join(", ")
来源：http://bg.wgjwhj.cn

Java: String.join(", ", list)
来源：http://gf.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ue.colortex.cn

Ruby: arr.join(", ")
来源：http://qb.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://gs.szxytkj.cn

================================================================================
来源：http://cx.huanxung.cn

E. 字符串处理
来源：http://xv.panjiajie.cn

================================================================================
来源：http://pi.shtwfgs.cn

[E01] 拼接字符串
来源：http://uz.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pf.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://le.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://co.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cw.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cl.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yr.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fe.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zd.shxzukj.cn

[E02] 重复字符串
来源：http://ld.huixiangedu.cn

Py:   "ab" * 3
来源：http://mw.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://ee.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://xr.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://ky.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://do.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://vc.newstarts.cn

Ruby: "ab" * 3
来源：http://vg.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://an.lnxyls.cn

[E03] 截取子串
来源：http://gk.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sn.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wd.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://av.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://wo.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://xh.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kq.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://co.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://wj.hnjuh.cn

[E04] 查找子串位置
来源：http://ri.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://xn.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://zr.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ub.nszjky.cn

TS:   s.indexOf("x")
来源：http://dj.szxytkj.cn

Java: s.indexOf("x")
来源：http://ij.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://ai.muxihuayi.cn

Ruby: s.index("x")
来源：http://lf.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://ym.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yt.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ed.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ic.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ln.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://em.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kb.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mf.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xy.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bi.asd995.cn

[E06] 替换子串
来源：http://dr.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xe.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ra.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ds.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://bo.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://us.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fz.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://my.jctech888.com.cn


<!-- 参考信息 -->