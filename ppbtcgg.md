代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xn.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nf.yuntaijiaju.cn

Java: // 无解构
来源：http://sz.panjiajie.cn

Go:   // 无解构
来源：http://tp.521024.cn

Ruby: a, b = pair
来源：http://rk.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://wb.nicolike.cn

[C16] 函数 / 方法重载
来源：http://mz.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cs.bjjhwx.cn

PHP:  // 无重载
来源：http://ff.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://aj.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://tw.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bs.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://ha.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://tb.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ao.szxytkj.cn

================================================================================
来源：http://vx.521024.cn

D. 数组 / 列表 / 集合
来源：http://jl.szxytkj.cn

================================================================================
来源：http://hq.nszjky.cn

[D01] 创建数组 / 列表
来源：http://pr.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://up.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rr.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yg.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ss.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ps.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://kt.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://fa.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cw.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://rp.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hj.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kb.asd995.cn

JS:   arr.push(4);
来源：http://jd.hahajie.cn

TS:   arr.push(4);
来源：http://kx.nicolike.cn

Java: list.add(4);
来源：http://gm.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://kn.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://qd.hahajie.cn

C#:   list.Add(4);
来源：http://sc.chemitech.net.cn

[D03] 在指定位置插入元素
来源：http://lj.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://rb.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zh.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mf.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://cu.colortex.cn

Java: list.add(0, 0);
来源：http://fy.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ij.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fb.521024.cn

C#:   list.Insert(0, 0);
来源：http://pj.szxytkj.cn

[D04] 删除元素
来源：http://zn.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mo.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://md.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ir.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://fe.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ub.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lo.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ey.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rf.muxihuayi.cn

[D05] 访问与修改元素
来源：http://yi.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://th.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xb.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ld.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://hv.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://pb.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://os.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oi.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ro.colortex.cn

[D06] 数组长度
来源：http://ar.nszjky.cn

Py:   len(arr)
来源：http://az.haigaiapp.cn

PHP:  count($arr);
来源：http://dx.jctech888.com.cn

JS:   arr.length
来源：http://ls.huanxung.cn

TS:   arr.length
来源：http://ht.szxytkj.cn

Java: list.size();
来源：http://sf.huixinmuqiang.cn

Go:   len(arr)
来源：http://nb.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://my.huixiangedu.cn

C#:   list.Count;
来源：http://tr.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://kx.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cy.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dj.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://wy.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://br.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://zr.shxzukj.cn

Go:   arr[1:4]
来源：http://jw.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://dy.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://gw.jctech888.com.cn

[D08] 合并两个数组
来源：http://fh.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://qy.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://lw.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aw.bjjhwx.cn

TS:   [...a, ...b];
来源：http://zq.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wx.bookmarksfly.cn

Go:   append(a, b...)
来源：http://on.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://sv.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://fj.shtwfgs.cn

[D09] 排序（升序）
来源：http://ws.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ku.szxytkj.cn

PHP:  sort($arr);
来源：http://fm.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xr.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wl.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tg.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uz.jianghongdianzi.cn

Ruby: arr.sort
来源：http://sf.bjjhwx.cn

C#:   list.Sort();
来源：http://ks.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gn.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xp.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://de.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nn.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ec.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vp.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bw.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wg.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kg.nszjky.cn

[D11] 反转数组
来源：http://yj.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bf.521024.cn

PHP:  array_reverse($arr);
来源：http://wl.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lp.asd995.cn

TS:   [...arr].reverse();
来源：http://ws.colortex.cn

Java: Collections.reverse(list);
来源：http://ac.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://oj.gzmigu.cn

Ruby: arr.reverse
来源：http://xg.huanxung.cn

C#:   list.Reverse();
来源：http://fq.nicolike.cn

[D12] 查找元素下标
来源：http://zv.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://fc.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zv.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://og.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fo.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jn.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://tz.chemitech.net.cn

Ruby: arr.index(x)
来源：http://rm.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://su.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://wa.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ui.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wa.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://wl.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://fe.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fo.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ex.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uc.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ka.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://va.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://md.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://td.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://da.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://fx.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fx.yuntaijiaju.cn

