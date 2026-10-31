代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://iq.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://eo.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pe.szxytkj.cn

================================================================================
来源：http://fy.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://xw.bookmarksfly.cn

================================================================================
来源：http://ke.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://up.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yr.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jm.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xv.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sj.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oz.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://xk.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://ld.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cc.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://ct.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jw.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uh.yuexingan06.cn

JS:   arr.push(4);
来源：http://wd.szxytkj.cn

TS:   arr.push(4);
来源：http://op.huixinmuqiang.cn

Java: list.add(4);
来源：http://pe.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://zl.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://ir.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://jd.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://xv.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://di.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://da.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vx.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://lx.lnxyls.cn

Java: list.add(0, 0);
来源：http://bi.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tj.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://az.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://ao.muxihuayi.cn

[D04] 删除元素
来源：http://kd.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ie.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yw.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bl.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://td.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kd.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cd.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jb.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ka.asd995.cn

[D05] 访问与修改元素
来源：http://as.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ix.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hn.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://am.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ye.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://kp.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://fq.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cn.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ez.panjiajie.cn

[D06] 数组长度
来源：http://cm.lnxyls.cn

Py:   len(arr)
来源：http://pe.521024.cn

PHP:  count($arr);
来源：http://sc.newstarts.cn

JS:   arr.length
来源：http://vl.shtwfgs.cn

TS:   arr.length
来源：http://db.huanxung.cn

Java: list.size();
来源：http://wo.521024.cn

Go:   len(arr)
来源：http://wx.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://yi.bjjhwx.cn

C#:   list.Count;
来源：http://ac.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://sq.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wq.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://da.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://hr.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://td.nszjky.cn

Java: list.subList(1, 4);
来源：http://wr.szsharing.cn

Go:   arr[1:4]
来源：http://se.hahajie.cn

Ruby: arr[1, 3]
来源：http://cp.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://yn.9csxet.cn

[D08] 合并两个数组
来源：http://su.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://js.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://pi.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bx.shxzskj.cn

TS:   [...a, ...b];
来源：http://ws.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kv.521024.cn

Go:   append(a, b...)
来源：http://kv.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://ys.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://pa.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://xl.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://dl.szxytkj.cn

PHP:  sort($arr);
来源：http://pc.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ex.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aq.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bp.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bl.shtwfgs.cn

Ruby: arr.sort
来源：http://dv.gzmigu.cn

C#:   list.Sort();
来源：http://mu.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lf.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dn.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ud.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ux.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lv.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lj.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mq.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wh.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wu.jctech888.com.cn

[D11] 反转数组
来源：http://zk.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dk.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://yc.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xm.asd995.cn

TS:   [...arr].reverse();
来源：http://ra.nicolike.cn

Java: Collections.reverse(list);
来源：http://kh.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://zy.newstarts.cn

Ruby: arr.reverse
来源：http://mc.panjiajie.cn

C#:   list.Reverse();
来源：http://ct.shxzskj.cn

[D12] 查找元素下标
来源：http://dq.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://rw.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yd.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://je.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oq.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://br.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://cv.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://af.newstarts.cn

C#:   list.IndexOf(x);
来源：http://yd.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://on.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sb.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yz.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://bx.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://op.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mb.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pp.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kq.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yv.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://zl.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pf.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://td.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://sz.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://nj.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hh.9csxet.cn

Go:   // 手写循环
来源：http://bl.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bz.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ta.yuexingan06.cn

[D15] 去重
来源：http://lx.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ey.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://ad.9csxet.cn

JS:   [...new Set(arr)]
来源：http://nj.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://qa.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ox.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nr.521024.cn

Ruby: arr.uniq
来源：http://kf.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://dv.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://rb.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zo.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oo.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wk.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fj.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nm.asd995.cn

Go:   // 手写循环累加
来源：http://uq.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ea.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://dj.jctech888.com.cn

[D17] 最大值与最小值
来源：http://ny.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://tx.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://th.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lz.lnxyls.cn

