代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uu.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rw.hahajie.cn

Java: // 无解构
来源：http://zt.hahajie.cn

Go:   // 无解构
来源：http://kq.szxytkj.cn

Ruby: a, b = pair
来源：http://cm.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://uu.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://pj.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cy.nszjky.cn

PHP:  // 无重载
来源：http://rg.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wq.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://hh.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ix.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://sh.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://hz.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yn.gzmigu.cn

================================================================================
来源：http://uq.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://ho.chemitech.net.cn

================================================================================
来源：http://ys.asd995.cn

[D01] 创建数组 / 列表
来源：http://pc.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bo.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cw.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wo.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://su.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rw.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://oo.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://jp.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oo.asd995.cn

[D02] 追加元素到末尾
来源：http://nz.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ni.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rn.shtwfgs.cn

JS:   arr.push(4);
来源：http://fq.newstarts.cn

TS:   arr.push(4);
来源：http://ks.huixinmuqiang.cn

Java: list.add(4);
来源：http://hc.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://zs.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://jf.yuexingan06.cn

C#:   list.Add(4);
来源：http://sf.nszjky.cn

[D03] 在指定位置插入元素
来源：http://ji.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://kc.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://su.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gx.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://ud.chemitech.net.cn

Java: list.add(0, 0);
来源：http://qa.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ow.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fd.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://uc.bjjhwx.cn

[D04] 删除元素
来源：http://dd.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pu.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ox.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gr.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://fr.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zh.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pc.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mu.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yw.asd995.cn

[D05] 访问与修改元素
来源：http://qe.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ic.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zr.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gr.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://oc.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://li.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://gr.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fy.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ju.chemitech.net.cn

[D06] 数组长度
来源：http://jp.9csxet.cn

Py:   len(arr)
来源：http://aq.jianghongdianzi.cn

PHP:  count($arr);
来源：http://yz.muxihuayi.cn

JS:   arr.length
来源：http://bu.hahajie.cn

TS:   arr.length
来源：http://mb.gzmigu.cn

Java: list.size();
来源：http://xe.nicolike.cn

Go:   len(arr)
来源：http://jb.newstarts.cn

Ruby: arr.length; arr.size
来源：http://xn.bookmarksfly.cn

C#:   list.Count;
来源：http://tk.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://kf.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ki.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kx.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://qy.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://jj.hahajie.cn

Java: list.subList(1, 4);
来源：http://yu.huanxung.cn

Go:   arr[1:4]
来源：http://kq.lnxyls.cn

Ruby: arr[1, 3]
来源：http://fk.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://ei.colortex.cn

[D08] 合并两个数组
来源：http://ih.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://si.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://av.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zr.haigaiapp.cn

TS:   [...a, ...b];
来源：http://jf.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dw.lnxyls.cn

Go:   append(a, b...)
来源：http://dn.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://ql.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://eh.9csxet.cn

[D09] 排序（升序）
来源：http://wh.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jb.yuexingan06.cn

PHP:  sort($arr);
来源：http://rw.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mk.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wo.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hy.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vg.521024.cn

Ruby: arr.sort
来源：http://jf.shxzskj.cn

C#:   list.Sort();
来源：http://nf.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kx.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ot.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://da.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://si.huixiangedu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zf.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bc.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ff.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vv.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wm.huixinmuqiang.cn

[D11] 反转数组
来源：http://dq.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fk.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://xl.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jo.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://rg.521024.cn

Java: Collections.reverse(list);
来源：http://la.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://yk.colortex.cn

Ruby: arr.reverse
来源：http://ky.gzmigu.cn

C#:   list.Reverse();
来源：http://hg.shxzukj.cn

[D12] 查找元素下标
来源：http://kz.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://is.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gf.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ir.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bn.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eq.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://wt.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://pa.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://ve.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://xr.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ot.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jx.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://ew.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://we.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bz.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tx.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vq.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nc.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://jf.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hk.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xa.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://re.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://mf.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fi.shxzukj.cn

Go:   // 手写循环
来源：http://ab.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ju.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wt.521024.cn

[D15] 去重
来源：http://ss.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ny.hnjuh.cn

PHP:  array_unique($arr);
来源：http://bs.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://lj.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://qb.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hc.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jb.huanxung.cn

