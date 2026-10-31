代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://do.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vp.huixinmuqiang.cn

Java: // 无解构
来源：http://pt.shxzukj.cn

Go:   // 无解构
来源：http://bs.lnxyls.cn

Ruby: a, b = pair
来源：http://on.szsharing.cn

C#:   var (a, b) = pair;
来源：http://cs.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://mk.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sw.chemitech.net.cn

PHP:  // 无重载
来源：http://gl.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://su.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://pf.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hg.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://rk.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://li.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qu.bookmarksfly.cn

================================================================================
来源：http://ro.colortex.cn

D. 数组 / 列表 / 集合
来源：http://ce.gzmigu.cn

================================================================================
来源：http://pj.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://qu.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mc.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cv.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zh.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gx.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iw.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://yr.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://cb.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kq.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://vn.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oo.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tw.panjiajie.cn

JS:   arr.push(4);
来源：http://sn.nicolike.cn

TS:   arr.push(4);
来源：http://be.jianghongdianzi.cn

Java: list.add(4);
来源：http://je.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://sq.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ld.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://hj.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://gq.521024.cn

Py:   arr.insert(0, 0)
来源：http://iq.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nn.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://be.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://bt.521024.cn

Java: list.add(0, 0);
来源：http://ez.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zl.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uw.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://sq.szxytkj.cn

[D04] 删除元素
来源：http://os.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jb.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://py.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tu.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://rs.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ll.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mf.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rp.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rf.jctech888.com.cn

[D05] 访问与修改元素
来源：http://xd.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xj.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://py.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fd.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://sg.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://yq.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://uy.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fk.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oq.jctech888.com.cn

[D06] 数组长度
来源：http://lv.shtwfgs.cn

Py:   len(arr)
来源：http://mp.bjjhwx.cn

PHP:  count($arr);
来源：http://gw.szsharing.cn

JS:   arr.length
来源：http://gk.yuexingan06.cn

TS:   arr.length
来源：http://pa.shxzskj.cn

Java: list.size();
来源：http://ur.hnjuh.cn

Go:   len(arr)
来源：http://oi.nicolike.cn

Ruby: arr.length; arr.size
来源：http://fj.nicolike.cn

C#:   list.Count;
来源：http://jp.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://gx.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ht.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bz.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://il.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://ck.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://fp.gzmigu.cn

Go:   arr[1:4]
来源：http://lf.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://va.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://md.nszjky.cn

[D08] 合并两个数组
来源：http://fu.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://lj.521024.cn

PHP:  array_merge($a, $b);
来源：http://ma.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gr.521024.cn

TS:   [...a, ...b];
来源：http://ig.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fb.yuexingan06.cn

Go:   append(a, b...)
来源：http://yk.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://bl.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://vd.jctech888.com.cn

[D09] 排序（升序）
来源：http://jd.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://xx.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://up.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://se.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cv.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://on.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ad.szxytkj.cn

Ruby: arr.sort
来源：http://xb.jctech888.com.cn

C#:   list.Sort();
来源：http://vi.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fx.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bi.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dy.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qs.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ub.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ao.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pm.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mk.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ja.shxzskj.cn

[D11] 反转数组
来源：http://eb.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ag.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://qn.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://de.newstarts.cn

TS:   [...arr].reverse();
来源：http://cl.hahajie.cn

Java: Collections.reverse(list);
来源：http://uc.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://lr.yuexingan06.cn

Ruby: arr.reverse
来源：http://zh.colortex.cn

C#:   list.Reverse();
来源：http://zw.chemitech.net.cn

[D12] 查找元素下标
来源：http://ft.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://im.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iw.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nc.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qi.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lf.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://zx.gzmigu.cn

Ruby: arr.index(x)
来源：http://ji.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://io.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://zn.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bt.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oi.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://vx.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://qg.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eg.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bw.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hj.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nv.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://sy.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cj.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://op.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://zv.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://kv.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uf.huixinmuqiang.cn

Go:   // 手写循环
来源：http://wt.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mw.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ye.yuexingan06.cn

