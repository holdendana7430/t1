代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eq.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zv.jianghongdianzi.cn

Java: // 无解构
来源：http://xg.huanxung.cn

Go:   // 无解构
来源：http://io.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://jv.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://pk.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://iv.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qq.jianghongdianzi.cn

PHP:  // 无重载
来源：http://nf.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qy.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ta.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ig.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://nd.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://ws.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tq.chemitech.net.cn

================================================================================
来源：http://xf.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://eb.szxytkj.cn

================================================================================
来源：http://cw.szsharing.cn

[D01] 创建数组 / 列表
来源：http://cf.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hp.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qz.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wm.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uw.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xd.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://sz.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://kl.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qo.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://fo.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gd.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lv.bjjhwx.cn

JS:   arr.push(4);
来源：http://sv.bookmarksfly.cn

TS:   arr.push(4);
来源：http://wk.wgjwhj.cn

Java: list.add(4);
来源：http://hq.asd995.cn

Go:   arr = append(arr, 4)
来源：http://uv.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://ma.shxzukj.cn

C#:   list.Add(4);
来源：http://pn.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://ed.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://xp.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rm.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ca.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://py.huanxung.cn

Java: list.add(0, 0);
来源：http://jp.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://by.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zj.asd995.cn

C#:   list.Insert(0, 0);
来源：http://qu.yuexingan06.cn

[D04] 删除元素
来源：http://ff.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://li.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sq.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://id.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://su.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dg.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ud.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://su.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ka.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://fu.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rg.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ik.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zf.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://hx.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://si.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://di.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://de.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rv.huanxung.cn

[D06] 数组长度
来源：http://ep.newstarts.cn

Py:   len(arr)
来源：http://aa.shxzskj.cn

PHP:  count($arr);
来源：http://iu.haigaiapp.cn

JS:   arr.length
来源：http://ir.yuexingan06.cn

TS:   arr.length
来源：http://qr.jianghongdianzi.cn

Java: list.size();
来源：http://um.shxzskj.cn

Go:   len(arr)
来源：http://zj.colortex.cn

Ruby: arr.length; arr.size
来源：http://yg.newstarts.cn

C#:   list.Count;
来源：http://az.nszjky.cn

[D07] 切片 / 取子数组
来源：http://kf.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bc.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wf.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://bg.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://zq.newstarts.cn

Java: list.subList(1, 4);
来源：http://ng.huanxung.cn

Go:   arr[1:4]
来源：http://sm.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://xt.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://lz.shxzukj.cn

[D08] 合并两个数组
来源：http://iu.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://ut.colortex.cn

PHP:  array_merge($a, $b);
来源：http://ow.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lj.nicolike.cn

TS:   [...a, ...b];
来源：http://db.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ds.yuexingan06.cn

Go:   append(a, b...)
来源：http://fe.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://wg.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://fy.hahajie.cn

[D09] 排序（升序）
来源：http://gh.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://tu.chemitech.net.cn

PHP:  sort($arr);
来源：http://hl.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ap.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yn.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xd.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rq.asd995.cn

Ruby: arr.sort
来源：http://gm.huixinmuqiang.cn

C#:   list.Sort();
来源：http://zc.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yt.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gj.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wp.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mc.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://om.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wy.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lt.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bn.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://es.huixinmuqiang.cn

[D11] 反转数组
来源：http://hi.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bv.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://wu.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://px.szxytkj.cn

TS:   [...arr].reverse();
来源：http://ka.szxytkj.cn

Java: Collections.reverse(list);
来源：http://gk.521024.cn

Go:   slices.Reverse(arr)
来源：http://hx.asd995.cn

Ruby: arr.reverse
来源：http://sk.nicolike.cn

C#:   list.Reverse();
来源：http://sr.szxytkj.cn

[D12] 查找元素下标
来源：http://sq.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://to.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hh.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ev.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fs.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eh.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://bq.wgjwhj.cn

Ruby: arr.index(x)
来源：http://dj.colortex.cn

C#:   list.IndexOf(x);
来源：http://ju.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ns.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://se.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yu.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://la.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://fo.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pg.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aa.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oq.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vm.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://el.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hx.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mo.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://bk.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://eh.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mg.newstarts.cn

Go:   // 手写循环
来源：http://ir.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kw.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cq.jctech888.com.cn