Ruby: arr.uniq
来源：http://pu.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://nj.nszjky.cn

[D16] 求和与平均值
来源：http://mr.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qu.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jj.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://om.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rr.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jm.shxzukj.cn

Go:   // 手写循环累加
来源：http://ye.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wi.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://tb.haigaiapp.cn

[D17] 最大值与最小值
来源：http://wq.colortex.cn

Py:   max(arr);  min(arr)
来源：http://ab.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://pb.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jd.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://ib.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ej.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://be.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://qb.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://ri.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://gj.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ab.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://tl.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ve.huixiangedu.cn

TS:   nested.flat();
来源：http://xn.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ma.yuexingan06.cn

Go:   // 手写双层循环
来源：http://fu.9csxet.cn

Ruby: nested.flatten
来源：http://fp.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yy.yuexingan06.cn

[D19] 按字段分组
来源：http://yt.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ju.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lw.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iq.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yn.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://of.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://at.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fz.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bs.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://aq.jctech888.com.cn

Py:   Counter(arr)
来源：http://yk.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://sd.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ty.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iy.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yw.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://sv.nicolike.cn

Ruby: arr.tally
来源：http://fy.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ir.hahajie.cn

[D21] 判断是否包含某元素
来源：http://fq.shxzskj.cn

Py:   x in arr
来源：http://om.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://do.yuexingan06.cn

JS:   arr.includes(x)
来源：http://zs.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://ao.nicolike.cn

Java: list.contains(x)
来源：http://ne.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://md.9csxet.cn

Ruby: arr.include?(x)
来源：http://ff.lnxyls.cn

C#:   list.Contains(x)
来源：http://tt.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://nk.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gx.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://in.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uh.9csxet.cn

TS:   [...arr];
来源：http://jf.nszjky.cn

Java: new ArrayList<>(list);
来源：http://iw.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ly.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://ro.lnxyls.cn

C#:   new List<int>(list);
来源：http://zu.521024.cn

[D23] reduce 累积计算
来源：http://rs.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ui.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rm.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pb.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oj.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pu.panjiajie.cn

Go:   // 手写循环
来源：http://uh.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wl.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sv.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://ex.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ju.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zy.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mj.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sa.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://la.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ld.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yj.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jf.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://hr.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tw.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ee.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ft.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tn.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vw.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ff.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mk.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wp.shxzskj.cn

[D26] 数组转字符串
来源：http://pz.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://wk.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://ul.shtwfgs.cn

JS:   arr.join(", ")
来源：http://pp.panjiajie.cn

TS:   arr.join(", ")
来源：http://yt.muxihuayi.cn

Java: String.join(", ", list)
来源：http://mq.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://zw.hnjuh.cn

Ruby: arr.join(", ")
来源：http://em.newstarts.cn

C#:   string.Join(", ", list)
来源：http://ye.bookmarksfly.cn

================================================================================
来源：http://in.asd995.cn

E. 字符串处理
来源：http://jc.huanxung.cn

================================================================================
来源：http://af.szsharing.cn

[E01] 拼接字符串
来源：http://jq.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kd.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xq.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ku.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://za.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ar.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lq.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xe.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vi.hahajie.cn

[E02] 重复字符串
来源：http://yw.bookmarksfly.cn

Py:   "ab" * 3
来源：http://ld.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://an.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://fp.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://lw.nszjky.cn

Java: "ab".repeat(3)
来源：http://vr.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://gb.asd995.cn

Ruby: "ab" * 3
来源：http://qh.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zg.shtwfgs.cn

[E03] 截取子串
来源：http://oa.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ta.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hk.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yi.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://lz.521024.cn

Java: s.substring(1, 4)
来源：http://ld.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vz.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://la.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://eh.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://cr.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://tb.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://gf.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lr.9csxet.cn

TS:   s.indexOf("x")
来源：http://ba.gzmigu.cn

Java: s.indexOf("x")
来源：http://nx.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://dz.gzmigu.cn

Ruby: s.index("x")
来源：http://gb.nszjky.cn

C#:   s.IndexOf("x")
来源：http://bh.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qc.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://py.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qb.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ev.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mk.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vz.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cg.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fl.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://up.shxzukj.cn


<!-- 参考信息 -->