代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bd.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pj.szxytkj.cn

Java: // 无解构
来源：http://ds.wgjwhj.cn

Go:   // 无解构
来源：http://jn.hnjuh.cn

Ruby: a, b = pair
来源：http://eo.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://at.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://qw.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xi.wgjwhj.cn

PHP:  // 无重载
来源：http://ng.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mu.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://wk.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dh.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://gt.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://xm.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qk.shtwfgs.cn

================================================================================
来源：http://uq.521024.cn

D. 数组 / 列表 / 集合
来源：http://bg.bjjhwx.cn

================================================================================
来源：http://lk.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://ik.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wp.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ei.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hv.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vh.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://db.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://cw.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://xp.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jj.lnxyls.cn

[D02] 追加元素到末尾
来源：http://qy.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://us.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zn.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://uo.asd995.cn

TS:   arr.push(4);
来源：http://es.hahajie.cn

Java: list.add(4);
来源：http://gf.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://mn.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://nl.jctech888.com.cn

C#:   list.Add(4);
来源：http://nk.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://gt.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://wh.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tx.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yv.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://hb.521024.cn

Java: list.add(0, 0);
来源：http://on.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tf.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fg.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://pl.gzmigu.cn

[D04] 删除元素
来源：http://ge.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lj.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uv.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://th.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://ek.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ob.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kg.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://el.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xx.haigaiapp.cn

[D05] 访问与修改元素
来源：http://ku.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oh.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wb.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ep.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ei.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://wc.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://zk.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ce.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fr.nszjky.cn

[D06] 数组长度
来源：http://in.jctech888.com.cn

Py:   len(arr)
来源：http://eu.shxzskj.cn

PHP:  count($arr);
来源：http://hr.szsharing.cn

JS:   arr.length
来源：http://nl.muxihuayi.cn

TS:   arr.length
来源：http://tt.asd995.cn

Java: list.size();
来源：http://ag.bjjhwx.cn

Go:   len(arr)
来源：http://dq.colortex.cn

Ruby: arr.length; arr.size
来源：http://mz.nszjky.cn

C#:   list.Count;
来源：http://bi.colortex.cn

[D07] 切片 / 取子数组
来源：http://iq.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kq.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cv.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://ou.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://dy.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://gj.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://um.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://cw.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://du.panjiajie.cn

[D08] 合并两个数组
来源：http://bt.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://rl.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://es.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bp.gzmigu.cn

TS:   [...a, ...b];
来源：http://ap.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zf.muxihuayi.cn

Go:   append(a, b...)
来源：http://aa.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://ah.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://on.haigaiapp.cn

[D09] 排序（升序）
来源：http://mw.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ow.bjjhwx.cn

PHP:  sort($arr);
来源：http://zw.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ma.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sc.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lb.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pi.9csxet.cn

Ruby: arr.sort
来源：http://vz.asd995.cn

C#:   list.Sort();
来源：http://tp.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dr.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ut.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rq.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nj.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rr.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cg.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jn.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zz.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gd.9csxet.cn

[D11] 反转数组
来源：http://mm.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fl.asd995.cn

PHP:  array_reverse($arr);
来源：http://ce.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sh.nicolike.cn

TS:   [...arr].reverse();
来源：http://re.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://ws.colortex.cn

Go:   slices.Reverse(arr)
来源：http://zh.nicolike.cn

Ruby: arr.reverse
来源：http://ys.szsharing.cn

C#:   list.Reverse();
来源：http://vg.szxytkj.cn

[D12] 查找元素下标
来源：http://qt.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://hb.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ns.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ih.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://og.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lc.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://yh.huixiangedu.cn

Ruby: arr.index(x)
来源：http://tc.asd995.cn

C#:   list.IndexOf(x);
来源：http://nj.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ls.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pn.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jp.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://zh.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://gv.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vz.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lz.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cq.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wr.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://ze.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wi.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mm.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://wg.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://ae.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qr.bjjhwx.cn

Go:   // 手写循环
来源：http://rb.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xk.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rk.jctech888.com.cn

[D15] 去重
来源：http://an.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vg.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://if.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://br.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://oz.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cn.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kr.shtwfgs.cn

