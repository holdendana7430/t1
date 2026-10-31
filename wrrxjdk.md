代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://sr.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://vg.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ui.nszjky.cn

================================================================================
来源：http://oj.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://ir.nszjky.cn

================================================================================
来源：http://mb.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://pt.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bi.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ca.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hr.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jx.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hj.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://gj.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://ij.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oq.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://wr.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xk.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jn.huixiangedu.cn

JS:   arr.push(4);
来源：http://xb.huixiangedu.cn

TS:   arr.push(4);
来源：http://kh.jianghongdianzi.cn

Java: list.add(4);
来源：http://es.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://aj.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ij.szxytkj.cn

C#:   list.Add(4);
来源：http://qo.newstarts.cn

[D03] 在指定位置插入元素
来源：http://vb.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://uz.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lb.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fy.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://ul.hnjuh.cn

Java: list.add(0, 0);
来源：http://ct.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kr.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nf.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://im.shxzukj.cn

[D04] 删除元素
来源：http://jv.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://je.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uc.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://us.521024.cn

TS:   arr.splice(0, 1);
来源：http://uq.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sa.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ai.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jr.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mq.chemitech.net.cn

[D05] 访问与修改元素
来源：http://cq.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kg.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ya.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fx.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://ee.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://yk.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://wf.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rb.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xi.lnxyls.cn

[D06] 数组长度
来源：http://uu.nicolike.cn

Py:   len(arr)
来源：http://kw.haigaiapp.cn

PHP:  count($arr);
来源：http://xl.shxzukj.cn

JS:   arr.length
来源：http://lk.panjiajie.cn

TS:   arr.length
来源：http://ir.jctech888.com.cn

Java: list.size();
来源：http://fx.9csxet.cn

Go:   len(arr)
来源：http://hl.521024.cn

Ruby: arr.length; arr.size
来源：http://ff.jianghongdianzi.cn

C#:   list.Count;
来源：http://az.szsharing.cn

[D07] 切片 / 取子数组
来源：http://cn.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ef.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://su.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://do.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://ag.nicolike.cn

Java: list.subList(1, 4);
来源：http://en.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://zk.panjiajie.cn

Ruby: arr[1, 3]
来源：http://rp.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://uk.panjiajie.cn

[D08] 合并两个数组
来源：http://ar.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://nj.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://oh.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oe.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://tb.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ls.chemitech.net.cn

Go:   append(a, b...)
来源：http://jz.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://gp.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://uj.jctech888.com.cn

[D09] 排序（升序）
来源：http://jo.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://og.yuexingan06.cn

PHP:  sort($arr);
来源：http://pt.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fn.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cf.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fr.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fb.jianghongdianzi.cn

Ruby: arr.sort
来源：http://hd.shtwfgs.cn

C#:   list.Sort();
来源：http://qw.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yk.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://go.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wb.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ke.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ed.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ka.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mu.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lt.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oa.bookmarksfly.cn

[D11] 反转数组
来源：http://rg.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kp.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://im.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vu.nicolike.cn

TS:   [...arr].reverse();
来源：http://tj.szsharing.cn

Java: Collections.reverse(list);
来源：http://ae.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://vj.huixiangedu.cn

Ruby: arr.reverse
来源：http://xq.nicolike.cn

C#:   list.Reverse();
来源：http://bi.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://wj.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://mn.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ge.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tc.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bw.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oi.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://sp.shtwfgs.cn

Ruby: arr.index(x)
来源：http://sk.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://vf.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://px.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ln.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://id.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://fl.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://ht.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://be.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tl.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://id.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://wr.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://le.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ur.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://nx.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://yf.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ko.szsharing.cn

Go:   // 手写循环
来源：http://mm.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://si.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eg.muxihuayi.cn

[D15] 去重
来源：http://rz.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dw.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://jz.asd995.cn

JS:   [...new Set(arr)]
来源：http://zl.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://kb.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ro.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xi.newstarts.cn

Ruby: arr.uniq
来源：http://dq.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://tp.jctech888.com.cn

