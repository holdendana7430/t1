代发 wailian999

Ruby: a, b = pair
来源：http://rz.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://kr.521024.cn

[C16] 函数 / 方法重载
来源：http://jy.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nr.haigaiapp.cn

PHP:  // 无重载
来源：http://cp.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ta.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://nj.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hk.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://oc.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://uw.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hc.huanxung.cn

================================================================================
来源：http://cb.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://ul.bjjhwx.cn

================================================================================
来源：http://vw.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://uk.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mr.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eh.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bi.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vn.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ot.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://zl.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://oi.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iu.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://fq.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xl.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mk.nszjky.cn

JS:   arr.push(4);
来源：http://og.colortex.cn

TS:   arr.push(4);
来源：http://cm.yuexingan06.cn

Java: list.add(4);
来源：http://nf.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://yp.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://fm.wgjwhj.cn

C#:   list.Add(4);
来源：http://rv.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://hm.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://op.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ps.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eb.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://dr.shxzskj.cn

Java: list.add(0, 0);
来源：http://bb.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://or.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://io.521024.cn

C#:   list.Insert(0, 0);
来源：http://cg.asd995.cn

[D04] 删除元素
来源：http://bw.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dq.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tv.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ol.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://fy.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ph.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://en.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ug.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mi.szsharing.cn

[D05] 访问与修改元素
来源：http://we.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rz.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ux.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ii.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://nh.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://dk.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://al.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kc.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gv.bookmarksfly.cn

[D06] 数组长度
来源：http://nb.jianghongdianzi.cn

Py:   len(arr)
来源：http://ts.hnjuh.cn

PHP:  count($arr);
来源：http://ko.nszjky.cn

JS:   arr.length
来源：http://cy.9csxet.cn

TS:   arr.length
来源：http://wd.bjjhwx.cn

Java: list.size();
来源：http://vy.panjiajie.cn

Go:   len(arr)
来源：http://kw.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://gp.jctech888.com.cn

C#:   list.Count;
来源：http://ig.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://wq.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ji.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ba.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://xw.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://bz.lnxyls.cn

Java: list.subList(1, 4);
来源：http://ny.yuexingan06.cn

Go:   arr[1:4]
来源：http://ky.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://og.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://lk.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://ka.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://ec.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://bj.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uy.9csxet.cn

TS:   [...a, ...b];
来源：http://kj.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bl.shxzukj.cn

Go:   append(a, b...)
来源：http://uv.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://zr.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://sp.yuexingan06.cn

[D09] 排序（升序）
来源：http://sq.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://sz.huanxung.cn

PHP:  sort($arr);
来源：http://gp.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qb.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://em.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yu.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cs.nicolike.cn

Ruby: arr.sort
来源：http://en.bjjhwx.cn

C#:   list.Sort();
来源：http://fe.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fs.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mz.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pw.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://we.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kv.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bb.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sq.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ei.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gk.nicolike.cn

[D11] 反转数组
来源：http://to.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nt.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://ko.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ti.newstarts.cn

TS:   [...arr].reverse();
来源：http://jm.shxzukj.cn

Java: Collections.reverse(list);
来源：http://gw.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://qk.colortex.cn

Ruby: arr.reverse
来源：http://dv.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://xn.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://fn.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://yr.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sl.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qn.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wz.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gp.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://fz.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://qv.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://ch.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://xg.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ze.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mq.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://zq.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://da.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://re.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ua.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lj.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ox.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://jc.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hl.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jp.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://mn.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://sw.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://je.hnjuh.cn

Go:   // 手写循环
来源：http://os.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sk.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nm.newstarts.cn

[D15] 去重
来源：http://vx.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yr.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://sr.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://ez.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://cw.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rs.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hx.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://vu.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://fj.chemitech.net.cn

[D16] 求和与平均值
来源：http://rf.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rk.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hb.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nw.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ca.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cu.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://ru.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zd.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://qw.hnjuh.cn

[D17] 最大值与最小值
来源：http://ae.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://ua.521024.cn

PHP:  max($arr);  min($arr);
来源：http://ya.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ib.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://qo.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ok.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fe.521024.cn

Ruby: arr.max;  arr.min
来源：http://mp.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://ox.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://ck.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mz.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://gz.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rz.hnjuh.cn

TS:   nested.flat();
来源：http://eo.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kw.hahajie.cn

Go:   // 手写双层循环
来源：http://sp.9csxet.cn

Ruby: nested.flatten
来源：http://rr.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://un.colortex.cn

[D19] 按字段分组
来源：http://kp.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lb.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jj.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vi.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bv.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fa.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://uc.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hj.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cq.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://jj.9csxet.cn

Py:   Counter(arr)
来源：http://xk.asd995.cn

PHP:  array_count_values($arr);
来源：http://pd.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ct.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://no.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uv.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://wz.hnjuh.cn

Ruby: arr.tally
来源：http://hs.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ob.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://yi.szsharing.cn

Py:   x in arr
来源：http://ld.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://ll.gzmigu.cn

JS:   arr.includes(x)
来源：http://ez.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://zj.wgjwhj.cn

Java: list.contains(x)
来源：http://qv.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://vx.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://os.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://ke.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://fd.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qw.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://or.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zm.huixinmuqiang.cn

TS:   [...arr];
来源：http://ho.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://ci.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nw.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://vk.gzmigu.cn

C#:   new List<int>(list);
来源：http://cb.panjiajie.cn

[D23] reduce 累积计算
来源：http://xt.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://um.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kn.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://or.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aa.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xf.yuntaijiaju.cn

Go:   // 手写循环
来源：http://hw.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gx.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vv.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://tp.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zf.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bc.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uk.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ao.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xr.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://br.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rw.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://in.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://hh.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lr.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xi.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rb.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uy.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ao.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bs.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pz.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wm.shtwfgs.cn

[D26] 数组转字符串
来源：http://so.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://ud.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://zx.szxytkj.cn

JS:   arr.join(", ")
来源：http://lx.lnxyls.cn

TS:   arr.join(", ")
来源：http://so.9csxet.cn

Java: String.join(", ", list)
来源：http://ax.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://ji.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://am.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://ln.newstarts.cn

================================================================================
来源：http://rd.muxihuayi.cn

E. 字符串处理
来源：http://qf.lnxyls.cn

================================================================================
来源：http://tr.nicolike.cn

[E01] 拼接字符串
来源：http://lu.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kr.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://po.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zf.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://on.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ru.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://de.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hf.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lr.jianghongdianzi.cn

[E02] 重复字符串
来源：http://kq.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://rs.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://qw.hahajie.cn

JS:   "ab".repeat(3)
来源：http://pw.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://uj.szxytkj.cn

Java: "ab".repeat(3)
来源：http://mm.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://xl.colortex.cn

Ruby: "ab" * 3
来源：http://zn.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gl.haigaiapp.cn

[E03] 截取子串
来源：http://bs.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://et.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ns.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kp.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://rm.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://sk.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://el.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uf.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://di.wgjwhj.cn

[E04] 查找子串位置
来源：http://rk.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://ma.huanxung.cn

PHP:  strpos($s, "x");
来源：http://kt.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ii.panjiajie.cn

TS:   s.indexOf("x")
来源：http://xm.shxzskj.cn

Java: s.indexOf("x")
来源：http://by.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://os.521024.cn

Ruby: s.index("x")
来源：http://oh.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://gp.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bu.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yd.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://le.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mh.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ts.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hm.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yx.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eq.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rv.newstarts.cn

[E06] 替换子串
来源：http://yx.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fc.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://oj.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lm.huixinmuqiang.cn


<!-- 参考信息 -->