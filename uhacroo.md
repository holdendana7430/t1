代发 wailian999

Ruby: a, b = pair
来源：http://gg.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://fp.nicolike.cn

[C16] 函数 / 方法重载
来源：http://gz.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ur.muxihuayi.cn

PHP:  // 无重载
来源：http://jm.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ot.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ri.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dz.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://fu.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://ya.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://il.nszjky.cn

================================================================================
来源：http://vb.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://xu.lnxyls.cn

================================================================================
来源：http://hn.newstarts.cn

[D01] 创建数组 / 列表
来源：http://xz.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bg.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wm.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ki.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qh.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wc.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://qq.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://it.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uh.szsharing.cn

[D02] 追加元素到末尾
来源：http://yt.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://st.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hs.9csxet.cn

JS:   arr.push(4);
来源：http://zj.newstarts.cn

TS:   arr.push(4);
来源：http://ec.lnxyls.cn

Java: list.add(4);
来源：http://dw.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://kc.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://fn.hnjuh.cn

C#:   list.Add(4);
来源：http://oc.colortex.cn

[D03] 在指定位置插入元素
来源：http://mp.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://ah.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wh.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pc.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ad.bjjhwx.cn

Java: list.add(0, 0);
来源：http://yz.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://co.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hi.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://hv.asd995.cn

[D04] 删除元素
来源：http://ev.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jj.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fz.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fj.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://on.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fi.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jz.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tn.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ig.shxzukj.cn

[D05] 访问与修改元素
来源：http://tt.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ju.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sv.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xo.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://yv.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://cp.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://en.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sc.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sh.9csxet.cn

[D06] 数组长度
来源：http://rz.hnjuh.cn

Py:   len(arr)
来源：http://qa.521024.cn

PHP:  count($arr);
来源：http://pc.yuexingan06.cn

JS:   arr.length
来源：http://da.yuexingan06.cn

TS:   arr.length
来源：http://ph.521024.cn

Java: list.size();
来源：http://hg.newstarts.cn

Go:   len(arr)
来源：http://xt.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://by.shxzukj.cn

C#:   list.Count;
来源：http://pf.521024.cn

[D07] 切片 / 取子数组
来源：http://lz.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ao.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://um.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://ho.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://da.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://md.muxihuayi.cn

Go:   arr[1:4]
来源：http://lu.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://mt.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://ee.huixiangedu.cn

[D08] 合并两个数组
来源：http://wu.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://aw.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://hs.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kq.huanxung.cn

TS:   [...a, ...b];
来源：http://xg.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://td.hahajie.cn

Go:   append(a, b...)
来源：http://wy.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://cx.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://hh.asd995.cn

[D09] 排序（升序）
来源：http://td.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://eh.nszjky.cn

PHP:  sort($arr);
来源：http://ei.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zj.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ot.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pb.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jf.asd995.cn

Ruby: arr.sort
来源：http://vd.asd995.cn

C#:   list.Sort();
来源：http://tv.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mz.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fp.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yj.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://br.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ze.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yc.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kh.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tl.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qy.nszjky.cn

[D11] 反转数组
来源：http://bi.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tr.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://gd.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mc.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://gl.nicolike.cn

Java: Collections.reverse(list);
来源：http://on.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://xz.shxzukj.cn

Ruby: arr.reverse
来源：http://xj.yuexingan06.cn

C#:   list.Reverse();
来源：http://bc.521024.cn

[D12] 查找元素下标
来源：http://pl.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://sy.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fr.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fs.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lm.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gj.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://hx.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://vt.szsharing.cn

C#:   list.IndexOf(x);
来源：http://jk.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://fk.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oc.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jo.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://cy.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://id.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zk.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pu.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://js.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://co.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://am.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wy.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fs.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://mn.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://uv.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jy.gzmigu.cn

Go:   // 手写循环
来源：http://eh.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eq.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://is.lnxyls.cn

[D15] 去重
来源：http://tl.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jp.szxytkj.cn

PHP:  array_unique($arr);
来源：http://gp.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://xx.nszjky.cn

TS:   [...new Set(arr)]
来源：http://qa.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tz.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nq.nszjky.cn

