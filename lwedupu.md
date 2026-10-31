代发 wailian999

Java: list.add(4);
来源：http://zp.colortex.cn

Go:   arr = append(arr, 4)
来源：http://vd.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://br.521024.cn

C#:   list.Add(4);
来源：http://ca.hahajie.cn

[D03] 在指定位置插入元素
来源：http://pd.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://ja.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zg.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fc.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://xu.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://hl.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cu.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://px.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://aw.panjiajie.cn

[D04] 删除元素
来源：http://ba.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tk.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xw.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zn.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://xu.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yg.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ed.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jn.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gv.nszjky.cn

[D05] 访问与修改元素
来源：http://yb.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mk.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mi.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mj.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://cj.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://lw.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://cg.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ou.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bc.shxzukj.cn

[D06] 数组长度
来源：http://pd.hnjuh.cn

Py:   len(arr)
来源：http://vx.szxytkj.cn

PHP:  count($arr);
来源：http://gf.yuexingan06.cn

JS:   arr.length
来源：http://nt.chemitech.net.cn

TS:   arr.length
来源：http://uh.colortex.cn

Java: list.size();
来源：http://tt.yuexingan06.cn

Go:   len(arr)
来源：http://lx.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://jj.shxzskj.cn

C#:   list.Count;
来源：http://ai.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://nv.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zx.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bx.521024.cn

JS:   arr.slice(1, 4);
来源：http://el.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://yb.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://yz.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://of.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://gm.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://eg.jctech888.com.cn

[D08] 合并两个数组
来源：http://ue.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://uw.521024.cn

PHP:  array_merge($a, $b);
来源：http://wr.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tc.shxzukj.cn

TS:   [...a, ...b];
来源：http://vl.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yl.huanxung.cn

Go:   append(a, b...)
来源：http://gh.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://en.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://bz.colortex.cn

[D09] 排序（升序）
来源：http://in.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://bd.lnxyls.cn

PHP:  sort($arr);
来源：http://xu.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iy.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nd.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cf.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bi.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ui.lnxyls.cn

C#:   list.Sort();
来源：http://fu.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tv.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tj.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iw.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ss.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ir.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hd.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iu.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jk.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vn.asd995.cn

[D11] 反转数组
来源：http://kv.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dh.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://vj.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://to.gzmigu.cn

TS:   [...arr].reverse();
来源：http://sd.nszjky.cn

Java: Collections.reverse(list);
来源：http://pv.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://ox.9csxet.cn

Ruby: arr.reverse
来源：http://zr.jctech888.com.cn

C#:   list.Reverse();
来源：http://fi.yuexingan06.cn

[D12] 查找元素下标
来源：http://qw.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://vd.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://st.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iy.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xj.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qe.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://kn.wgjwhj.cn

Ruby: arr.index(x)
来源：http://yz.nicolike.cn

C#:   list.IndexOf(x);
来源：http://yy.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://lb.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ix.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xy.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://je.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://ku.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hp.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lu.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oy.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ts.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://qy.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aa.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oy.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://iw.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://lw.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eq.jctech888.com.cn

Go:   // 手写循环
来源：http://ia.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bt.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rc.colortex.cn

[D15] 去重
来源：http://xh.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iz.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://zx.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://bg.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://uy.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sp.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yg.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://im.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://cv.muxihuayi.cn

[D16] 求和与平均值
来源：http://mm.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ju.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sb.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zo.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wq.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xv.bjjhwx.cn

Go:   // 手写循环累加
来源：http://gx.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://by.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://ms.hnjuh.cn

[D17] 最大值与最小值
来源：http://nr.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://ad.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://bw.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qe.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://us.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wf.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vq.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://ku.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://sw.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://rm.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iy.colortex.cn

PHP:  array_merge(...$nested);
来源：http://nl.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cx.jctech888.com.cn

TS:   nested.flat();
来源：http://yc.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sh.wgjwhj.cn

Go:   // 手写双层循环
来源：http://xe.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://hx.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bn.yuntaijiaju.cn

[D19] 按字段分组
来源：http://mb.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qf.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fe.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://br.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ha.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pb.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://ss.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wp.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gs.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://ho.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://xv.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://ii.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gv.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nh.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fn.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://nt.gzmigu.cn

