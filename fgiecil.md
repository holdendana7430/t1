代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tz.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tg.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ze.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ti.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bl.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://zj.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jz.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ih.huixinmuqiang.cn

[C14] 泛型函数
来源：http://to.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bh.szxytkj.cn

PHP:  // 无泛型
来源：http://it.jctech888.com.cn

JS:   // 无泛型
来源：http://xo.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ch.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://op.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bx.shxzukj.cn

Ruby: # 无泛型
来源：http://oh.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zk.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://de.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yr.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://tl.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jy.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ia.muxihuayi.cn

Java: // 无解构
来源：http://qu.szxytkj.cn

Go:   // 无解构
来源：http://wz.panjiajie.cn

Ruby: a, b = pair
来源：http://ma.newstarts.cn

C#:   var (a, b) = pair;
来源：http://eb.colortex.cn

[C16] 函数 / 方法重载
来源：http://tn.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tl.huixiangedu.cn

PHP:  // 无重载
来源：http://vp.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://va.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://wx.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ke.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://ph.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://pa.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hh.huanxung.cn

================================================================================
来源：http://md.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://qc.nicolike.cn

================================================================================
来源：http://iw.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://zd.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qu.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fu.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ds.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zo.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ew.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://hq.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://nw.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kj.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://dn.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oq.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rs.szxytkj.cn

JS:   arr.push(4);
来源：http://gc.muxihuayi.cn

TS:   arr.push(4);
来源：http://zm.muxihuayi.cn

Java: list.add(4);
来源：http://tg.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://mo.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://ur.hahajie.cn

C#:   list.Add(4);
来源：http://dx.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://dl.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://wm.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fc.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://or.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://zy.panjiajie.cn

Java: list.add(0, 0);
来源：http://ip.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://to.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ac.521024.cn

C#:   list.Insert(0, 0);
来源：http://jt.huixiangedu.cn

[D04] 删除元素
来源：http://kc.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rf.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xg.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ja.colortex.cn

TS:   arr.splice(0, 1);
来源：http://qy.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aj.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zn.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eo.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jd.shxzukj.cn

[D05] 访问与修改元素
来源：http://ou.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lh.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://za.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sw.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://bx.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://qf.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://hv.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://er.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ke.szxytkj.cn

[D06] 数组长度
来源：http://hb.wgjwhj.cn

Py:   len(arr)
来源：http://yh.nszjky.cn

PHP:  count($arr);
来源：http://wf.yuntaijiaju.cn

JS:   arr.length
来源：http://kv.chemitech.net.cn

TS:   arr.length
来源：http://np.shtwfgs.cn

Java: list.size();
来源：http://us.panjiajie.cn

Go:   len(arr)
来源：http://xq.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://hs.newstarts.cn

C#:   list.Count;
来源：http://qm.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://zp.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ja.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cn.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://tq.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://ot.hahajie.cn

Java: list.subList(1, 4);
来源：http://ff.wgjwhj.cn

Go:   arr[1:4]
来源：http://zd.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://hz.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://fz.haigaiapp.cn

[D08] 合并两个数组
来源：http://xb.521024.cn

Py:   a + b;  a.extend(b)
来源：http://bt.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://co.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tg.nszjky.cn

TS:   [...a, ...b];
来源：http://lm.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://er.colortex.cn

Go:   append(a, b...)
来源：http://nw.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://cw.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://xx.521024.cn

[D09] 排序（升序）
来源：http://mm.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://dm.shtwfgs.cn

PHP:  sort($arr);
来源：http://pn.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hn.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ba.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dt.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ca.521024.cn

Ruby: arr.sort
来源：http://ci.huanxung.cn

C#:   list.Sort();
来源：http://et.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jy.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dk.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ln.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://at.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qa.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qd.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pg.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yi.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yv.nszjky.cn

[D11] 反转数组
来源：http://en.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sx.nszjky.cn

PHP:  array_reverse($arr);
来源：http://qf.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vj.lnxyls.cn

TS:   [...arr].reverse();
来源：http://wc.9csxet.cn

Java: Collections.reverse(list);
来源：http://wo.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://tr.9csxet.cn

Ruby: arr.reverse
来源：http://in.colortex.cn

C#:   list.Reverse();
来源：http://mc.gzmigu.cn

[D12] 查找元素下标
来源：http://gp.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://by.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tm.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lm.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pz.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jb.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://dw.9csxet.cn

