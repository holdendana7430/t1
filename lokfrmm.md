代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dw.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uq.panjiajie.cn

Java: // 无解构
来源：http://ru.chemitech.net.cn

Go:   // 无解构
来源：http://pw.bookmarksfly.cn

Ruby: a, b = pair
来源：http://vf.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://jl.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://nt.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://au.shxzukj.cn

PHP:  // 无重载
来源：http://pq.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vp.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://sl.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hk.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://ev.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://uw.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mg.hnjuh.cn

================================================================================
来源：http://pf.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://lz.hahajie.cn

================================================================================
来源：http://my.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://rq.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fy.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fl.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ui.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cn.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ai.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://dg.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://li.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xm.colortex.cn

[D02] 追加元素到末尾
来源：http://tx.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://et.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sw.yuexingan06.cn

JS:   arr.push(4);
来源：http://qt.nszjky.cn

TS:   arr.push(4);
来源：http://la.jianghongdianzi.cn

Java: list.add(4);
来源：http://pm.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://bk.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://vx.newstarts.cn

C#:   list.Add(4);
来源：http://ad.9csxet.cn

[D03] 在指定位置插入元素
来源：http://jz.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://pb.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://td.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sp.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://os.nicolike.cn

Java: list.add(0, 0);
来源：http://fd.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ip.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ma.asd995.cn

C#:   list.Insert(0, 0);
来源：http://bi.szxytkj.cn

[D04] 删除元素
来源：http://zq.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zc.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ra.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mf.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://kz.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xu.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ug.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ec.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yy.shxzukj.cn

[D05] 访问与修改元素
来源：http://ci.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sf.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://on.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ad.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://mp.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://if.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://ba.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uf.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ke.bjjhwx.cn

[D06] 数组长度
来源：http://oh.szxytkj.cn

Py:   len(arr)
来源：http://le.huanxung.cn

PHP:  count($arr);
来源：http://yc.jianghongdianzi.cn

JS:   arr.length
来源：http://hc.huixiangedu.cn

TS:   arr.length
来源：http://pg.lnxyls.cn

Java: list.size();
来源：http://nt.yuexingan06.cn

Go:   len(arr)
来源：http://bq.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://dv.newstarts.cn

C#:   list.Count;
来源：http://sy.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://ez.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hm.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kp.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://hr.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://op.colortex.cn

Java: list.subList(1, 4);
来源：http://uz.chemitech.net.cn

Go:   arr[1:4]
来源：http://ff.521024.cn

Ruby: arr[1, 3]
来源：http://ae.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://vw.nszjky.cn

[D08] 合并两个数组
来源：http://td.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://gq.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://gx.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qz.haigaiapp.cn

TS:   [...a, ...b];
来源：http://fs.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jr.nicolike.cn

Go:   append(a, b...)
来源：http://cf.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://cn.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://we.hnjuh.cn

[D09] 排序（升序）
来源：http://ge.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://jx.hahajie.cn

PHP:  sort($arr);
来源：http://zx.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ja.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xc.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oh.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gl.jctech888.com.cn

Ruby: arr.sort
来源：http://ts.jctech888.com.cn

C#:   list.Sort();
来源：http://et.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fy.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ps.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://np.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jx.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lb.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tt.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pg.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ck.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rc.wgjwhj.cn

[D11] 反转数组
来源：http://aq.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://py.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://hz.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oj.9csxet.cn

TS:   [...arr].reverse();
来源：http://za.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://gl.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://rn.huixiangedu.cn

Ruby: arr.reverse
来源：http://zu.newstarts.cn

C#:   list.Reverse();
来源：http://kx.bookmarksfly.cn

[D12] 查找元素下标
来源：http://bm.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ns.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jl.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bs.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://os.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://at.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://hg.newstarts.cn

Ruby: arr.index(x)
来源：http://yq.nszjky.cn

C#:   list.IndexOf(x);
来源：http://qg.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://md.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tf.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://he.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://kn.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://kx.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lo.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tr.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://er.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mf.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://nh.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://en.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cu.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://wd.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://vx.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lw.szsharing.cn

Go:   // 手写循环
来源：http://js.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ad.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xc.jctech888.com.cn