Ruby: arr.uniq
来源：http://fo.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://fq.colortex.cn

[D16] 求和与平均值
来源：http://ai.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vc.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ir.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rw.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gv.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pb.newstarts.cn

Go:   // 手写循环累加
来源：http://pv.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vt.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://ur.haigaiapp.cn

[D17] 最大值与最小值
来源：http://ry.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://ru.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://ds.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://di.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://he.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ur.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rs.colortex.cn

Ruby: arr.max;  arr.min
来源：http://qd.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://pr.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://mx.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rj.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://cj.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://go.asd995.cn

TS:   nested.flat();
来源：http://as.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eg.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://mz.wgjwhj.cn

Ruby: nested.flatten
来源：http://om.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bg.9csxet.cn

[D19] 按字段分组
来源：http://yl.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jc.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sx.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nz.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cx.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fw.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://tr.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ps.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ia.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://pv.szxytkj.cn

Py:   Counter(arr)
来源：http://vg.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://la.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tg.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xi.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rx.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://oz.jctech888.com.cn

Ruby: arr.tally
来源：http://pi.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dn.colortex.cn

[D21] 判断是否包含某元素
来源：http://ol.521024.cn

Py:   x in arr
来源：http://wa.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://lb.huanxung.cn

JS:   arr.includes(x)
来源：http://kc.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://mu.9csxet.cn

Java: list.contains(x)
来源：http://qq.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://wu.szxytkj.cn

Ruby: arr.include?(x)
来源：http://cj.wgjwhj.cn

C#:   list.Contains(x)
来源：http://lq.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://im.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qi.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://om.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wq.nicolike.cn

TS:   [...arr];
来源：http://eh.colortex.cn

Java: new ArrayList<>(list);
来源：http://ik.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cf.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://qu.shxzukj.cn

C#:   new List<int>(list);
来源：http://jk.panjiajie.cn

[D23] reduce 累积计算
来源：http://lg.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pr.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wr.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bd.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gm.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aa.gzmigu.cn

Go:   // 手写循环
来源：http://rp.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fq.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lx.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://gy.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zk.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mq.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dw.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xp.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ex.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://am.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iy.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ve.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://eh.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pu.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jq.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://al.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yi.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kt.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://no.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mb.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lm.haigaiapp.cn

[D26] 数组转字符串
来源：http://rx.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://sg.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://kb.yuexingan06.cn

JS:   arr.join(", ")
来源：http://cw.szsharing.cn

TS:   arr.join(", ")
来源：http://gk.asd995.cn

Java: String.join(", ", list)
来源：http://gj.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://rw.shxzskj.cn

Ruby: arr.join(", ")
来源：http://zt.newstarts.cn

C#:   string.Join(", ", list)
来源：http://nb.bjjhwx.cn

================================================================================
来源：http://bh.yuexingan06.cn

E. 字符串处理
来源：http://wu.yuexingan06.cn

================================================================================
来源：http://oz.lnxyls.cn

[E01] 拼接字符串
来源：http://us.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hg.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bb.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rf.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rt.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://or.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lo.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rt.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fw.szsharing.cn

[E02] 重复字符串
来源：http://sn.nicolike.cn

Py:   "ab" * 3
来源：http://sl.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://vl.hahajie.cn

JS:   "ab".repeat(3)
来源：http://jf.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://xz.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://bi.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ua.lnxyls.cn

Ruby: "ab" * 3
来源：http://ln.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fd.jianghongdianzi.cn

[E03] 截取子串
来源：http://gm.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ku.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jc.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cb.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://uv.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://rw.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cn.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gp.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://ld.521024.cn

[E04] 查找子串位置
来源：http://nr.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://jz.huanxung.cn

PHP:  strpos($s, "x");
来源：http://rt.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yo.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://lj.panjiajie.cn

Java: s.indexOf("x")
来源：http://on.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://jm.bjjhwx.cn

Ruby: s.index("x")
来源：http://fe.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://qo.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cf.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://go.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://et.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bf.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gm.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hm.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tw.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mo.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fp.shtwfgs.cn


<!-- 参考信息 -->