Go:   // 手写循环
来源：http://yu.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ww.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mh.nszjky.cn

[D15] 去重
来源：http://vm.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gn.shxzukj.cn

PHP:  array_unique($arr);
来源：http://rt.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://uh.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://ce.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ux.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qz.shtwfgs.cn

Ruby: arr.uniq
来源：http://nk.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://ie.shxzukj.cn

[D16] 求和与平均值
来源：http://ko.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gz.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fs.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kl.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ay.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pe.asd995.cn

Go:   // 手写循环累加
来源：http://sf.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fg.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://om.panjiajie.cn

[D17] 最大值与最小值
来源：http://tq.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://mp.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://ae.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wx.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://rl.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xu.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pv.asd995.cn

Ruby: arr.max;  arr.min
来源：http://dk.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://se.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://ei.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lg.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://ev.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://az.muxihuayi.cn

TS:   nested.flat();
来源：http://lk.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://we.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://yf.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://ml.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yf.gzmigu.cn

[D19] 按字段分组
来源：http://kd.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cy.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ny.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rj.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://id.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pu.521024.cn

Go:   // 手写 map[string][]T
来源：http://aq.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wz.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dq.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://na.huanxung.cn

Py:   Counter(arr)
来源：http://ed.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://cu.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lj.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ct.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rf.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://ca.huixiangedu.cn

Ruby: arr.tally
来源：http://ga.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://km.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://md.shxzskj.cn

Py:   x in arr
来源：http://vy.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://rm.bjjhwx.cn

JS:   arr.includes(x)
来源：http://yz.gzmigu.cn

TS:   arr.includes(x)
来源：http://tb.gzmigu.cn

Java: list.contains(x)
来源：http://hx.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://qc.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://yx.9csxet.cn

C#:   list.Contains(x)
来源：http://ss.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://ug.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xw.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sq.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fx.lnxyls.cn

TS:   [...arr];
来源：http://hv.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://ex.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sk.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://oy.bjjhwx.cn

C#:   new List<int>(list);
来源：http://kz.jctech888.com.cn

[D23] reduce 累积计算
来源：http://dx.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://us.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://li.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jq.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dj.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xq.colortex.cn

Go:   // 手写循环
来源：http://ar.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yp.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://od.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://is.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vc.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://in.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ux.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nn.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uj.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mx.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wf.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nz.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://bg.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fb.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lf.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ct.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mk.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ke.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ey.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://im.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mo.wgjwhj.cn

[D26] 数组转字符串
来源：http://ed.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://uf.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://fc.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://me.jctech888.com.cn

TS:   arr.join(", ")
来源：http://to.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://lu.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://id.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://fj.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://gt.nicolike.cn

================================================================================
来源：http://nz.muxihuayi.cn

E. 字符串处理
来源：http://ne.haigaiapp.cn

================================================================================
来源：http://tg.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://ak.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rz.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tc.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qx.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ce.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xv.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://br.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lu.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vu.lnxyls.cn

[E02] 重复字符串
来源：http://wh.szxytkj.cn

Py:   "ab" * 3
来源：http://qe.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://yf.newstarts.cn

JS:   "ab".repeat(3)
来源：http://ns.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://ts.colortex.cn

Java: "ab".repeat(3)
来源：http://rn.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://jt.wgjwhj.cn

Ruby: "ab" * 3
来源：http://jm.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eq.szxytkj.cn

[E03] 截取子串
来源：http://mu.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jb.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xu.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sm.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://kd.9csxet.cn

Java: s.substring(1, 4)
来源：http://jb.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qn.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pc.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://gf.bjjhwx.cn

[E04] 查找子串位置
来源：http://ep.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://st.huanxung.cn

PHP:  strpos($s, "x");
来源：http://og.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://li.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://qd.szsharing.cn

Java: s.indexOf("x")
来源：http://cg.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://ef.chemitech.net.cn

Ruby: s.index("x")
来源：http://zm.521024.cn

C#:   s.IndexOf("x")
来源：http://en.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oq.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ls.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yu.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vm.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hl.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pe.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cp.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tp.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ve.chemitech.net.cn


<!-- 参考信息 -->