Ruby: arr.index(x)
来源：http://nb.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://ei.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://ui.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nm.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://br.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://jj.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://oq.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cz.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ox.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://us.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yy.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://yf.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wq.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cw.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://fv.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://mg.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gh.newstarts.cn

Go:   // 手写循环
来源：http://ex.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tz.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oi.jctech888.com.cn

[D15] 去重
来源：http://fm.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hl.shxzukj.cn

PHP:  array_unique($arr);
来源：http://jy.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://sp.hahajie.cn

TS:   [...new Set(arr)]
来源：http://qs.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yq.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hp.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://kz.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://yp.nicolike.cn

[D16] 求和与平均值
来源：http://by.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uk.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eh.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wm.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qm.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pw.hnjuh.cn

Go:   // 手写循环累加
来源：http://xt.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gt.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://bl.shtwfgs.cn

[D17] 最大值与最小值
来源：http://al.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://ug.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://wd.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hx.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://wb.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ix.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rp.colortex.cn

Ruby: arr.max;  arr.min
来源：http://ad.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://ma.521024.cn

[D18] 扁平化嵌套数组
来源：http://zm.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://et.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://bk.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qk.shxzskj.cn

TS:   nested.flat();
来源：http://pp.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://of.shtwfgs.cn

Go:   // 手写双层循环
来源：http://fl.9csxet.cn

Ruby: nested.flatten
来源：http://pa.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gl.szsharing.cn

[D19] 按字段分组
来源：http://cm.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://it.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cs.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gv.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mm.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xr.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://ha.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fk.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://po.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://qc.haigaiapp.cn

Py:   Counter(arr)
来源：http://ck.szsharing.cn

PHP:  array_count_values($arr);
来源：http://lq.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dw.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rq.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bc.nicolike.cn

Go:   // 手写 map[T]int
来源：http://rt.newstarts.cn

Ruby: arr.tally
来源：http://it.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yf.9csxet.cn

[D21] 判断是否包含某元素
来源：http://eh.bjjhwx.cn

Py:   x in arr
来源：http://se.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://zd.bjjhwx.cn

JS:   arr.includes(x)
来源：http://fm.hahajie.cn

TS:   arr.includes(x)
来源：http://vf.szsharing.cn

Java: list.contains(x)
来源：http://fw.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://qv.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://gg.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://ag.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://ue.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qt.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ka.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zr.shtwfgs.cn

TS:   [...arr];
来源：http://tb.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://ze.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dr.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://zs.szxytkj.cn

C#:   new List<int>(list);
来源：http://or.muxihuayi.cn

[D23] reduce 累积计算
来源：http://wf.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xv.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mb.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xe.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gz.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ov.chemitech.net.cn

Go:   // 手写循环
来源：http://il.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dr.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ko.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://pc.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cp.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://np.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ey.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vt.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qb.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wf.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vs.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kr.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://mo.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zj.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gh.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vm.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bl.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hr.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sw.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vi.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://go.hahajie.cn

[D26] 数组转字符串
来源：http://dq.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://hj.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://vb.huanxung.cn

JS:   arr.join(", ")
来源：http://dy.bjjhwx.cn

TS:   arr.join(", ")
来源：http://qu.asd995.cn

Java: String.join(", ", list)
来源：http://zd.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://sa.gzmigu.cn

Ruby: arr.join(", ")
来源：http://sj.huanxung.cn

C#:   string.Join(", ", list)
来源：http://pi.shxzukj.cn

================================================================================
来源：http://ef.asd995.cn

E. 字符串处理
来源：http://ir.chemitech.net.cn

================================================================================
来源：http://yv.hahajie.cn

[E01] 拼接字符串
来源：http://zu.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tf.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hn.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sm.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://va.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bo.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mc.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pg.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fm.szsharing.cn

[E02] 重复字符串
来源：http://ux.shxzukj.cn

Py:   "ab" * 3
来源：http://nw.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://pz.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://un.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://ln.newstarts.cn

Java: "ab".repeat(3)
来源：http://lp.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://qv.huixiangedu.cn

Ruby: "ab" * 3
来源：http://vv.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lu.jctech888.com.cn

[E03] 截取子串
来源：http://fl.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://io.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rz.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xa.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://ar.hahajie.cn

Java: s.substring(1, 4)
来源：http://dw.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gc.szxytkj.cn


<!-- 参考信息 -->