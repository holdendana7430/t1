代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://je.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://rb.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vn.bookmarksfly.cn

================================================================================
来源：http://sp.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://rj.colortex.cn

================================================================================
来源：http://oi.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://ew.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rk.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pt.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cl.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wd.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://id.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://bp.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://xs.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jr.newstarts.cn

[D02] 追加元素到末尾
来源：http://ur.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kr.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ps.chemitech.net.cn

JS:   arr.push(4);
来源：http://na.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://bn.nicolike.cn

Java: list.add(4);
来源：http://py.asd995.cn

Go:   arr = append(arr, 4)
来源：http://xk.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://bw.nszjky.cn

C#:   list.Add(4);
来源：http://zw.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://ev.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://jo.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gw.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vm.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://be.haigaiapp.cn

Java: list.add(0, 0);
来源：http://ba.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fl.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://au.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://jw.hahajie.cn

[D04] 删除元素
来源：http://xt.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wc.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cz.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ea.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://ur.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uq.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nq.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rj.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xw.hnjuh.cn

[D05] 访问与修改元素
来源：http://ql.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fj.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jg.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cu.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://qa.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://uu.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://fm.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://up.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://te.shxzukj.cn

[D06] 数组长度
来源：http://go.bookmarksfly.cn

Py:   len(arr)
来源：http://lp.shxzukj.cn

PHP:  count($arr);
来源：http://gh.nicolike.cn

JS:   arr.length
来源：http://jp.szsharing.cn

TS:   arr.length
来源：http://pw.huanxung.cn

Java: list.size();
来源：http://ui.9csxet.cn

Go:   len(arr)
来源：http://ci.9csxet.cn

Ruby: arr.length; arr.size
来源：http://wf.hahajie.cn

C#:   list.Count;
来源：http://sc.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://gj.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vz.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ne.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://qx.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://on.newstarts.cn

Java: list.subList(1, 4);
来源：http://wg.szxytkj.cn

Go:   arr[1:4]
来源：http://yc.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://rz.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://el.9csxet.cn

[D08] 合并两个数组
来源：http://jw.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://hs.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://aq.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://il.shxzskj.cn

TS:   [...a, ...b];
来源：http://ck.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fk.nszjky.cn

Go:   append(a, b...)
来源：http://pk.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://hf.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://mi.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://ai.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://qj.huanxung.cn

PHP:  sort($arr);
来源：http://el.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yj.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ct.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mx.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cn.huanxung.cn

Ruby: arr.sort
来源：http://pi.yuexingan06.cn

C#:   list.Sort();
来源：http://fr.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lv.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zj.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qd.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ts.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ln.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ac.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tx.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bp.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zc.szxytkj.cn

[D11] 反转数组
来源：http://ql.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gb.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://et.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ie.asd995.cn

TS:   [...arr].reverse();
来源：http://ph.huanxung.cn

Java: Collections.reverse(list);
来源：http://kr.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://zk.szsharing.cn

Ruby: arr.reverse
来源：http://fg.chemitech.net.cn

C#:   list.Reverse();
来源：http://pm.panjiajie.cn

[D12] 查找元素下标
来源：http://ox.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://on.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rm.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yb.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qj.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://du.asd995.cn

Go:   slices.Index(arr, x)
来源：http://fs.muxihuayi.cn

Ruby: arr.index(x)
来源：http://yu.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://sv.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://dg.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yo.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ap.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://wx.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://aj.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ad.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ha.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jp.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zq.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://uu.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ab.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://au.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://as.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://bg.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ti.hnjuh.cn

Go:   // 手写循环
来源：http://td.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xf.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iv.gzmigu.cn

[D15] 去重
来源：http://az.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yf.asd995.cn

PHP:  array_unique($arr);
来源：http://ii.nszjky.cn

JS:   [...new Set(arr)]
来源：http://ni.9csxet.cn

TS:   [...new Set(arr)]
来源：http://fn.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ca.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vy.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://ex.521024.cn

C#:   list.Distinct().ToList()
来源：http://vv.szxytkj.cn

