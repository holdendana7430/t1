代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rr.szsharing.cn

[C15] 解构 / 展开参数
来源：http://sl.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fs.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://yq.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eo.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pr.muxihuayi.cn

Java: // 无解构
来源：http://tp.panjiajie.cn

Go:   // 无解构
来源：http://wm.jctech888.com.cn

Ruby: a, b = pair
来源：http://df.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://jl.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://yc.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oa.szxytkj.cn

PHP:  // 无重载
来源：http://wj.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://le.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ji.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yj.szxytkj.cn

Go:   // 无重载：用不同函数名
来源：http://ev.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://ts.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bd.yuntaijiaju.cn

================================================================================
来源：http://dp.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://sy.shxzukj.cn

================================================================================
来源：http://hn.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://ds.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bo.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dd.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ke.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fv.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tf.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://eb.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://nh.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gj.shxzukj.cn

[D02] 追加元素到末尾
来源：http://td.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zf.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pw.521024.cn

JS:   arr.push(4);
来源：http://fn.lnxyls.cn

TS:   arr.push(4);
来源：http://xm.nicolike.cn

Java: list.add(4);
来源：http://tn.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://iz.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://cl.nszjky.cn

C#:   list.Add(4);
来源：http://aq.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://sx.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://sc.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://os.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hy.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://dh.shxzskj.cn

Java: list.add(0, 0);
来源：http://tg.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yt.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qs.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://lj.huixinmuqiang.cn

[D04] 删除元素
来源：http://wu.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ia.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wr.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kg.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://li.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ta.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fe.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rj.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yp.nszjky.cn

[D05] 访问与修改元素
来源：http://op.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dt.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ru.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ze.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://os.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://dg.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://bj.panjiajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xn.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zy.chemitech.net.cn

[D06] 数组长度
来源：http://ts.jctech888.com.cn

Py:   len(arr)
来源：http://xv.jctech888.com.cn

PHP:  count($arr);
来源：http://nd.huixiangedu.cn

JS:   arr.length
来源：http://ux.shxzskj.cn

TS:   arr.length
来源：http://qg.nicolike.cn

Java: list.size();
来源：http://my.szsharing.cn

Go:   len(arr)
来源：http://ig.szsharing.cn

Ruby: arr.length; arr.size
来源：http://sd.yuexingan06.cn

C#:   list.Count;
来源：http://kt.521024.cn

[D07] 切片 / 取子数组
来源：http://ov.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jm.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qj.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://lp.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://fe.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://em.muxihuayi.cn

Go:   arr[1:4]
来源：http://lf.nicolike.cn

Ruby: arr[1, 3]
来源：http://qj.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://ab.lnxyls.cn

[D08] 合并两个数组
来源：http://gt.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://wy.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://jd.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tg.nicolike.cn

TS:   [...a, ...b];
来源：http://si.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cm.shxzukj.cn

Go:   append(a, b...)
来源：http://pw.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://cy.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://rn.muxihuayi.cn

[D09] 排序（升序）
来源：http://na.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://wx.bjjhwx.cn

PHP:  sort($arr);
来源：http://dh.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ek.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nw.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cu.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://el.haigaiapp.cn

Ruby: arr.sort
来源：http://jy.szxytkj.cn

C#:   list.Sort();
来源：http://by.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://al.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oo.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wh.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hn.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cy.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vk.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xs.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fz.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rx.hnjuh.cn

[D11] 反转数组
来源：http://yj.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://be.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://xq.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://br.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://jm.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://cv.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://cd.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://ba.shxzskj.cn

C#:   list.Reverse();
来源：http://ya.bjjhwx.cn

[D12] 查找元素下标
来源：http://al.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://tt.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mu.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://az.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gp.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qw.asd995.cn

Go:   slices.Index(arr, x)
来源：http://jd.panjiajie.cn

Ruby: arr.index(x)
来源：http://ne.colortex.cn

C#:   list.IndexOf(x);
来源：http://uo.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://nm.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dg.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ax.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://wl.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://ok.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sy.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://af.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fk.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gs.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://xr.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wf.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://un.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://rn.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://ay.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zg.shxzskj.cn

Go:   // 手写循环
来源：http://yn.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nx.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hr.yuntaijiaju.cn