Ruby: arr.uniq
来源：http://cv.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://qs.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://xc.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yy.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fk.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eu.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pd.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iz.huixiangedu.cn

Go:   // 手写循环累加
来源：http://rd.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nu.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://nl.521024.cn

[D17] 最大值与最小值
来源：http://ra.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://hr.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://ga.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vp.9csxet.cn

TS:   Math.max(...arr);
来源：http://fi.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jz.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ex.colortex.cn

Ruby: arr.max;  arr.min
来源：http://zh.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://bb.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://at.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pt.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ew.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vc.muxihuayi.cn

TS:   nested.flat();
来源：http://cz.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rm.bjjhwx.cn

Go:   // 手写双层循环
来源：http://ex.haigaiapp.cn

Ruby: nested.flatten
来源：http://yo.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tx.colortex.cn

[D19] 按字段分组
来源：http://fd.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ew.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pq.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jw.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ra.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ul.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://wu.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cc.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vv.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://se.nicolike.cn

Py:   Counter(arr)
来源：http://ce.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://dx.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lt.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oi.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kv.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://tz.nszjky.cn

Ruby: arr.tally
来源：http://pc.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cm.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://qu.yuntaijiaju.cn

Py:   x in arr
来源：http://ot.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://qg.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://am.huanxung.cn

TS:   arr.includes(x)
来源：http://zd.nszjky.cn

Java: list.contains(x)
来源：http://yq.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://ez.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://oo.hnjuh.cn

C#:   list.Contains(x)
来源：http://dp.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://du.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qc.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zd.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pm.521024.cn

TS:   [...arr];
来源：http://ut.colortex.cn

Java: new ArrayList<>(list);
来源：http://mr.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fc.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://wj.bjjhwx.cn

C#:   new List<int>(list);
来源：http://ia.gzmigu.cn

[D23] reduce 累积计算
来源：http://nr.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://am.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pn.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jo.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mq.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eu.szxytkj.cn

Go:   // 手写循环
来源：http://pb.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xz.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rp.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://od.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ys.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fk.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kc.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xz.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nm.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lw.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nu.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mx.asd995.cn

[D25] Set 集合去重与交并差
来源：http://kt.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zt.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dh.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yr.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kg.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zy.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hy.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rm.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pj.muxihuayi.cn

[D26] 数组转字符串
来源：http://qk.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://ub.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://rl.yuexingan06.cn

JS:   arr.join(", ")
来源：http://or.9csxet.cn

TS:   arr.join(", ")
来源：http://zo.muxihuayi.cn

Java: String.join(", ", list)
来源：http://na.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://px.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://hl.nicolike.cn

C#:   string.Join(", ", list)
来源：http://zb.gzmigu.cn

================================================================================
来源：http://mk.yuntaijiaju.cn

E. 字符串处理
来源：http://jt.hahajie.cn

================================================================================
来源：http://ms.9csxet.cn

[E01] 拼接字符串
来源：http://vr.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bb.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aq.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lt.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://im.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ui.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cp.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fy.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ig.hahajie.cn

[E02] 重复字符串
来源：http://wx.hahajie.cn

Py:   "ab" * 3
来源：http://tn.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://nk.szsharing.cn

JS:   "ab".repeat(3)
来源：http://yw.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://gg.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://vn.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://ej.szxytkj.cn

Ruby: "ab" * 3
来源：http://al.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mi.colortex.cn

[E03] 截取子串
来源：http://ay.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hm.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ga.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gj.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://yw.nicolike.cn

Java: s.substring(1, 4)
来源：http://li.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mb.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dl.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://ow.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://io.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://kk.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://dk.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ys.hnjuh.cn

TS:   s.indexOf("x")
来源：http://go.521024.cn

Java: s.indexOf("x")
来源：http://uj.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://uc.521024.cn

Ruby: s.index("x")
来源：http://rd.asd995.cn

C#:   s.IndexOf("x")
来源：http://uh.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://up.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wj.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gi.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sn.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://si.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mm.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zv.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lw.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dk.521024.cn

[E06] 替换子串
来源：http://uk.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://to.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://uh.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jt.yuexingan06.cn


<!-- 参考信息 -->