[D16] 求和与平均值
来源：http://rp.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kv.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xi.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hf.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://to.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ot.colortex.cn

Go:   // 手写循环累加
来源：http://ki.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zb.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://wy.hnjuh.cn

[D17] 最大值与最小值
来源：http://eb.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://si.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://zb.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xv.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://tr.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cc.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ws.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://mv.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://yj.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://mm.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sp.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://ae.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uk.gzmigu.cn

TS:   nested.flat();
来源：http://lg.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qr.gzmigu.cn

Go:   // 手写双层循环
来源：http://ui.huanxung.cn

Ruby: nested.flatten
来源：http://ah.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ks.nicolike.cn

[D19] 按字段分组
来源：http://rm.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fr.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vb.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ks.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://un.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hs.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://qd.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bb.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vr.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://px.szsharing.cn

Py:   Counter(arr)
来源：http://vk.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://fz.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cy.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zs.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hc.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://lp.bjjhwx.cn

Ruby: arr.tally
来源：http://qs.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yd.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://li.yuntaijiaju.cn

Py:   x in arr
来源：http://ny.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://xa.nszjky.cn

JS:   arr.includes(x)
来源：http://mr.panjiajie.cn

TS:   arr.includes(x)
来源：http://do.muxihuayi.cn

Java: list.contains(x)
来源：http://tv.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://tt.nszjky.cn

Ruby: arr.include?(x)
来源：http://gj.lnxyls.cn

C#:   list.Contains(x)
来源：http://oc.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://uy.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pt.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xx.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qx.szxytkj.cn

TS:   [...arr];
来源：http://gx.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://dh.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zl.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://cr.hahajie.cn

C#:   new List<int>(list);
来源：http://fh.jctech888.com.cn

[D23] reduce 累积计算
来源：http://fh.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fx.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fn.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nl.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vv.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ep.newstarts.cn

Go:   // 手写循环
来源：http://ie.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kb.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hf.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://dd.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pe.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sx.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ch.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bb.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xz.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sg.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gt.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pa.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://hl.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ek.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mj.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xn.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sc.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cb.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jx.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mu.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fb.yuexingan06.cn

[D26] 数组转字符串
来源：http://gp.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://xq.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://xr.9csxet.cn

JS:   arr.join(", ")
来源：http://na.huanxung.cn

TS:   arr.join(", ")
来源：http://qw.muxihuayi.cn

Java: String.join(", ", list)
来源：http://cc.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://kr.521024.cn

Ruby: arr.join(", ")
来源：http://bx.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://uw.huixiangedu.cn

================================================================================
来源：http://rm.muxihuayi.cn

E. 字符串处理
来源：http://hy.gzmigu.cn

================================================================================
来源：http://ne.9csxet.cn

[E01] 拼接字符串
来源：http://at.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rk.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ab.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xo.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jf.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kg.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pf.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kg.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sr.shxzskj.cn

[E02] 重复字符串
来源：http://cc.colortex.cn

Py:   "ab" * 3
来源：http://os.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://er.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://we.newstarts.cn

TS:   "ab".repeat(3)
来源：http://eq.nicolike.cn

Java: "ab".repeat(3)
来源：http://uv.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://mz.hahajie.cn

Ruby: "ab" * 3
来源：http://yd.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dt.haigaiapp.cn

[E03] 截取子串
来源：http://cf.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://on.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vh.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ee.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://ym.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://co.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://es.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://do.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://ce.szxytkj.cn

[E04] 查找子串位置
来源：http://qw.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://xs.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://hd.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rc.hnjuh.cn

TS:   s.indexOf("x")
来源：http://jo.huixiangedu.cn

Java: s.indexOf("x")
来源：http://sp.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://vg.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://nj.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://lu.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ta.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ur.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wl.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ov.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://na.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ly.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zw.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ty.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fk.szxytkj.cn

[E06] 替换子串
来源：http://sa.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yn.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://kf.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://go.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://mt.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qd.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://by.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://au.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://pi.asd995.cn

[E07] 按分隔符拆分
来源：http://cz.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nx.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uc.haigaiapp.cn


<!-- 参考信息 -->