Ruby: arr.tally
来源：http://uv.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qt.huanxung.cn

[D21] 判断是否包含某元素
来源：http://ag.colortex.cn

Py:   x in arr
来源：http://pm.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://dm.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://bk.newstarts.cn

TS:   arr.includes(x)
来源：http://vg.newstarts.cn

Java: list.contains(x)
来源：http://ge.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://kx.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://ls.9csxet.cn

C#:   list.Contains(x)
来源：http://fg.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://dx.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zm.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bh.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eh.nszjky.cn

TS:   [...arr];
来源：http://ra.nszjky.cn

Java: new ArrayList<>(list);
来源：http://ch.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pn.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://qr.lnxyls.cn

C#:   new List<int>(list);
来源：http://wc.shtwfgs.cn

[D23] reduce 累积计算
来源：http://qw.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://up.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wu.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gv.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zq.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cz.haigaiapp.cn

Go:   // 手写循环
来源：http://tl.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://le.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uf.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://uj.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ss.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zz.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cs.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tn.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rj.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zc.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wy.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oc.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://sf.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lu.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cd.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ok.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ow.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cw.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hk.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ro.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fg.muxihuayi.cn

[D26] 数组转字符串
来源：http://ar.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://zj.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://bv.szsharing.cn

JS:   arr.join(", ")
来源：http://hs.newstarts.cn

TS:   arr.join(", ")
来源：http://sc.lnxyls.cn

Java: String.join(", ", list)
来源：http://eq.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://di.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://ne.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://lp.shtwfgs.cn

================================================================================
来源：http://os.9csxet.cn

E. 字符串处理
来源：http://sf.bookmarksfly.cn

================================================================================
来源：http://bw.521024.cn

[E01] 拼接字符串
来源：http://qo.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wl.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tj.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vy.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fw.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dv.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wc.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ml.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://un.521024.cn

[E02] 重复字符串
来源：http://az.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://ny.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://cm.hahajie.cn

JS:   "ab".repeat(3)
来源：http://ek.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://be.huanxung.cn

Java: "ab".repeat(3)
来源：http://qj.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://gi.shxzukj.cn

Ruby: "ab" * 3
来源：http://ng.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wi.panjiajie.cn

[E03] 截取子串
来源：http://wx.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kj.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://na.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yt.nicolike.cn

TS:   s.slice(1, 4)
来源：http://ut.9csxet.cn

Java: s.substring(1, 4)
来源：http://pa.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://by.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vs.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://vc.colortex.cn

[E04] 查找子串位置
来源：http://le.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://lt.asd995.cn

PHP:  strpos($s, "x");
来源：http://ae.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ps.huanxung.cn

TS:   s.indexOf("x")
来源：http://vk.jctech888.com.cn

Java: s.indexOf("x")
来源：http://ug.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://pv.521024.cn

Ruby: s.index("x")
来源：http://bs.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://bk.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dm.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hs.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wj.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rm.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wt.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jq.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wn.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ax.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://in.panjiajie.cn

[E06] 替换子串
来源：http://vj.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dp.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ab.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ws.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://wv.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bl.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sb.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cv.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://yj.szxytkj.cn

[E07] 按分隔符拆分
来源：http://pm.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bw.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ls.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jx.jianghongdianzi.cn

TS:   s.split(",")
来源：http://wv.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xt.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://it.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://tk.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://es.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://pe.shtwfgs.cn

Py:   ",".join(items)
来源：http://uh.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://ek.huixinmuqiang.cn

JS:   items.join(",")
来源：http://fi.9csxet.cn

TS:   items.join(",")
来源：http://dp.szsharing.cn

Java: String.join(",", items)
来源：http://mu.521024.cn

Go:   strings.Join(items, ",")
来源：http://zi.nszjky.cn

Ruby: items.join(",")
来源：http://xa.shxzskj.cn

C#:   string.Join(",", items)
来源：http://gg.hahajie.cn

[E09] 去除所有空白字符
来源：http://bv.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xr.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gr.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://xv.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://px.yuexingan06.cn


<!-- 参考信息 -->