[D15] 去重
来源：http://bx.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xd.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://to.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://hd.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://lp.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qr.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pe.asd995.cn

Ruby: arr.uniq
来源：http://rv.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://zb.9csxet.cn

[D16] 求和与平均值
来源：http://te.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gz.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bk.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yu.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xg.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vw.nszjky.cn

Go:   // 手写循环累加
来源：http://pa.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lp.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://ix.gzmigu.cn

[D17] 最大值与最小值
来源：http://zk.521024.cn

Py:   max(arr);  min(arr)
来源：http://gb.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://zt.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zd.huanxung.cn

TS:   Math.max(...arr);
来源：http://za.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kp.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vs.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://nh.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://hx.521024.cn

[D18] 扁平化嵌套数组
来源：http://hn.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vo.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://oa.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yb.newstarts.cn

TS:   nested.flat();
来源：http://bt.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://af.chemitech.net.cn

Go:   // 手写双层循环
来源：http://yl.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://je.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bk.yuexingan06.cn

[D19] 按字段分组
来源：http://tj.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ps.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://je.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kd.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ua.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vv.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://dt.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://io.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aw.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://bx.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://fr.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://ui.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nx.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oi.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ll.huanxung.cn

Go:   // 手写 map[T]int
来源：http://sx.jianghongdianzi.cn

Ruby: arr.tally
来源：http://gn.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wg.asd995.cn

[D21] 判断是否包含某元素
来源：http://es.nszjky.cn

Py:   x in arr
来源：http://cg.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://br.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://kq.newstarts.cn

TS:   arr.includes(x)
来源：http://hm.chemitech.net.cn

Java: list.contains(x)
来源：http://wd.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://ld.colortex.cn

Ruby: arr.include?(x)
来源：http://lx.hnjuh.cn

C#:   list.Contains(x)
来源：http://oz.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://tj.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gw.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lz.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sw.shtwfgs.cn

TS:   [...arr];
来源：http://ca.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://ea.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kq.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://dr.huanxung.cn

C#:   new List<int>(list);
来源：http://tw.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://cq.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uw.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qe.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uh.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uw.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oc.jctech888.com.cn

Go:   // 手写循环
来源：http://uz.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ja.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dt.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://uc.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cr.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://io.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dl.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xk.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ka.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wv.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oc.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yt.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://ra.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ne.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oj.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ew.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fl.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rm.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nb.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ic.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ct.shtwfgs.cn

[D26] 数组转字符串
来源：http://bf.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://hu.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://mf.haigaiapp.cn

JS:   arr.join(", ")
来源：http://yq.szxytkj.cn

TS:   arr.join(", ")
来源：http://zs.521024.cn

Java: String.join(", ", list)
来源：http://il.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://mu.hnjuh.cn

Ruby: arr.join(", ")
来源：http://pp.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://is.bookmarksfly.cn

================================================================================
来源：http://dh.lnxyls.cn

E. 字符串处理
来源：http://sn.huixinmuqiang.cn

================================================================================
来源：http://yg.chemitech.net.cn

[E01] 拼接字符串
来源：http://qk.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cg.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cn.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://so.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ei.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mk.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ak.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sg.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pp.hahajie.cn

[E02] 重复字符串
来源：http://iq.hnjuh.cn

Py:   "ab" * 3
来源：http://yb.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://pe.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://oa.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://xp.521024.cn

Java: "ab".repeat(3)
来源：http://sh.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://hx.haigaiapp.cn

Ruby: "ab" * 3
来源：http://pd.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zc.jianghongdianzi.cn

[E03] 截取子串
来源：http://wg.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xe.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ie.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hk.9csxet.cn

TS:   s.slice(1, 4)
来源：http://wo.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://dv.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://is.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kd.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://lf.haigaiapp.cn

[E04] 查找子串位置
来源：http://wm.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://oe.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://ff.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lk.colortex.cn

TS:   s.indexOf("x")
来源：http://vf.wgjwhj.cn

Java: s.indexOf("x")
来源：http://zo.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://hb.colortex.cn

Ruby: s.index("x")
来源：http://ge.hahajie.cn

C#:   s.IndexOf("x")
来源：http://qm.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vg.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uh.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tx.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wm.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oz.hnjuh.cn


<!-- 参考信息 -->