[D15] 去重
来源：http://ql.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xg.521024.cn

PHP:  array_unique($arr);
来源：http://am.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://fl.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://dq.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nj.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ce.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://rq.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://dr.newstarts.cn

[D16] 求和与平均值
来源：http://xe.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qm.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vj.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lq.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ot.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://io.szxytkj.cn

Go:   // 手写循环累加
来源：http://yj.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xy.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://kj.asd995.cn

[D17] 最大值与最小值
来源：http://bo.colortex.cn

Py:   max(arr);  min(arr)
来源：http://ne.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://os.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qs.shxzukj.cn

TS:   Math.max(...arr);
来源：http://iv.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xb.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wl.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://oy.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://wa.asd995.cn

[D18] 扁平化嵌套数组
来源：http://wo.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://du.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://qm.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qz.hnjuh.cn

TS:   nested.flat();
来源：http://gc.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mj.bjjhwx.cn

Go:   // 手写双层循环
来源：http://gy.chemitech.net.cn

Ruby: nested.flatten
来源：http://wb.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rh.hnjuh.cn

[D19] 按字段分组
来源：http://ww.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yn.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jl.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://at.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hb.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lt.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://ek.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bf.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ml.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://aw.huixiangedu.cn

Py:   Counter(arr)
来源：http://wn.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://fr.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ft.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oz.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zh.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://be.muxihuayi.cn

Ruby: arr.tally
来源：http://lg.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lo.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://om.colortex.cn

Py:   x in arr
来源：http://jb.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://xg.jctech888.com.cn

JS:   arr.includes(x)
来源：http://zi.hahajie.cn

TS:   arr.includes(x)
来源：http://ia.muxihuayi.cn

Java: list.contains(x)
来源：http://tx.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://ob.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://ov.panjiajie.cn

C#:   list.Contains(x)
来源：http://dm.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://xd.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://an.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lc.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://na.bjjhwx.cn

TS:   [...arr];
来源：http://mc.nicolike.cn

Java: new ArrayList<>(list);
来源：http://at.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cx.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://yn.gzmigu.cn

C#:   new List<int>(list);
来源：http://sx.szxytkj.cn

[D23] reduce 累积计算
来源：http://ef.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://si.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ph.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ry.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ru.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dk.szsharing.cn

Go:   // 手写循环
来源：http://um.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sq.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://of.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://hz.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://te.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ks.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zn.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dm.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jm.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kc.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nr.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gk.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://mh.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tu.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ox.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rn.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cv.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yi.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tz.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mk.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://az.nicolike.cn

[D26] 数组转字符串
来源：http://um.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://jg.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://un.chemitech.net.cn

JS:   arr.join(", ")
来源：http://wl.bjjhwx.cn

TS:   arr.join(", ")
来源：http://zt.shxzskj.cn

Java: String.join(", ", list)
来源：http://nz.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://so.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://gm.9csxet.cn

C#:   string.Join(", ", list)
来源：http://tl.jianghongdianzi.cn

================================================================================
来源：http://jl.gzmigu.cn

E. 字符串处理
来源：http://cd.szxytkj.cn

================================================================================
来源：http://od.521024.cn

[E01] 拼接字符串
来源：http://sm.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yj.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ks.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nd.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ye.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://di.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ok.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yc.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rr.shxzskj.cn

[E02] 重复字符串
来源：http://ft.hahajie.cn

Py:   "ab" * 3
来源：http://wh.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://ib.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://pd.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://wt.9csxet.cn

Java: "ab".repeat(3)
来源：http://dg.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://xg.colortex.cn

Ruby: "ab" * 3
来源：http://dm.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ci.szsharing.cn

[E03] 截取子串
来源：http://el.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fw.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qz.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kz.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://or.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://ge.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ud.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yd.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://mb.bookmarksfly.cn

[E04] 查找子串位置
来源：http://cv.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://ms.521024.cn

PHP:  strpos($s, "x");
来源：http://ly.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vp.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://rn.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://qt.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://oo.haigaiapp.cn

Ruby: s.index("x")
来源：http://pj.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://fx.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zq.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hb.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ju.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lr.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ty.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mw.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vh.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rb.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vr.hahajie.cn


<!-- 参考信息 -->