[D15] 去重
来源：http://xa.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pi.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://sf.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://qt.nszjky.cn

TS:   [...new Set(arr)]
来源：http://ko.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jk.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gj.szxytkj.cn

Ruby: arr.uniq
来源：http://hu.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://qe.hahajie.cn

[D16] 求和与平均值
来源：http://gy.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://df.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ey.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mn.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cm.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dh.szxytkj.cn

Go:   // 手写循环累加
来源：http://tl.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oz.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://ym.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://iq.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://nz.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://px.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ow.521024.cn

TS:   Math.max(...arr);
来源：http://mf.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zs.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ps.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://ru.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://pq.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://xe.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ig.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://tm.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ji.jianghongdianzi.cn

TS:   nested.flat();
来源：http://ib.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nw.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://ma.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://zj.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://or.hahajie.cn

[D19] 按字段分组
来源：http://on.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sq.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jt.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://er.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gq.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rv.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://hl.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zw.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://go.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://ls.jctech888.com.cn

Py:   Counter(arr)
来源：http://ug.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://qc.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fz.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ja.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wj.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://mm.muxihuayi.cn

Ruby: arr.tally
来源：http://de.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ka.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://pd.yuexingan06.cn

Py:   x in arr
来源：http://kt.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://bj.yuexingan06.cn

JS:   arr.includes(x)
来源：http://mv.panjiajie.cn

TS:   arr.includes(x)
来源：http://ph.yuntaijiaju.cn

Java: list.contains(x)
来源：http://yr.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://sf.hahajie.cn

Ruby: arr.include?(x)
来源：http://jw.colortex.cn

C#:   list.Contains(x)
来源：http://iv.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://nm.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xj.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kh.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kr.yuexingan06.cn

TS:   [...arr];
来源：http://uv.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://hy.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zt.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://fj.asd995.cn

C#:   new List<int>(list);
来源：http://pl.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://bw.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kc.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ld.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mq.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bx.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jw.muxihuayi.cn

Go:   // 手写循环
来源：http://cy.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uq.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cf.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://wa.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wc.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://et.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wa.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vl.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://za.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qk.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zp.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mv.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://wu.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uj.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iz.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fx.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://za.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vx.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ms.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pw.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sd.shtwfgs.cn

[D26] 数组转字符串
来源：http://gi.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://sl.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://pw.9csxet.cn

JS:   arr.join(", ")
来源：http://uf.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://oe.bjjhwx.cn

Java: String.join(", ", list)
来源：http://sr.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://bj.huanxung.cn

Ruby: arr.join(", ")
来源：http://ih.nszjky.cn

C#:   string.Join(", ", list)
来源：http://fp.asd995.cn

================================================================================
来源：http://fi.huixiangedu.cn

E. 字符串处理
来源：http://yc.panjiajie.cn

================================================================================
来源：http://uo.panjiajie.cn

[E01] 拼接字符串
来源：http://zi.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gh.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sa.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bj.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fl.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kk.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uw.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rs.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qi.jctech888.com.cn

[E02] 重复字符串
来源：http://sd.asd995.cn

Py:   "ab" * 3
来源：http://xb.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://pi.hahajie.cn

JS:   "ab".repeat(3)
来源：http://vr.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://pw.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://sg.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://wi.haigaiapp.cn

Ruby: "ab" * 3
来源：http://ap.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hm.shxzukj.cn

[E03] 截取子串
来源：http://wa.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sc.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wi.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oj.521024.cn

TS:   s.slice(1, 4)
来源：http://eq.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://tx.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ze.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nz.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://ro.shxzukj.cn

[E04] 查找子串位置
来源：http://bj.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://im.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://wb.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sa.gzmigu.cn

TS:   s.indexOf("x")
来源：http://sv.lnxyls.cn

Java: s.indexOf("x")
来源：http://fc.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://zi.9csxet.cn

Ruby: s.index("x")
来源：http://vc.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://ye.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xm.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://im.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://id.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://do.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xm.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ix.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ap.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hx.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wp.chemitech.net.cn


<!-- 参考信息 -->