代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://lm.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://wd.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kq.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fs.nszjky.cn

[C14] 泛型函数
来源：http://wd.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://st.shxzskj.cn

PHP:  // 无泛型
来源：http://dn.hnjuh.cn

JS:   // 无泛型
来源：http://in.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ut.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cm.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ae.jctech888.com.cn

Ruby: # 无泛型
来源：http://jo.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mf.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://rh.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ge.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://om.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ea.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://df.shtwfgs.cn

Java: // 无解构
来源：http://qr.szsharing.cn

Go:   // 无解构
来源：http://ca.newstarts.cn

Ruby: a, b = pair
来源：http://oh.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://ds.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://ep.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cp.bookmarksfly.cn

PHP:  // 无重载
来源：http://jc.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ih.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://yb.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ec.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://ee.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://ha.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://um.nicolike.cn

================================================================================
来源：http://my.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://uo.newstarts.cn

================================================================================
来源：http://tn.szsharing.cn

[D01] 创建数组 / 列表
来源：http://kq.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sx.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ar.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pl.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ny.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rs.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://da.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://hq.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rx.asd995.cn

[D02] 追加元素到末尾
来源：http://ev.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zr.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cs.szsharing.cn

JS:   arr.push(4);
来源：http://kr.chemitech.net.cn

TS:   arr.push(4);
来源：http://xf.bookmarksfly.cn

Java: list.add(4);
来源：http://li.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://cd.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://vn.wgjwhj.cn

C#:   list.Add(4);
来源：http://cp.521024.cn

[D03] 在指定位置插入元素
来源：http://sn.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://kb.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kk.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fu.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://td.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://pz.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mg.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oa.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://se.bookmarksfly.cn

[D04] 删除元素
来源：http://hg.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sg.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fq.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ib.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://wt.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fd.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rr.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eq.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://si.jctech888.com.cn

[D05] 访问与修改元素
来源：http://tb.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lc.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fe.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kq.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://nh.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://uz.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://nc.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nn.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qo.szsharing.cn

[D06] 数组长度
来源：http://dr.szsharing.cn

Py:   len(arr)
来源：http://xf.bjjhwx.cn

PHP:  count($arr);
来源：http://rq.szxytkj.cn

JS:   arr.length
来源：http://km.asd995.cn

TS:   arr.length
来源：http://mz.yuntaijiaju.cn

Java: list.size();
来源：http://zh.lnxyls.cn

Go:   len(arr)
来源：http://ln.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://nj.chemitech.net.cn

C#:   list.Count;
来源：http://er.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://bq.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rq.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://es.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://lf.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://ha.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://wm.bjjhwx.cn

Go:   arr[1:4]
来源：http://rw.hahajie.cn

Ruby: arr[1, 3]
来源：http://rg.521024.cn

C#:   list.GetRange(1, 3);
来源：http://zg.jctech888.com.cn

[D08] 合并两个数组
来源：http://un.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://un.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://xg.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jd.newstarts.cn

TS:   [...a, ...b];
来源：http://hw.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jy.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://cj.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://wm.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://vj.huixiangedu.cn

[D09] 排序（升序）
来源：http://wd.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://yi.asd995.cn

PHP:  sort($arr);
来源：http://xp.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gu.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mr.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ti.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vl.shxzskj.cn

Ruby: arr.sort
来源：http://mk.jianghongdianzi.cn

C#:   list.Sort();
来源：http://ta.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lb.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://py.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ya.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gb.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mq.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qq.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xz.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vg.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://up.bookmarksfly.cn

[D11] 反转数组
来源：http://zu.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://er.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://fg.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lr.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://qf.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://xd.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://ms.asd995.cn

Ruby: arr.reverse
来源：http://hc.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://jq.jctech888.com.cn

[D12] 查找元素下标
来源：http://br.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://vx.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wz.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wo.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sr.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fr.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://fe.gzmigu.cn