[D15] 去重
来源：http://yd.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zr.szsharing.cn

PHP:  array_unique($arr);
来源：http://jf.huanxung.cn

JS:   [...new Set(arr)]
来源：http://ik.nicolike.cn

TS:   [...new Set(arr)]
来源：http://kv.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zw.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://df.bookmarksfly.cn

Ruby: arr.uniq
来源：http://sf.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://um.521024.cn

[D16] 求和与平均值
来源：http://do.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://th.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ah.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ap.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ig.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kh.nicolike.cn

Go:   // 手写循环累加
来源：http://ef.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xg.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://la.bjjhwx.cn

[D17] 最大值与最小值
来源：http://ou.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://cl.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://xn.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://en.szsharing.cn

TS:   Math.max(...arr);
来源：http://nm.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wn.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://he.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://mc.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://nk.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://ak.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ho.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://vb.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gj.chemitech.net.cn

TS:   nested.flat();
来源：http://ad.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tr.panjiajie.cn

Go:   // 手写双层循环
来源：http://il.huanxung.cn

Ruby: nested.flatten
来源：http://gp.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ky.bjjhwx.cn

[D19] 按字段分组
来源：http://tj.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gb.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bn.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sk.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jg.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jr.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://ev.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ax.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xj.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://on.yuexingan06.cn

Py:   Counter(arr)
来源：http://xd.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://hl.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cv.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://di.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jz.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://bi.newstarts.cn

Ruby: arr.tally
来源：http://mw.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ou.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://le.szxytkj.cn

Py:   x in arr
来源：http://rh.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://uo.shtwfgs.cn

JS:   arr.includes(x)
来源：http://iy.jctech888.com.cn

TS:   arr.includes(x)
来源：http://nu.szsharing.cn

Java: list.contains(x)
来源：http://wk.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://rw.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://my.shxzskj.cn

C#:   list.Contains(x)
来源：http://tj.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://zt.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lb.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kp.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kt.szsharing.cn

TS:   [...arr];
来源：http://ad.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://mu.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cg.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://az.colortex.cn

C#:   new List<int>(list);
来源：http://be.jctech888.com.cn

[D23] reduce 累积计算
来源：http://ta.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ow.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ln.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gz.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dr.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uf.huixiangedu.cn

Go:   // 手写循环
来源：http://ok.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nt.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ha.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://sb.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hk.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gf.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://le.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pr.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qe.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gt.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gu.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zp.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://og.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ij.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sd.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oj.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ex.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://du.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qx.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oa.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fb.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://sr.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://ys.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://ca.shxzskj.cn

JS:   arr.join(", ")
来源：http://eq.chemitech.net.cn

TS:   arr.join(", ")
来源：http://nc.szxytkj.cn

Java: String.join(", ", list)
来源：http://qc.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://ft.9csxet.cn

Ruby: arr.join(", ")
来源：http://xi.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://ve.hnjuh.cn

================================================================================
来源：http://an.jianghongdianzi.cn

E. 字符串处理
来源：http://ax.huixinmuqiang.cn

================================================================================
来源：http://pz.szxytkj.cn

[E01] 拼接字符串
来源：http://gg.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sq.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ml.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qj.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cg.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yn.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sz.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bc.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rz.shxzskj.cn

[E02] 重复字符串
来源：http://ks.panjiajie.cn

Py:   "ab" * 3
来源：http://mu.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://ph.szsharing.cn

JS:   "ab".repeat(3)
来源：http://yj.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://mt.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://xr.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://is.bjjhwx.cn

Ruby: "ab" * 3
来源：http://vy.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ot.wgjwhj.cn

[E03] 截取子串
来源：http://yp.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ah.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kk.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jt.asd995.cn

TS:   s.slice(1, 4)
来源：http://hg.colortex.cn

Java: s.substring(1, 4)
来源：http://qx.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dc.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qv.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://oj.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://vh.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://ve.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://cm.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gt.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://ph.shxzukj.cn

Java: s.indexOf("x")
来源：http://qb.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://sd.szsharing.cn

Ruby: s.index("x")
来源：http://pq.nicolike.cn

C#:   s.IndexOf("x")
来源：http://xc.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bw.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cw.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sy.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ek.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pk.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fj.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fh.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wx.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hs.bjjhwx.cn


<!-- 参考信息 -->