[D16] 求和与平均值
来源：http://yc.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://go.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mf.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xh.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yd.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fw.yuexingan06.cn

Go:   // 手写循环累加
来源：http://ib.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bi.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://ey.newstarts.cn

[D17] 最大值与最小值
来源：http://kv.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://od.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://cq.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tr.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://nm.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ta.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bc.521024.cn

Ruby: arr.max;  arr.min
来源：http://ca.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://ln.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://lj.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ah.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://al.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lt.hahajie.cn

TS:   nested.flat();
来源：http://vw.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ua.shxzukj.cn

Go:   // 手写双层循环
来源：http://ty.panjiajie.cn

Ruby: nested.flatten
来源：http://wf.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jh.szxytkj.cn

[D19] 按字段分组
来源：http://mw.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ea.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vy.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vk.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wc.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gf.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://bt.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zn.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fl.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://li.asd995.cn

Py:   Counter(arr)
来源：http://do.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://gv.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yx.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uc.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qv.szsharing.cn

Go:   // 手写 map[T]int
来源：http://gk.huanxung.cn

Ruby: arr.tally
来源：http://xp.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cd.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://xb.gzmigu.cn

Py:   x in arr
来源：http://bz.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://vq.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://lh.szsharing.cn

TS:   arr.includes(x)
来源：http://rx.szsharing.cn

Java: list.contains(x)
来源：http://db.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://kj.huanxung.cn

Ruby: arr.include?(x)
来源：http://fo.shtwfgs.cn

C#:   list.Contains(x)
来源：http://xn.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://bp.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hn.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pm.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hk.colortex.cn

TS:   [...arr];
来源：http://pe.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://xq.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rk.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://zw.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://vt.hahajie.cn

[D23] reduce 累积计算
来源：http://ny.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://no.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sl.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://je.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gc.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nz.yuntaijiaju.cn

Go:   // 手写循环
来源：http://dk.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://om.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ja.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://mo.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://or.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eo.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jr.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://az.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rv.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://du.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tv.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lk.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://vh.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ha.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ja.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sc.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gi.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ao.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ki.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yr.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xy.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://yb.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://pq.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://ge.panjiajie.cn

JS:   arr.join(", ")
来源：http://dd.colortex.cn

TS:   arr.join(", ")
来源：http://pa.colortex.cn

Java: String.join(", ", list)
来源：http://yo.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://zp.hnjuh.cn

Ruby: arr.join(", ")
来源：http://pq.521024.cn

C#:   string.Join(", ", list)
来源：http://dk.shtwfgs.cn

================================================================================
来源：http://pl.lnxyls.cn

E. 字符串处理
来源：http://jg.huixiangedu.cn

================================================================================
来源：http://vt.lnxyls.cn

[E01] 拼接字符串
来源：http://no.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qx.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ga.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xo.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pi.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vz.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zh.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ue.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oo.asd995.cn

[E02] 重复字符串
来源：http://pv.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://uv.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://rc.521024.cn

JS:   "ab".repeat(3)
来源：http://us.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://tc.nicolike.cn

Java: "ab".repeat(3)
来源：http://dd.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://qn.jctech888.com.cn

Ruby: "ab" * 3
来源：http://rh.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nk.yuntaijiaju.cn

[E03] 截取子串
来源：http://ym.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vu.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dz.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dp.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://ej.521024.cn

Java: s.substring(1, 4)
来源：http://yi.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://im.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mw.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://ar.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://gz.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://qb.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://ct.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gm.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://ye.muxihuayi.cn

Java: s.indexOf("x")
来源：http://do.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://wa.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://dc.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://pt.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lv.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lw.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mn.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pv.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zm.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ch.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yr.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ih.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ae.haigaiapp.cn

[E06] 替换子串
来源：http://im.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ne.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://ra.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://in.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://yk.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ah.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sv.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gv.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://bb.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://bl.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qg.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rk.szsharing.cn


<!-- 参考信息 -->