TS:   Math.max(...arr);
来源：http://bq.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wj.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yd.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://fd.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://wr.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://ba.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dj.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://qp.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://db.huanxung.cn

TS:   nested.flat();
来源：http://ev.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jk.shxzskj.cn

Go:   // 手写双层循环
来源：http://fi.szxytkj.cn

Ruby: nested.flatten
来源：http://fs.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jw.asd995.cn

[D19] 按字段分组
来源：http://ft.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bq.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ol.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qq.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nl.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oh.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://yt.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bc.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fr.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://ul.shxzukj.cn

Py:   Counter(arr)
来源：http://kd.szsharing.cn

PHP:  array_count_values($arr);
来源：http://ep.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bb.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iy.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oq.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://bx.jianghongdianzi.cn

Ruby: arr.tally
来源：http://ht.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yv.colortex.cn

[D21] 判断是否包含某元素
来源：http://ld.asd995.cn

Py:   x in arr
来源：http://ay.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://ws.panjiajie.cn

JS:   arr.includes(x)
来源：http://lp.szxytkj.cn

TS:   arr.includes(x)
来源：http://gu.jctech888.com.cn

Java: list.contains(x)
来源：http://pb.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://wm.lnxyls.cn

Ruby: arr.include?(x)
来源：http://si.szxytkj.cn

C#:   list.Contains(x)
来源：http://bq.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://qn.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vn.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dn.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bk.lnxyls.cn

TS:   [...arr];
来源：http://im.colortex.cn

Java: new ArrayList<>(list);
来源：http://xi.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gz.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://be.jctech888.com.cn

C#:   new List<int>(list);
来源：http://xh.bjjhwx.cn

[D23] reduce 累积计算
来源：http://ex.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lh.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zh.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kx.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gc.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mp.jianghongdianzi.cn

Go:   // 手写循环
来源：http://hi.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yj.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://re.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://qq.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gr.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://se.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zb.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cu.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dp.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vs.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xq.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ke.521024.cn

[D25] Set 集合去重与交并差
来源：http://zg.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xs.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dk.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xh.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ar.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dk.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ft.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vg.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xe.jctech888.com.cn

[D26] 数组转字符串
来源：http://ir.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://kc.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://yc.muxihuayi.cn

JS:   arr.join(", ")
来源：http://sp.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://qf.haigaiapp.cn

Java: String.join(", ", list)
来源：http://js.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://qz.hnjuh.cn

Ruby: arr.join(", ")
来源：http://iw.nicolike.cn

C#:   string.Join(", ", list)
来源：http://rj.bjjhwx.cn

================================================================================
来源：http://ak.jianghongdianzi.cn

E. 字符串处理
来源：http://ko.haigaiapp.cn

================================================================================
来源：http://zx.shtwfgs.cn

[E01] 拼接字符串
来源：http://qm.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ni.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://em.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jv.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://je.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qm.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uq.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xs.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ay.yuexingan06.cn

[E02] 重复字符串
来源：http://le.shxzukj.cn

Py:   "ab" * 3
来源：http://eo.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://ku.nicolike.cn

JS:   "ab".repeat(3)
来源：http://ju.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://tz.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://uj.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://uf.asd995.cn

Ruby: "ab" * 3
来源：http://at.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ew.yuexingan06.cn

[E03] 截取子串
来源：http://zg.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zf.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ps.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lk.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://zy.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://sa.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kp.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ak.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://yh.chemitech.net.cn

[E04] 查找子串位置
来源：http://wy.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://yy.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://ab.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bm.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://lb.nszjky.cn

Java: s.indexOf("x")
来源：http://ez.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://qk.jctech888.com.cn

Ruby: s.index("x")
来源：http://id.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://xo.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ob.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dt.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ox.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qb.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eb.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qr.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sf.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ew.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nb.lnxyls.cn

[E06] 替换子串
来源：http://mo.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ce.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://vr.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ph.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://vl.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fx.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oo.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sq.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://dw.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://il.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ri.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nm.nszjky.cn


<!-- 参考信息 -->