Ruby: arr.index(x)
来源：http://fu.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://nq.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://jk.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vw.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://be.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://qr.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://gf.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cq.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ga.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ds.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yd.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://nu.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://et.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fk.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://un.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://dq.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ii.hnjuh.cn

Go:   // 手写循环
来源：http://pi.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ul.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://om.jctech888.com.cn

[D15] 去重
来源：http://df.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hc.521024.cn

PHP:  array_unique($arr);
来源：http://zq.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://pg.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://ir.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zd.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wj.bookmarksfly.cn

Ruby: arr.uniq
来源：http://sh.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://kw.hnjuh.cn

[D16] 求和与平均值
来源：http://rr.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xh.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jg.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ce.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sm.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://as.colortex.cn

Go:   // 手写循环累加
来源：http://wj.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jp.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://gi.shxzukj.cn

[D17] 最大值与最小值
来源：http://ha.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://ws.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://gu.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dn.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://ai.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lg.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bc.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://nl.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://gc.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://sn.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://if.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://ja.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cj.haigaiapp.cn

TS:   nested.flat();
来源：http://zl.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ma.szxytkj.cn

Go:   // 手写双层循环
来源：http://gg.shxzskj.cn

Ruby: nested.flatten
来源：http://ny.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zo.nicolike.cn

[D19] 按字段分组
来源：http://wu.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bz.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dx.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ov.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vg.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mv.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://oq.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kg.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tr.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://aj.521024.cn

Py:   Counter(arr)
来源：http://xb.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://rm.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xi.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yb.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uc.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://hg.hnjuh.cn

Ruby: arr.tally
来源：http://vg.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kr.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://nk.szxytkj.cn

Py:   x in arr
来源：http://qk.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://uh.chemitech.net.cn

JS:   arr.includes(x)
来源：http://od.colortex.cn

TS:   arr.includes(x)
来源：http://we.shxzskj.cn

Java: list.contains(x)
来源：http://se.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://cp.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://ft.colortex.cn

C#:   list.Contains(x)
来源：http://qs.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://vd.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gv.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://to.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bv.newstarts.cn

TS:   [...arr];
来源：http://ij.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://nv.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ft.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://qa.wgjwhj.cn

C#:   new List<int>(list);
来源：http://pu.hnjuh.cn

[D23] reduce 累积计算
来源：http://bq.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mu.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fj.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bz.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://js.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xv.hahajie.cn

Go:   // 手写循环
来源：http://as.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yi.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zo.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://lp.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hc.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yo.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kr.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zg.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hx.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mw.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jz.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uv.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://tp.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qc.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nu.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hf.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xr.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eg.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yd.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pr.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sx.szxytkj.cn

[D26] 数组转字符串
来源：http://wi.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://lf.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://yn.newstarts.cn

JS:   arr.join(", ")
来源：http://vp.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://ha.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://pr.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://zi.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://jf.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://rv.nicolike.cn

================================================================================
来源：http://ag.bjjhwx.cn

E. 字符串处理
来源：http://cg.panjiajie.cn

================================================================================
来源：http://rw.shtwfgs.cn

[E01] 拼接字符串
来源：http://hp.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tu.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://il.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tx.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oe.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://je.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lu.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qb.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zx.huixinmuqiang.cn

[E02] 重复字符串
来源：http://ut.panjiajie.cn

Py:   "ab" * 3
来源：http://ng.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://fx.huanxung.cn

JS:   "ab".repeat(3)
来源：http://hd.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://bo.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://lb.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://nw.nicolike.cn

Ruby: "ab" * 3
来源：http://sf.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sv.yuexingan06.cn

[E03] 截取子串
来源：http://ta.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yo.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fi.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pt.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://du.nicolike.cn

Java: s.substring(1, 4)
来源：http://jk.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://or.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jz.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://nm.gzmigu.cn

[E04] 查找子串位置
来源：http://wz.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://jq.newstarts.cn


<!-- 参考信息 -->